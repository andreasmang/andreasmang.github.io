---
layout: default
title: Research
description: "Research of Andreas Mang: inverse problems, PDE-constrained optimization, scientific machine learning, and scalable algorithms."
---

I am a member of the Numerical Analysis & Scientific Computing group. I am the head of the **SCOPA** (Scientific Computing, Optimization, and Parallel Algorithms) lab. You can find more information on the [SCOPA webpage](https://scopagroup.github.io). A list of my publications is available [here](/publications/), and a selection of my [talks](/talks/) is also available.

My key research areas include:

- scientific machine learning and data-driven modeling
- inverse problems and PDE-constrained optimization
- numerical optimization, including optimization for machine learning
- tensor methods, model reduction, and surrogate models
- uncertainty quantification and Bayesian inference
- nonlinear optimal control
- geometric methods and the analysis of shapes and manifold-valued data
- scalable, parallel, and GPU-accelerated algorithms

The goal of my research is the design of principled and scalable algorithms at the interface of machine learning, optimization, and scientific computing that integrate *data* with *simulation* to enable data-driven discovery in the applied sciences. I am interested in methods that combine the interpretability and predictive power of mechanistic models with the flexibility of learning, and in the numerical analysis that makes them trustworthy &mdash; stability, structure preservation, and a rigorous accounting of uncertainty. My work is driven by applications in medical imaging and the life sciences, and much of it is released as open-source software for GPU and supercomputing platforms.

**Integrating models with data.** Much of my work concerns settings in which a mechanistic model &mdash; typically a system of differential equations &mdash; must be reconciled with observations. This leads to large-scale problems that are nonconvex, ill-posed, and expensive to solve. I am interested in formulations that respect the structure of the underlying problem, in fast solvers that make such problems tractable at realistic scale, and in Bayesian and randomized techniques that quantify the uncertainty of the resulting estimates.

**Learning and numerics.** Mechanistic models are interpretable and extrapolate beyond the data, but they are costly; learned models are fast and flexible, but can be opaque and unreliable outside the regime they were trained on. A growing part of my work combines the two in a principled way, through continuous-time and dynamical-systems formulations of learning, structure- and stability-preserving discretizations, optimization methods for training, and surrogate and operator-learning frameworks. The guiding question is how to bring the standards of numerical analysis &mdash; stability, convergence, well-posedness &mdash; to methods that learn from data.

**Reduction and scale.** Making these problems affordable is itself a mathematical question. Tensor-based reduced-order models and learned surrogates compress parametric models into forms cheap enough for many-query settings such as model calibration, uncertainty quantification, and digital twins. Complementing this, I design parallel and GPU-accelerated algorithms so that the resulting methods scale from a workstation to a supercomputer.

**Geometry and applications.** Many of the objects I work with &mdash; images, shapes, deformations, and covariance structures &mdash; do not live in flat vector spaces, and respecting their geometry is often what makes an algorithm both meaningful and efficient. These methods are driven by applications in medical imaging and the life sciences, including computational anatomy, biophysical modeling of disease progression, cardiology, and systems biology.

### SCOPA Members

- **Pegah Amiri**, PhD Student
- **Christopher Chukwuemeka**, PhD Student
- **Asikul Islam**, PhD Student
- **Samundra Regmi**, PhD Student (co-advised with Dr. Charon)

### Former SCOPA Members

<details markdown="1">
<summary>Click to expand</summary>

- Jannatul Chhoa, PhD Student (co-advised with Dr. He), 2021&ndash;2025
- Dinh Binh Le, Undergraduate Student (2025 SURF Recipient)
- Radmir Sultamuratov, PhD Student (co-advised with Dr. Azencott), 2021&ndash;2024
- Mayank Konduri, High School Student, 2023&ndash;2024
- Anjalee Nair, Undergraduate Student (2024 SURF Recipient), Summer 2024
- Li Meng, Graduate Student, 2023&ndash;2024
- German Villalobos, PhD Student, 2020&ndash;2023
- Brayan Gutierrez, Undergraduate Student (2023 SURF Recipient), Summer 2023
- Jae Youn Kim, PhD Student, 2019&ndash;2023
- Danial Khan, Undergraduate Student (2022 SURF Recipient), Summer 2022
- Gundeep Singh, Undergraduate Student (2021 PURS Recipient), Summer 2019 and Fall 2021
- Ali Hamza Abidi Syed, Undergraduate Student (2021 PURS and SURF Recipient), Spring 2021 and Summer 2021
- Hossein Dabirian, Graduate Student (co-advised with Dr. Azencott), 2019&ndash;2021
- Yaseen Syed, Undergraduate Student (2021 PURS Recipient), Spring 2021
- Saeed Sarmadi, PhD Student (co-advised with Dr. Azencott), 2017&ndash;2020
- Haley Rosso, Undergraduate Student (2020 SURF Recipient), Summer 2020
- James L. Herring, Postdoctoral Researcher, 2018&ndash;2019
- Felix Huber, Visiting Graduate Student (co-advised with Dr. Mehl), 2018&ndash;2019
- Erin Gabrysch, Graduate Student (co-advised with Dr. Quaini), 2018&ndash;2019
- Brenda Gonzalez, Undergraduate Honors Student (2018 SURF Recipient), Summer 2018
- Orion Lowy, Undergraduate Student (co-advised with Dr. Bodmann), Summer 2018

</details>

### Support

This work is supported by the following awards:
- NSF Award [DMS-2145845](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2145845) (CAREER Award; 2022-2027)
- NSF Award [DMS-2430460](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2430460) (2025)
- NSF Award [DMS-2012825](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2012825) (2020-2023)
- NSF Award [DMS-2009923](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2009923) (2020-2023)
- NSF Award [DMS-1854853](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1854853) (2019-2022)
- Simons Foundation Award 586055 (2019)
- NVIDIA Corporation
- UH DOR GEAR Award 2025
