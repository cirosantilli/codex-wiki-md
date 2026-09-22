<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Values at the endpoint one do not affect any of the conclusions, since $\mathbb P(U=1)=0$. Set $b_n(1)=1$ to define each [random variable](../../../../../../random-variable-split.md) everywhere, and choose a [Borel measurable function](../../../../../../borel-measurable-function.md) agreeing with $f$ [almost everywhere](../../../../../../almost-everywhere.md) if necessary. These choices leave all integrals and almost-sure assertions unchanged.

Every [dyadic interval](../../../../../../dyadic-interval.md) at level $n+1$ lies in a [dyadic interval](../../../../../../dyadic-interval.md) at level $n$. Equivalently, $b_n(U)$ is a measurable function of $b_{n+1}(U)$, so $\mathcal F_n\subseteq\mathcal F_{n+1}$: these [sigma-algebras](../../../../../../sigma-algebra.md) form a [filtration](../../../../../../filtration-probability-theory.md). Since the [uniform distribution](../../../../../../continuous-uniform-distribution.md) of $U$ gives $\mathbb E|f(U)|=\int_0^1|f(u)|\,du<\infty$, the [conditional expectations](../../../../../../conditional-expectation.md) $X_n=\mathbb E[f(U)\mid\mathcal F_n]$ are integrable and adapted. The [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) gives

$$
\mathbb E[X_{n+1}\mid\mathcal F_n]
=\mathbb E[\mathbb E[f(U)\mid\mathcal F_{n+1}]\mid\mathcal F_n]
=\mathbb E[f(U)\mid\mathcal F_n]=X_n.
$$

Thus $(X_n)$ is a [martingale](../../../../../../martingale-split.md), and part (a) proves that it is [uniformly integrable](../../../../../../uniform-integrability.md).

For $I_{n,k}=[k2^{-n},(k+1)2^{-n})$, the [event](../../../../../../event.md) $\{U\in I_{n,k}\}$ is an [atom of a sigma-algebra](../../../../../../atom-of-a-sigma-algebra.md) $\mathcal F_n$, with [probability](../../../../../../probability.md) $2^{-n}$. The value of the [conditional expectation](../../../../../../conditional-expectation.md) there is therefore

$$
\frac{\mathbb E[f(U)\mathbf1_{\{U\in I_{n,k}\}}]}{\mathbb P(U\in I_{n,k})}
=2^n\int_{I_{n,k}}f(u)\,du.
$$

Consequently $\boxed{X_n=f_n(U)\text{ almost surely}.}$ This also shows directly that $\int_0^1|f_n|\leq\int_0^1|f|$.

By the [uniformly integrable martingale convergence theorem](../../../../../../uniformly-integrable-martingale-convergence-theorem.md), there is an integrable $Y$ such that $X_n\to Y$ [almost surely](../../../../../../almost-sure-convergence.md) and in the [L1 norm](../../../../../../l1-norm.md). To identify this limit, put $\mathcal F_\infty=\sigma(\bigcup_n\mathcal F_n)$. Since $0\leq U-b_n(U)<2^{-n}$ away from the harmless endpoint, $U=\lim_n b_n(U)$, and $U$ is $\mathcal F_\infty$-measurable. Conversely every $b_n(U)$ is a measurable function of $U$. Thus $\mathcal F_\infty=\sigma(U)$, and both $Y$ and $f(U)$ have $\mathcal F_\infty$-measurable versions.

For $A\in\mathcal F_m$, the defining property of [conditional expectation](../../../../../../conditional-expectation.md) gives $\mathbb E[X_n\mathbf1_A]=\mathbb E[f(U)\mathbf1_A]$ whenever $n\geq m$. Passing to the limit in the [L1 norm](../../../../../../l1-norm.md) yields

$$
\mathbb E[Y\mathbf1_A]=\mathbb E[f(U)\mathbf1_A].
$$

The increasing [union](../../../../../../set-union.md) $\bigcup_m\mathcal F_m$ is an [algebra of sets](../../../../../../algebra-of-sets.md) generating $\mathcal F_\infty$. The class of [events](../../../../../../event.md) for which this integral identity holds is a [Dynkin system](../../../../../../dynkin-system.md), so the [pi-lambda theorem](../../../../../../pi-lambda-theorem.md) extends the identity to every $A\in\mathcal F_\infty$. Since both [random variables](../../../../../../random-variable-split.md) are measurable there, uniqueness of [conditional expectation](../../../../../../conditional-expectation.md) gives $Y=f(U)$ [almost surely](../../../../../../almost-sure-convergence.md). We have proved that the [dyadic conditional averages recover integrable functions](../../../../../../dyadic-conditional-averages-recover-integrable-functions.md):

$$
\boxed{f_n(x)\longrightarrow f(x)\quad\text{for Lebesgue-almost every }x\in[0,1],}
$$

because a [probability](../../../../../../probability.md)-one assertion for $U$ is a full-[Lebesgue measure](../../../../../../lebesgue-measure.md) assertion for $x$. Likewise, the [uniform distribution](../../../../../../continuous-uniform-distribution.md) of $U$ turns [convergence in L1](../../../../../../convergence-in-l1.md) into

$$
\boxed{\int_0^1|f_n(u)-f(u)|\,du
=\mathbb E|X_n-f(U)|\longrightarrow0.}
$$

No pointwise continuity of $f$ is required.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
