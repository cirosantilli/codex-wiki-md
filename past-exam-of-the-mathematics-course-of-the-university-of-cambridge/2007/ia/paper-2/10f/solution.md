<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

The inverse [change of variables](../../../../../change-of-variables-formula.md) is $x=u$, $y=(v-u)/a$, with absolute [Jacobian determinant](../../../../../jacobian-determinant.md) $1/a$. Because the original [random variables](../../../../../random-variable-split.md) are independent, their joint density is $f(x)g(y)$. Thus the transformed [joint density](../../../../../joint-probability-density.md) is

$$
\boxed{f_{U,V}(u,v)=\begin{cases}
\dfrac1a f(u)g\left(\dfrac{v-u}a\right),&0\leq u\leq v,\\
0,&\text{otherwise}.
\end{cases}}
$$

The support is important: $X,Y\geq0$ implies $V\geq U\geq0$.

For independent [exponential random variables](../../../../../exponential-distribution.md) of rate $\lambda>0$ and $a=1/2$, this becomes $2\lambda^2e^{-2\lambda v+\lambda u}$ on $0\leq u\leq v$. Integrating out $u$ gives the density of the sum:

$$
\boxed{f_{X+Y/2}(v)=2\lambda^2e^{-2\lambda v}\int_0^v e^{\lambda u}\,du
=2\lambda(e^{-\lambda v}-e^{-2\lambda v}),\quad v\geq0.}
$$

It vanishes for $v<0$. On the other hand, the [cumulative distribution function](../../../../../cumulative-distribution-function.md) of the maximum is

$$
P(\max(X,Y)\leq v)=P(X\leq v)P(Y\leq v)=(1-e^{-\lambda v})^2\quad(v\geq0).
$$

Differentiating yields exactly the same density. **The maximum and $X+Y/2$ have the same distribution**, as described by [maximum of two exponentials as a scaled sum](../../../../../maximum-of-two-exponentials-as-a-scaled-sum.md); this does not assert that they are equal for the same pair of sampled values.

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
