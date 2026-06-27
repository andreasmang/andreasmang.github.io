---
layout: default
title: Publications
heading: Selected Publications
---

A more complete list of publications can be found on my [Google Scholar profile](https://scholar.google.com/citations?user=CJc0_msAAAAJ&hl=en).

<div class="pub-filters">
  <div class="pub-filter-group" role="group" aria-label="Filter publications by type">
    <button type="button" class="pub-filter active" data-filter-type="all" aria-pressed="true">All</button>
    <button type="button" class="pub-filter" data-filter-type="journal" aria-pressed="false">Journal</button>
    <button type="button" class="pub-filter" data-filter-type="preprint" aria-pressed="false">Preprint</button>
    <button type="button" class="pub-filter" data-filter-type="conference" aria-pressed="false">Conference</button>
    <button type="button" class="pub-filter" data-filter-type="book" aria-pressed="false">Book</button>
    <button type="button" class="pub-filter" data-filter-type="bookchapter" aria-pressed="false">Chapter</button>
  </div>
  <label class="pub-year-filter">Year
    <select id="pub-year-select">
      <option value="all">All</option>
      {% assign years = site.data.publications | map: "year" | uniq | sort | reverse %}
      {% for y in years %}<option value="{{ y }}">{{ y }}</option>
      {% endfor %}
    </select>
  </label>
</div>

<ul class="pub-list">
{% for pub in site.data.publications %}  <li class="pub-item" data-category="{{ pub.category }}" data-year="{{ pub.year }}">{% if pub.authors and pub.authors.size > 0 %}{{ pub.authors }}, {% endif %}<em>{{ pub.title }}</em>.{% if pub.venue != "" %} {{ pub.venue }}.{% endif %}{% if pub.doi %} <a href="{{ pub.doi }}">doi</a>{% endif %}{% if pub.arxiv %} <a href="{{ pub.arxiv }}">arXiv</a>{% endif %} {% if pub.category == "bookchapter" %}<span class="pub-category bookchapter">chapter</span>{% elsif pub.category == "book" %}<span class="pub-category book">book</span>{% else %}<span class="pub-category {{ pub.category }}">{{ pub.category }}</span>{% endif %}</li>
{% endfor %}</ul>

<p class="pub-empty" hidden>No publications match the selected filters.</p>

<script>
(function () {
  var typeBtns = Array.prototype.slice.call(document.querySelectorAll('.pub-filter'));
  var yearSel = document.getElementById('pub-year-select');
  var items = Array.prototype.slice.call(document.querySelectorAll('.pub-item'));
  var empty = document.querySelector('.pub-empty');
  var curType = 'all';

  function apply() {
    var curYear = yearSel ? yearSel.value : 'all';
    var visible = 0;
    items.forEach(function (it) {
      var okType = curType === 'all' || it.getAttribute('data-category') === curType;
      var okYear = curYear === 'all' || it.getAttribute('data-year') === curYear;
      var show = okType && okYear;
      it.hidden = !show;
      if (show) { visible++; }
    });
    if (empty) { empty.hidden = visible !== 0; }
  }

  typeBtns.forEach(function (btn) {
    btn.addEventListener('click', function () {
      curType = this.getAttribute('data-filter-type');
      typeBtns.forEach(function (b) {
        var active = b === btn;
        b.classList.toggle('active', active);
        b.setAttribute('aria-pressed', active ? 'true' : 'false');
      });
      apply();
    });
  });

  if (yearSel) { yearSel.addEventListener('change', apply); }
})();
</script>
