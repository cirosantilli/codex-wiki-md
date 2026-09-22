<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the large-$N$ [Gross–Pitaevskii equation](../../../../gross-pitaevskii-equation.md), dropping the [kinetic energy](../../../../kinetic-energy.md) gives $[\kappa r^2/2+gn(r)-\mu]\Psi(r)=0$. The physical nonnegative [Thomas–Fermi approximation for a condensate](../../../../thomas-fermi-approximation-for-a-condensate.md) is therefore

$$
\boxed{n(r)=\frac1g\left(\mu-\frac\kappa2r^2\right)_+,\qquad R=\sqrt{\frac{2\mu}\kappa},}
$$

where $(z)_+=\max(z,0)$ and $R$ is the cloud radius. Its [particle number](../../../../particle-number.md) is

$$
N=2\pi\int_0^Rr\,n(r)\,dr=\frac{2\pi}{g}\left(\frac{\mu R^2}2-\frac{\kappa R^4}8\right)
=\frac{\pi\mu^2}{g\kappa}.
$$

Thus the [two-dimensional Thomas–Fermi condensate](../../../../two-dimensional-thomas-fermi-condensate.md) obeys

$$
\boxed{\mu=\sqrt{\frac{Ng\kappa}\pi},\qquad R=\left(\frac{4Ng}{\pi\kappa}\right)^{1/4},\qquad n(0)=\frac\mu g.}
$$

Here $N=\int n\,d^2r$ is a total [particle number](../../../../particle-number.md). Keeping the exact pair count in the fixed-$N$ [Hartree product state](../../../../hartree-product-state.md) would replace $g$ by $g(1-1/N)$ in these formulas expressed in terms of $n=N|\phi|^2$.

The approximation is **best at the centre, $r=0$, and worst near the edge, $r=R$**. For example its omitted [quantum pressure of a condensate](../../../../quantum-pressure-of-a-condensate.md), evaluated on the interior profile, is

$$
Q(r)=-\frac{\hbar^2}{2m}\frac{\nabla^2\sqrt{n}}{\sqrt n}
=\frac{\hbar^2}{2mR^2}\frac{2-r^2/R^2}{(1-r^2/R^2)^2}.
$$

It is smallest at the centre and diverges at the artificial sharp edge. The central [healing length](../../../../healing-length.md) $\xi_0=\hbar/\sqrt{2m\mu}$ is much smaller than $R$ when $\mu\gg\hbar\omega$, since $R/\xi_0=2\mu/(\hbar\omega)$. This is the bulk validity condition; the full [Gross–Pitaevskii equation](../../../../gross-pitaevskii-equation.md) smooths the edge and gives a decaying tail outside $R$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the quantum matter course of the University of Oxford](../../../split.md)
5. [Quantum matter course of the University of Oxford](../../../../quantum-matter-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
