<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a bubble carrying momentum $p$, a [Feynman parameter](../../../../../../../feynman-parameter.md) and a shift of the loop momentum give, after Wick rotation and [cutoff regularization](../../../../../../../cutoff-regularization.md),

$$
B(p^2)=\int_0^1dx\int_{|\ell_E|<\Lambda}
\frac{d^4\ell_E}{(2\pi)^4}
\frac1{[\ell_E^2+F(p^2)]^2}
=\frac1{16\pi^2}\int_0^1dx
\left[\log\frac{\Lambda^2}{F(p^2)}-1\right]
+O(\Lambda^{-2}),
$$

where $F(p^2)=m^2-x(1-x)p^2-i0$. The [quantum effective action](../../../../../../../effective-action.md) therefore contains

$$
\Gamma_4(s,t,u)=\lambda+\delta_\lambda
-\frac{\lambda^2}{2}\{B(s)+B(t)+B(u)\}+O(\lambda^3).
$$

The [renormalization condition](../../../../../../../renormalization-condition.md) $\Gamma_4(M^2,M^2,M^2)=\lambda$ fixes

$$
\delta_\lambda=\frac{3\lambda^2}{2}B(M^2)+O(\lambda^3).
$$

Substitution cancels both the cutoff and the scheme-dependent constant and leaves

$$
\Gamma_4(s,t,u)=\lambda-\frac{\lambda^2}{32\pi^2}
\int_0^1dx\log\left[
\frac{F(M^2)^3}{F(s)F(t)F(u)}
\right]+O(\lambda^3),
$$

as required.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 304](../../../../paper-304-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
