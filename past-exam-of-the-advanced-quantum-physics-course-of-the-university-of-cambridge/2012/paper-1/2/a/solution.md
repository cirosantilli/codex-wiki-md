<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [WKB approximation](../../../../../wkb-approximation.md), also called JWKB, describes a short local de Broglie wavelength in a slowly varying [potential energy](../../../../../potential-energy.md). For $p(x)=\sqrt{2m[E-V(x)]}$ in a classically allowed region, its two local waves are

$$
\boxed{\psi(x)\simeq\frac1{\sqrt{p(x)}}\left[Ae^{(i/\hbar)\int^xp(s)ds}+Be^{-(i/\hbar)\int^xp(s)ds}\right].}
$$

The phase follows the classical [momentum](../../../../../momentum-split.md); its amplitude varies to conserve [probability current](../../../../../probability-current.md). In a forbidden region, putting $\kappa(x)=\sqrt{2m[V(x)-E]}$ gives $\psi\simeq\kappa^{-1/2}[Ce^{\int^x\kappa/\hbar}+De^{-\int^x\kappa/\hbar}]$, with boundary conditions selecting the physical combination.

The [WKB validity condition](../../../../../wkb-validity-condition.md) is $\hbar|p'|/p^2\ll1$, with the analogous condition on $\kappa$. It fails at a [turning point](../../../../../turning-point.md) where $E=V$. For a simple turning point, locally linearizing V yields an [Airy function](../../../../../airy-function.md); matching fixes the relative amplitudes and a $\pi/4$ phase. Two such turning points give the [two-turning-point WKB quantization condition](../../../../../two-turning-point-wkb-quantization-condition.md)

$$
\boxed{\int_{x_1}^{x_2}p(x)\,dx=\left(n+\tfrac12\right)\pi\hbar,\qquad n=0,1,\ldots.}
$$

For an opaque barrier, the [WKB tunnelling exponent](../../../../../wkb-tunnelling-exponent.md) instead gives

$$
\boxed{T\sim\exp\left[-\frac2\hbar\int_{x_1}^{x_2}\kappa(x)\,dx\right].}
$$

The factor two distinguishes probability from amplitude. Matching determines the prefactor; the exponential alone is not accurate near the barrier top. These formulas connect [bound state](../../../../../bound-state.md) [energy eigenvalues](../../../../../energy-eigenvalue-split.md) and [quantum tunnelling](../../../../../quantum-tunnelling.md) to classical actions. [§2.2, printed pp.37–49, semiclassical expansion, Airy matching and tunnelling](../../../../../topics-in-quantum-mechanics-by-david-tong.md)

<a id="2/a/image-an-illustrative-smooth-barrier-separates-two-oscillatory-wkb-regions-by-an-evanescent-interval"></a>
![](../../../../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2012/paper-1-aqp2012-wkb-barrier.png)

**[Figure 1](#2/a/image-an-illustrative-smooth-barrier-separates-two-oscillatory-wkb-regions-by-an-evanescent-interval). An illustrative smooth barrier separates two oscillatory WKB regions by an evanescent interval**. [Source](paper-1-aqp2012-wkb-barrier.py).

## ↑ Ancestors (14)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Physics course of the University of Cambridge](../../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
