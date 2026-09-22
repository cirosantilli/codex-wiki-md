<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [principal divisor criterion on an elliptic curve](../../../../../../principal-divisor-criterion-on-an-elliptic-curve.md) says that $D=\sum n_P(P)$ is principal exactly when $\deg D=0$ and $\sum[n_P]P=O$.

On $E':y^2+dy=x^3$, take

$$
T=(0,0),\qquad f=y.
$$

The line $y=0$ meets the cubic three times at $T$, while $y$ has a triple pole at the point at infinity. Hence

$$
\operatorname{div}(f)=3(T)-3(O_{E'}).
$$

With $g=u/v\in\mathbb Q(E)$, part (a) gives

$$
\phi^*f=\frac{u^3}{v^3}=g^3.
$$

Taking divisors and cancelling the factor three yields

$$
\operatorname{div}(g)=\phi^*((T)-(O_{E'})).
$$

Pullback on degree-zero divisor classes is the [dual isogeny](../../../../../../dual-isogeny.md), so the pulled-back class is represented by $\widehat\phi(T)$. It is principal, and therefore

$$
\boxed{T\in\ker\widehat\phi.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
