<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the question's decreasing [survivor function](../../../../../survival-function.md) convention $F(t)=\mathbb P(T>t)$, rather than interpreting $F$ as a cumulative distribution function. An exact failure at $t$ contributes the mass $F(t-)-F(t)$. The [right censoring](../../../../../right-censoring.md) contribution is $F(3)$, and the [interval censoring](../../../../../interval-censoring.md) contribution is $F(2)-F(5)$. Under independent observations and a noninformative observation mechanism, the [empirical likelihood with mixed censoring](../../../../../empirical-likelihood-with-mixed-censoring.md), omitting observation-mechanism factors, is

$$
\boxed{L(F)=[F(1-)-F(1)][F(4-)-F(4)][F(6-)-F(6)]F(3)[F(2)-F(5)].}
$$

This is a likelihood over probability distributions with possible atoms; replacing the exact-event masses by a smooth density would be a different model.

Set $u=F(2)$ and $v=F(5)$. Monotonicity and $0\leq F\leq1$ give

$$
\begin{aligned}
F(1-)-F(1)&\leq1-u,\\
F(4-)-F(4)&\leq u-v,\\
F(6-)-F(6)&\leq v,\\
F(3)&\leq u.
\end{aligned}
$$

For instance, $F(4-)\leq F(2)=u$ while $F(4)\geq F(5)=v$, proving the second inequality. The interval-censoring factor already equals $u-v$. Multiplying gives the [monotonicity bound for a mixed-censoring likelihood](../../../../../monotonicity-bound-for-a-mixed-censoring-likelihood.md)

$$
L(F)\leq(1-u)(u-v)^2uv.
$$

For any $0<v<u<1$, this bound is attained by a distribution with masses $1-u$, $u-v$ and $v$ at $1$, $4$ and $6$ respectively. Its survivor function is one before the first mass, $u$ between the first and second, $v$ between the second and third, and zero thereafter.

The maximum likelihood is positive, because such a three-mass distribution has positive likelihood. At any maximizer all the above inequalities must therefore be equalities; otherwise replacing it by that three-mass distribution at the same $u,v$ would strictly improve its likelihood. Equality, together with monotonicity, yields

$$
\boxed{\begin{aligned}
\widehat F(1-)&=1,\\
\widehat F(4-)&=\widehat F(3)=\widehat F(2)=\widehat F(1),\\
\widehat F(6-)&=\widehat F(5)=\widehat F(4),\\
\widehat F(6)&=0.
\end{aligned}}
$$

Thus these relations are consequences of maximum likelihood, not assumptions about where an arbitrary distribution must put its mass.

The reduced [log-likelihood](../../../../../log-likelihood.md) is

$$
\ell(u,v)=\log(1-u)+2\log(u-v)+\log u+\log v,\qquad0<v<u<1.
$$

Its stationary equations are

$$
-\frac1{1-u}+\frac2{u-v}+\frac1u=0,\qquad-\frac2{u-v}+\frac1v=0.
$$

The second gives $u=3v$. Substituting in the first gives $-1/(1-u)+4/u=0$, hence

$$
\boxed{\widehat F(2)=\frac45,\qquad\widehat F(5)=\frac4{15}.}
$$

The reduced log-likelihood is [strictly concave](../../../../../strictly-concave-function.md): its second directional derivative in a nonzero direction $(a,b)$ is

$$
-\frac{a^2}{(1-u)^2}-\frac{2(a-b)^2}{(u-v)^2}-\frac{a^2}{u^2}-\frac{b^2}{v^2}<0.
$$

The likelihood vanishes on the boundary of the admissible triangle, so this stationary point is the unique maximum. The corresponding [nonparametric maximum-likelihood estimator](../../../../../nonparametric-maximum-likelihood-estimator.md) puts masses $1/5$, $8/15$ and $4/15$ at the three exact failure times.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
