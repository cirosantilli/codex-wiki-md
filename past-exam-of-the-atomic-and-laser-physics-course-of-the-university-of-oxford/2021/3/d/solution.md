<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In [local thermodynamic equilibrium](../../../../local-thermodynamic-equilibrium.md), write the one-ray [radiative transfer equation](../../../../radiative-transfer-equation.md) as

$$
I_\nu+\kappa_\nu^{-1}\frac{dI_\nu}{dz}=B_\nu[T(z)].
$$

Large total [optical depth](../../../../optical-depth.md) removes the boundary contribution, but an additional local condition is essential: the [temperature](../../../../temperature-split.md) and [opacity](../../../../opacity.md) vary little over an absorption length $\kappa_\nu^{-1}$. Iterating once in that small gradient gives

$$
I_\nu=B_\nu-\frac1{\kappa_\nu}\frac{\partial B_\nu}{\partial T}\frac{dT}{dz}+\text{higher gradients}.
$$

The integrated [Planck function](../../../../planck-function.md) and its derivative are

$$
\int_0^\infty B_\nu\,d\nu=\frac{\sigma T^4}{\pi},\qquad
\int_0^\infty\frac{\partial B_\nu}{\partial T}\,d\nu=\frac{4\sigma T^3}{\pi}.
$$

Using the specified [Rosseland mean opacity](../../../../rosseland-mean-opacity.md), with $\kappa_R$ measured here in inverse length, the source's definition $F_{\rm ray}=\int I_\nu d\nu$ therefore gives

$$
\boxed{F_{\rm ray}(z)=\frac{\sigma T^4}{\pi}-\frac{4\sigma T^3}{\pi\kappa_R}\frac{dT}{dz}+\text{higher gradients}.}
$$

The printed leading term $\sigma T^4$ lacks a factor $1/\pi$ under that definition. An isothermal optically thick medium is a concrete counterexample: $I_\nu=B_\nu$ gives $F_{\rm ray}=\sigma T^4/\pi$ exactly, while the printed formula gives $\sigma T^4$.

A physical [radiative flux](../../../../radiative-flux.md) requires an angular integral. For direction cosine $\mu$, the same gradient expansion gives $I_\nu(\mu)=B_\nu-\mu\kappa_\nu^{-1}\partial_zB_\nu$. Integration over all directions gives the net [radiative diffusion](../../../../radiative-diffusion.md) flux

$$
\boxed{F_{\rm net}=2\pi\int_{-1}^1\mu\,d\mu\int_0^\infty I_\nu(\mu)\,d\nu
=-\frac{16\sigma T^3}{3\kappa_R}\frac{dT}{dz}.}
$$

The isotropic equilibrium contribution cancels between opposite directions. For comparison the outward-hemisphere flux alone is $\sigma T^4-8\sigma T^3(dT/dz)/(3\kappa_R)$ at this order. None of these consistent definitions yields the printed mixture of coefficients.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the atomic and laser physics course of the University of Oxford](../../../split.md)
5. [Atomic and laser physics course of the University of Oxford](../../../../atomic-and-laser-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
