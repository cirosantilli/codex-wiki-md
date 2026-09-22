<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a [profinite abelian group](../../../../../profinite-abelian-group.md) $G$, its [Iwasawa algebra](../../../../../iwasawa-algebra.md) is the completed [group algebra](../../../../../group-algebra.md)

$$
\boxed{\Lambda(G)=\varprojlim_U\mathbb Z_p[G/U]=\varprojlim_{U,r}(\mathbb Z/p^r\mathbb Z)[G/U],}
$$

where $U$ runs over open [subgroups](../../../../../subgroup.md). The transition map sums the coefficients over the fibers of $G/V\to G/U$ when $V\subset U$. Consequently an element gives compatible values $\mu(gU)\in\mathbb Z_p$ on [cosets](../../../../../coset.md), equivalently a finitely additive $\mathbb Z_p$-valued [p-adic measure](../../../../../p-adic-measure.md) on the [clopen sets](../../../../../clopen-set.md) of $G$. Conversely these values specify every finite-quotient coefficient. Integration of a [continuous function](../../../../../continuous-function.md) with values in $\mathbb Z_p$ is obtained by uniform approximation by locally constant functions; the integrals converge because all measure values have $p$-adic absolute value at most $1$. Multiplication in the [Iwasawa algebra](../../../../../iwasawa-algebra.md) becomes [convolution of p-adic measures](../../../../../convolution-of-p-adic-measures.md). This is its [measure realization of an Iwasawa algebra](../../../../../measure-realization-of-an-iwasawa-algebra.md).

The [Mahler theorem](../../../../../mahler-s-theorem.md) states that each [continuous function](../../../../../continuous-function.md) $g:\mathbb Z_p\to\mathbb Z_p$ has the unique expansion converging in the sense of [uniform convergence](../../../../../uniform-convergence.md)

$$
g(x)=\sum_{n\geq0}b_n\binom{x}{n},\qquad b_n\in\mathbb Z_p,\quad b_n\longrightarrow0.
$$

Its [Mahler coefficients](../../../../../mahler-coefficient.md) are

$$
b_n=\Delta^ng(0)=\sum_{j=0}^{n}(-1)^{n-j}\binom njg(j),
$$

and $\|g\|_\infty=\sup_n|b_n|_p$. The same assertion holds for [continuous functions](../../../../../continuous-function.md) with values in $\mathbb Q_p$ with coefficients in $\mathbb Q_p$.

Given $f(T)=\sum_{n\geq0}a_nT^n\in R$, define the [bounded linear functional](../../../../../continuous-linear-functional.md)

$$
L_f(g)=\sum_{n\geq0}a_nb_n.
$$

The sum converges because $a_n\in\mathbb Z_p$ and $b_n\to0$. Its values on [indicator functions](../../../../../indicator-function.md) of [clopen sets](../../../../../clopen-set.md) give a [p-adic measure](../../../../../p-adic-measure.md), denoted $\lambda(f)$, with

$$
\int_{\mathbb Z_p}\binom{x}{n}\,d\lambda(f)=a_n.
$$

Conversely, a [p-adic measure](../../../../../p-adic-measure.md) determines these coefficients $a_n\in\mathbb Z_p$, and continuity allows termwise integration of every [Mahler expansion](../../../../../mahler-s-theorem.md). Thus the inverse is

$$
\mu\longmapsto\sum_{n\geq0}\left(\int\binom{x}{n}\,d\mu\right)T^n,
$$

which is the [Amice transform](../../../../../amice-transform.md). These two constructions are inverse, proving the **canonical bijection $\lambda:R\simeq\Lambda(\mathbb Z_p)$**. In fact it is an [isomorphism](../../../../../isomorphism.md) of [rings](../../../../../ring.md): the identity $\binom{x+y}{n}=\sum_{i+j=n}\binom{x}{i}\binom{y}{j}$ identifies [convolution of p-adic measures](../../../../../convolution-of-p-adic-measures.md) with multiplication of [formal power series](../../../../../formal-power-series.md). For example, $\lambda(1)=\delta_0$ and $\lambda(1+T)=\delta_1$, where $\delta_a$ is the [Dirac measure](../../../../../dirac-measure.md) at $a$.

For the moment identity, let $\left\{{k\atop n}\right\}$ denote a [Stirling number of the second kind](../../../../../stirling-numbers-of-the-second-kind.md). The finite [polynomial identity](../../../../../polynomial-identity.md)

$$
x^k=\sum_{n=0}^{k}n!\left\{{k\atop n}\right\}\binom{x}{n}
$$

gives $\int x^k\,d\lambda(f)=\sum_{n=0}^{k}a_n n!\left\{{k\atop n}\right\}$. On the other hand, $D=(1+T)d/dT$ satisfies $D^k(1+T)^x=x^k(1+T)^x$ for every nonnegative integer $x$. Expanding $(1+T)^x$ and evaluating at $T=0$ yields

$$
x^k=\sum_{n=0}^{k}\binom{x}{n}(D^kT^n)(0).
$$

Comparison in the [basis](../../../../../basis.md) of binomial [polynomials](../../../../../polynomial-split.md) gives $(D^kT^n)(0)=n!\left\{{k\atop n}\right\}$. Terms with $n>k$ have zero constant term after at most $k$ differentiations, so no infinite-series interchange is needed. Therefore

$$
\boxed{\int_{\mathbb Z_p}x^k\,d\lambda(f)=(D^kf)(0)\qquad(k\geq0).}
$$

The case $k=0$ says that the total mass is $f(0)$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
