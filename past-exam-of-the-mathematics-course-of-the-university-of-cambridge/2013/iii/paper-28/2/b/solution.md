<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For [excess of loss reinsurance](../../../../../../excess-of-loss-reinsurance.md) the insurer pays each claim up to its retention level:

$$
\boxed{g(x)=\min(x,M),\qquad x-g(x)=(x-M)_+.}
$$

The cap applies separately to every claim. In particular the retained annual loss is $\sum_j\min(X_j,M)$, rather than a single cap on the annual total.

Let $F_i$ be the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) for the claim size on risk $i$, and put $\overline F_i=1-F_i$. The retained severity on that risk has the original [probability density function](../../../../../../probability-density-function.md) on $0<y<M$ and an [atom of a measure](../../../../../../atom-measure-theory.md) at $M$ of mass $\overline F_i(M)$. Thus $T_I$ has a [compound Poisson distribution](../../../../../../compound-poisson-distribution.md) with rate $\lambda_1+\lambda_2$ and the mixture of these capped severity laws. The mixture's mass at $M$ is $\sum_i\lambda_i\overline F_i(M)/(\lambda_1+\lambda_2)$.

For the [capped claim moments](../../../../../../capped-claim-moments.md), use the [tail integral formula for moments](../../../../../../tail-integral-formula-for-moments.md). Since $\mathbb P(\min(X_i,M)>x)=\overline F_i(x)$ for $0\le x<M$ and is zero for $x\ge M$,

$$
\mathbb E\min(X_i,M)=\int_0^M\overline F_i(x)\,dx,
\qquad
\mathbb E[\min(X_i,M)^2]=2\int_0^M x\overline F_i(x)\,dx.
$$

Substitution into the [compound Poisson distribution](../../../../../../compound-poisson-distribution.md) moment formulas gives

$$
\boxed{\mathbb ET_I=\sum_{i=1}^2\lambda_i\int_0^M\overline F_i(x)\,dx,\qquad
\operatorname{Var}(T_I)=2\sum_{i=1}^2\lambda_i\int_0^M x\overline F_i(x)\,dx.}
$$

Equivalently, the integrals are $\int_0^Mxf_i(x)\,dx+M\overline F_i(M)$ and $\int_0^Mx^2f_i(x)\,dx+M^2\overline F_i(M)$. The annual [variance](../../../../../../variance-split.md) uses the retained raw second moments; subtracting their squared means would omit the variation in the [Poisson distribution](../../../../../../poisson-distribution.md) count.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
