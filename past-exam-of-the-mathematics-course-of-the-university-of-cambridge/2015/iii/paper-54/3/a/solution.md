<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [Komar integral of a five-dimensional Reissner--Nordstrom metric](../../../../../../komar-integral-of-a-five-dimensional-reissner-nordstrom-metric.md), use the one-form metrically dual to the stationary [Killing vector field](../../../../../../killing-vector-field.md): $k^\flat=-f(r)dt$. Its [exterior derivative](../../../../../../exterior-derivative.md) is $dk^\flat=f'(r)dt\wedge dr$. The stated orientation gives volume form

$$
\epsilon=-r^3\sin^2\chi\sin\theta\,dt\wedge dr\wedge d\chi\wedge d\theta\wedge d\phi.
$$

Because the squared norm of $dt\wedge dr$ is $g^{tt}g^{rr}=-1$, the defining wedge identity for the [Hodge star operator](../../../../../../hodge-star-operator.md) gives

$$
\star(dt\wedge dr)=r^3\sin^2\chi\sin\theta\,d\chi\wedge d\theta\wedge d\phi.
$$

Thus the [Komar integral](../../../../../../komar-charge.md) over the positively oriented angular three-sphere is

$$
\int_{S^3}\star dk^\flat=2\pi^2r^3f'(r),
$$

since the unit three-sphere has volume $2\pi^2$. Write $s=r_+^2+r_-^2$, $q=r_+^2r_-^2$. Then $f=1-s/r^2+q/r^4$ and $r^3f'=2s-4q/r^2$. With the normalization specified for the [Komar mass](../../../../../../komar-mass.md),

$$
\boxed{M=\frac\pi4(r_+^2+r_-^2).}
$$

The orientation makes this positive. The problem's coefficient $1/(16\pi)$ must be retained: it is not the usual dimension-adjusted five-dimensional ADM-normalized Komar coefficient. With that conventional normalization the ADM [mass](../../../../../../mass.md) would instead be $3\pi s/8$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
