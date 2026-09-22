# Standard linear solid model

↑ **Parent:** [Viscoelasticity](viscoelasticity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Standard_linear_solid_model)

A [standard linear solid model](standard-linear-solid-model.md) has a finite instantaneous stiffness, a nonzero long-time stiffness and one exponential stress-relaxation mode. A [Kelvin-Voigt model](kelvin-voigt-model.md) with spring $G_0$ and viscosity $\eta$ in series with spring $G_1$ gives

$$
\eta\dot\sigma+(G_0+G_1)\sigma=G_1\eta\dot\epsilon+G_0G_1\epsilon,
\qquad G_L=\frac{G_0G_1}{G_0+G_1},\quad G_H=G_1,\quad\tau=\frac\eta{G_0+G_1}.
$$

These expressions follow by adding series strains under common [stress](stress.md). Its [storage modulus](storage-modulus.md) is $G_L+(G_H-G_L)x^2/(1+x^2)$ and its [loss modulus](loss-modulus.md) is $(G_H-G_L)x/(1+x^2)$ for $x=\omega\tau$. Its [relaxation modulus](relaxation-modulus.md) is $G(t)=G_L+(G_H-G_L)e^{-t/\tau}$, while its [creep compliance](creep-compliance.md) is $J(t)=G_1^{-1}+G_0^{-1}(1-e^{-G_0t/\eta})$. Thus creep retardation and stress-relaxation times differ. This solid has bounded creep and cannot represent terminal fluid flow.

**Table of contents**

- [Series spring and Voigt-branch creep](series-spring-and-voigt-branch-creep.md)
  - [Recovery after a finite-duration stress load](recovery-after-a-finite-duration-stress-load.md)
- [Peak frequencies in a standard linear solid](peak-frequencies-in-a-standard-linear-solid.md)

## ↑ Ancestors (7)

1. [Viscoelasticity](viscoelasticity.md)
2. [Non-Newtonian fluid](non-newtonian-fluid.md)
3. [Rheology](rheology-split.md)
4. [Fluid mechanics](fluid-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Burgers material](burgers-material.md)
- [Solution](past-exam-of-the-materials-science-course-of-the-university-of-cambridge/2015/paper-1/5/e/i/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2017/2/c/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2018/section-b/b3/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2021/section-b/4/d/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2021/section-b/4/e/solution.md)
- [Peak frequencies in a standard linear solid](peak-frequencies-in-a-standard-linear-solid.md)
- [Recovery after a finite-duration stress load](recovery-after-a-finite-duration-stress-load.md)
- [Retardation time (viscoelasticity)](retardation-time-viscoelasticity.md)
- [Standard linear solid model](standard-linear-solid-model.md)
