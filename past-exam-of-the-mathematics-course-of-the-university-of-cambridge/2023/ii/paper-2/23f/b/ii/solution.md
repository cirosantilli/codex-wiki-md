<h1 id="23f/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose a nonzero $f\in L^p(\mathbb R^n)\cap L^1(\mathbb R^n)$ whose transform belongs to $L^q$, for example a Gaussian by the [Fourier transform of a Gaussian](../../../../../../../fourier-transform-of-a-gaussian.md). For $\lambda>0$, set $f_\lambda(x)=f(\lambda x)$. The [scaling property of the Fourier transform](../../../../../../../scaling-property-of-the-fourier-transform.md) gives

$$
\|f_\lambda\|_p
=\lambda^{-n/p}\|f\|_p,
\qquad
\|\widehat {f_\lambda}\|_q
=\lambda^{-n(1-1/q)}\|\widehat f\|_q.
$$

The assumed estimate, applied for every $\lambda>0$, becomes

$$
\lambda^{-n(1-1/q)}\|\widehat f\|_q
\leq C\lambda^{-n/p}\|f\|_p.
$$

Since both norms are nonzero, this can hold as $\lambda$ tends both to zero and to infinity only if the powers agree. Thus the [scaling necessity for an Lp to Lq Fourier bound](../../../../../../../scaling-necessity-for-an-lp-to-lq-fourier-bound.md) yields

$$
1-\frac1q=\frac1p,
\qquad
\boxed{q=\frac p{p-1}}.
$$

**Hence $q$ is uniquely the [conjugate exponent](../../../../../../../conjugate-exponents.md) of $p$.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [23F](../../../23f.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
