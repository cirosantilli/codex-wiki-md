<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Since $a$ is an [indicator function](../../../../../../indicator-function.md) of [density of a finite subset](../../../../../../density-of-a-finite-subset.md) $\alpha$, the [triangle inequality](../../../../../../triangle-inequality.md) gives $|\widehat a(r)|\leq\mathbb E_xa(x)=\alpha$ for every frequency. Also, [character orthogonality](../../../../../../character-orthogonality.md) and the [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md) give

$$
\sum_r|\widehat a(r)|^2=\mathbb E_x|a(x)|^2=\alpha.
$$

For completeness, the [character orthogonality](../../../../../../character-orthogonality.md) used here is

$$
\sum_{r\in\mathbb Z_n}\omega^{r(y-x)}=
\begin{cases}n,&x=y,\\0,&x\ne y,\end{cases}
$$

which follows by summing a finite [geometric series](../../../../../../geometric-series.md). Expanding the squared [Fourier coefficients on a finite abelian group](../../../../../../fourier-coefficient-on-a-finite-abelian-group.md) and using this identity proves the displayed [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md) directly.

Combining the uniform bound with that identity gives the **fourth-moment bound**

$$
\boxed{\|\widehat A\|_4^4=\sum_r|\widehat a(r)|^4\leq\alpha^2\sum_r|\widehat a(r)|^2=\alpha^3.}
$$

In particular, the [Lp norm](../../../../../../lp-norm.md) on the frequency side here is a sum, not a normalized average. This is the [fourth Fourier moment bound for an indicator function](../../../../../../fourth-fourier-moment-bound-for-an-indicator-function.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
