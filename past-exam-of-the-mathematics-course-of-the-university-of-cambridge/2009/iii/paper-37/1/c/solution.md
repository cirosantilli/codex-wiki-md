<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [binomial distribution](../../../../../../binomial-distribution.md), $G_N(z)=(1-p+pz)^n$. Thus the [compound binomial distribution](../../../../../../compound-binomial-distribution.md) has

$$
\boxed{\kappa_S(t)=n\log\bigl(1-p+pM_{X_1}(t)\bigr).}
$$

Set $h(t)=1-p+pM_{X_1}(t)$. Since $h(0)=1$ and $h^{(j)}(0)=pm_j$, differentiating $n\log h$ three times gives

$$
\boxed{\kappa_{S,3}=n\bigl(pm_3-3p^2m_1m_2+2p^3m_1^3\bigr).}
$$

The first two [cumulants](../../../../../../cumulant.md), for comparison, are $npm_1$ and $n(pm_2-p^2m_1^2)$.

Choose deterministic claim sizes $X_i=d>0$. Then $S=dN$, so $m_j=d^j$ and

$$
\kappa_{S,3}=nd^3p(1-p)(1-2p).
$$

This is strictly negative for $p>1/2$ and $n\ge1$. A concrete **negative-skewness example** is $n=1$, $p=3/4$, $d=1$, for which

$$
\boxed{\kappa_{S,3}=-3/32<0.}
$$

There is no contradiction with positive claims: bounded Bernoulli-type totals can have more mass near their upper value and a longer left tail.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
