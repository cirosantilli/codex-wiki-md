<h1 id="41a/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fourier transformation in $m$ turns the recurrence into

$$
(1+\mu)\widehat u^{,n+1}
=2\mu\cos\theta\,\widehat u^{,n}
 +(1-\mu)\widehat u^{,n-1}.
$$

An amplification factor $z$ therefore satisfies

$$
(1+\mu)z^2-2\mu\cos\theta\,z-(1-\mu)=0.
$$

For $\mu>0$, the quadratic [Schur stability criterion](../../../../../../../schur-stability-criterion.md) gives

$$
|a_2|<1,qquad
1+a_1+a_2=\frac{2\mu(1-\cos\theta)}{1+\mu}\geq0,
$$



$$
1-a_1+a_2=\frac{2\mu(1+\cos\theta)}{1+\mu}\geq0,
$$

where $a_1=-2\mu\cos\theta/(1+\mu)$ and $a_2=(\mu-1)/(\mu+1)$. Thus both roots lie in the closed unit disk; roots on it at $\theta=0,\pi$ are simple. At $\mu=0$, the roots are $\pm1$. Parseval's identity then gives stability precisely for

$$
\boxed{\mu\geq0,}
$$

which is the full stated parameter range.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [41A](../../../41a.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
