<h1 id="1/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The [volumetric flow rate](../../../../../volumetric-flow-rate.md) is the [integral](../../../../../integral-split.md) of axial [velocity](../../../../../velocity.md) over the cross-section:

$$
Q=\int_{-a}^{a}\int_{-b}^{b}w(x,y)\,dy\,dx.
$$

The [plane Poiseuille flow](../../../../../plane-poiseuille-flow.md) contribution is

$$
\int_{-a}^{a}\int_{-b}^{b}\frac{G}{2\mu}(b^2-y^2)\,dy\,dx
=\frac{4ab^3G}{3\mu}.
$$

For each correction [eigenfunction](../../../../../eigenfunction.md),

$$
\int_{-a}^{a}\frac{\cosh(k_nx)}{\cosh(k_na)}\,dx
=\frac{2\tanh(k_na)}{k_n},\qquad
\int_{-b}^{b}\cos(k_ny)\,dy=\frac{2(-1)^n}{k_n}.
$$

[Uniform convergence](../../../../../uniform-convergence.md) permits [termwise integration](../../../../../termwise-integration.md). Multiplying these two [integrals](../../../../../integral-split.md) by $A_n$ gives

$$
A_n\frac{4(-1)^n}{k_n^2}\tanh(k_na)
=-\frac{256Gb^4}{\mu\pi^5}
\frac{\tanh(k_na)}{(2n+1)^5}.
$$

Consequently

$$
\boxed{Q=\frac{4ab^3G}{3\mu}
-\frac{256b^4G}{\pi^5\mu}
\sum_{n=0}^{\infty}\frac{1}{(2n+1)^5}
\tanh\!\left(\frac{(2n+1)\pi a}{2b}\right).}
$$

Every summand in the subtracted quantity is positive. Thus **the side walls reduce the flux** below the infinite-width [plane Poiseuille flow](../../../../../plane-poiseuille-flow.md) prediction. Its dimensions are [volume](../../../../../volume.md) per unit [time](../../../../../time-in-physics.md), as required for a [volumetric flow rate](../../../../../volumetric-flow-rate.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the viscous flow course of the University of Oxford](../../../../split.md)
6. [Viscous flow course of the University of Oxford](../../../../../viscous-flow-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
