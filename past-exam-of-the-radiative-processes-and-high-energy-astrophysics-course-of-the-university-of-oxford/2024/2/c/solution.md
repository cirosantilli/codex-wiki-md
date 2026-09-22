<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\Delta=R-r\ll R$. The near-surface [mass density](../../../../density.md) and [mean free path](../../../../mean-free-path.md) from [a](../a.md) and [b](../b.md) are

$$
\rho\simeq\rho_c\frac\Delta R,\qquad
\ell\simeq\frac{LR}{\Delta}.
$$

A simple local escape estimate sets the remaining distance equal to the [mean free path](../../../../mean-free-path.md), $\ell\simeq\Delta$. It gives

$$
\boxed{\Delta R_{\rm esc,local}\simeq\sqrt{LR},\qquad
\frac{\Delta R_{\rm esc,local}}R\simeq\sqrt{\frac LR}.}
$$

For the [Sun](../../../../sun.md)'s parameters this is $\boxed{\Delta R_{\rm esc,local}\simeq1.94\,\mathrm{km},\quad\Delta R_{\rm esc,local}/R\simeq2.79\times10^{-6}}$.

A more precise operational definition uses the outward radial [optical depth](../../../../optical-depth.md). In this varying [mass density](../../../../density.md),

$$
\tau(r)=\int_r^R\frac{ds}{\ell(s)}
=\frac1{aL}\int_{ar}^{\pi}\frac{\sin x}{x}\,dx
\simeq\frac{\Delta^2}{2LR}.
$$

The chance of an outward radial [photon](../../../../photon.md) escaping without another scattering is $e^{-\tau}$. Thus the conventional $\tau=1$ last-scattering depth gives

$$
\boxed{\Delta R_{\rm esc,\tau=1}\simeq\sqrt{2LR}
\simeq2.75\,\mathrm{km},\qquad
\Delta R_{\rm esc,\tau=1}/R\simeq3.95\times10^{-6}.}
$$

There is no sharp escape surface: $\tau\ll1$ gives nearly free propagation, and oblique rays have different [optical depths](../../../../optical-depth.md). The local $\ell=\Delta$ estimate actually has $\tau\simeq1/2$ in this model, not $1$; the factor $\sqrt2$ is a convention-dependent order-one correction, not a discrepancy in the [Thomson cross-section](../../../../thomson-cross-section.md). Neither scattering criterion establishes a thermalization surface.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the radiative processes and high energy astrophysics course of the University of Oxford](../../../split.md)
5. [Radiative processes and high energy astrophysics course of the University of Oxford](../../../../radiative-processes-and-high-energy-astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
