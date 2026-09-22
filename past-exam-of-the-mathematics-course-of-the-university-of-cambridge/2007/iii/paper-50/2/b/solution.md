<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $t=x^0-y^0$ and $\mathbf r=\mathbf x-\mathbf y$. By [time ordering](../../../../../../time-ordering.md) for a bosonic field,

$$
\Delta_F(x-y)=\theta(t)\int\frac{d^3p}{(2\pi)^3\,2E_p}e^{-iE_pt+i\mathbf p\cdot\mathbf r}
+\theta(-t)\int\frac{d^3p}{(2\pi)^3\,2E_p}e^{iE_pt-i\mathbf p\cdot\mathbf r}.
$$

Reverse $\mathbf p$ in the second integral. At fixed spatial momentum consider

$$
I(t)=\int_{-\infty}^{\infty}\frac{dp^0}{2\pi}\frac{i e^{-ip^0t}}{(p^0)^2-E_p^2+i0}.
$$

The [Feynman i-epsilon prescription](../../../../../../feynman-i-epsilon-prescription.md) places the poles at $+E_p-i0$ and $-E_p+i0$. For $t>0$, close in the lower half-plane, clockwise. The positive-energy residue and the orientation give $e^{-iE_pt}/(2E_p)$. For $t<0$, close counterclockwise in the upper half-plane; the negative pole has derivative denominator $-2E_p$, and its residue gives $e^{iE_pt}/(2E_p)$. Thus $I(t)=e^{-iE_p|t|}/(2E_p)$, reproducing the time-ordered mode expression. We obtain

$$
\boxed{\Delta_F(x-y)=\int\frac{d^4p}{(2\pi)^4}\frac{i e^{-ip\cdot(x-y)}}{p^2-\mu^2+i0}.}
$$

This is a distributional boundary value, not an absolutely convergent Fourier integral. As an independent normalization check, $I'(0^+)-I'(0^-)=-i$, so $(\Box+\mu^2)\Delta_F=-i\delta^{(4)}$; the numerator is $i$ with the question's definition of the propagator.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
