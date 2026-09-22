<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [sigma-algebra](../../../../../sigma-algebra.md) on $\Omega$ is a collection $\mathcal G\subseteq\mathcal P(\Omega)$ containing $\Omega$, closed under [complements](../../../../../complement-of-a-set.md) relative to $\Omega$, and closed under [countable unions](../../../../../countable-union.md). These properties also give closure under [countable intersections](../../../../../countable-intersection.md) by [De Morgan laws](../../../../../de-morgan-s-laws.md).

Let $\mathcal G=\bigcap_{r\in R}\mathcal F_r$. Every constituent [sigma-algebra](../../../../../sigma-algebra.md) contains $\Omega$, so $\Omega\in\mathcal G$. If $A\in\mathcal G$, its [complement](../../../../../complement-of-a-set.md) belongs to every $\mathcal F_r$, hence to $\mathcal G$. Likewise, if $A_j\in\mathcal G$ for all $j$, then $\bigcup_j A_j$ belongs to every $\mathcal F_r$. Thus $\mathcal G$ is a [sigma-algebra](../../../../../sigma-algebra.md). For an empty indexing set, the usual [intersection](../../../../../set-intersection.md) convention gives $\mathcal G=\mathcal P(\Omega)$, which is also a [sigma-algebra](../../../../../sigma-algebra.md).

A [union](../../../../../set-union.md) need not work. On $\Omega=\{1,2,3\}$ take

$$
\mathcal F_1=\{\varnothing,\Omega,\{1\},\{2,3\}\},\qquad
\mathcal F_2=\{\varnothing,\Omega,\{2\},\{1,3\}\}.
$$

Their [union](../../../../../set-union.md) contains $\{1\}$ and $\{2\}$ but not $\{1,2\}$, so it is not a [sigma-algebra](../../../../../sigma-algebra.md). Put $\mathcal A=\bigcup_r\mathcal F_r$ and let $\mathfrak C$ be the collection of all [sigma-algebras](../../../../../sigma-algebra.md) on $\Omega$ containing $\mathcal A$. This collection is nonempty because it contains the [power set](../../../../../power-set.md) $\mathcal P(\Omega)$. By the preceding [intersection](../../../../../set-intersection.md) argument,

$$
\boxed{\sigma(\mathcal A)=\bigcap_{\mathcal H\in\mathfrak C}\mathcal H}
$$

is a [sigma-algebra](../../../../../sigma-algebra.md) containing every $\mathcal F_r$, and it is contained in every other such [sigma-algebra](../../../../../sigma-algebra.md). This proves existence and minimality.

For the [independent random variables](../../../../../independent-random-variables.md), define the [tail sigma-algebra](../../../../../tail-sigma-algebra.md) by

$$
\mathcal T=\bigcap_{m\geq1}\sigma(X_m,X_{m+1},\ldots).
$$

Fix a [tail event](../../../../../tail-event.md) $A\in\mathcal T$. For each $m$, it belongs to $\sigma(X_{m+1},X_{m+2},\ldots)$, which is [independent](../../../../../independent-random-variables.md) of $\mathcal H_m=\sigma(X_1,\ldots,X_m)$. To justify independence of the generated [sigma-algebras](../../../../../sigma-algebra.md), first use independence of finite collections on cylinder [events](../../../../../event.md), then extend twice by the [pi-lambda theorem](../../../../../pi-lambda-theorem.md). In particular, $\mathbb P(A\cap C)=\mathbb P(A)\mathbb P(C)$ for every $C\in\mathcal H_m$ and every $m$.

The increasing [union](../../../../../set-union.md) $\bigcup_m\mathcal H_m$ is an [algebra of sets](../../../../../algebra-of-sets.md) generating $\mathcal H=\sigma(X_1,X_2,\ldots)$. The collection of $C\in\mathcal H$ satisfying this factorization is a [Dynkin system](../../../../../dynkin-system.md): it contains $\Omega$, is closed under [complements](../../../../../complement-of-a-set.md), and under countable disjoint [unions](../../../../../set-union.md). The [pi-lambda theorem](../../../../../pi-lambda-theorem.md) therefore extends the factorization to all $C\in\mathcal H$. Since $A\in\mathcal H$, taking $C=A$ gives $\mathbb P(A)=\mathbb P(A)^2$. Consequently,

$$
\boxed{\mathbb P(A)\in\{0,1\}\qquad(A\in\mathcal T).}
$$

This is the [Kolmogorov zero-one law](../../../../../kolmogorov-s-zero-one-law.md), proved here directly.

For each fixed $m$, write $S_n=S_{m-1}+\sum_{j=m}^nX_j$ for $n\geq m$, with $S_0=0$. The [random variable](../../../../../random-variable-split.md) $S_{m-1}$ is finite, so $S_{m-1}/\sqrt n\to0$. Adding a real sequence tending to zero changes neither the extended-real [limit inferior](../../../../../limit-inferior.md) nor the extended-real [limit superior](../../../../../limit-superior.md). Hence

$$
\liminf_n\frac{S_n}{\sqrt n}=\liminf_n\frac{\sum_{j=m}^nX_j}{\sqrt n},\qquad
\limsup_n\frac{S_n}{\sqrt n}=\limsup_n\frac{\sum_{j=m}^nX_j}{\sqrt n}.
$$

The quantities on the right are measurable with respect to $\sigma(X_m,X_{m+1},\ldots)$: write the [limit inferior](../../../../../limit-inferior.md) as $\sup_N\inf_{n\geq N}$ and the [limit superior](../../../../../limit-superior.md) as $\inf_N\sup_{n\geq N}$, using countable operations on [measurable functions](../../../../../measurable-function.md). Therefore both threshold [events](../../../../../event.md) belong to every such [sigma-algebra](../../../../../sigma-algebra.md), and hence are [tail events](../../../../../tail-event.md), for every real threshold, including when either limit is infinite.

**The final recurrence claim is false under the printed hypotheses.** For $c>0$, let $\varepsilon_j$ be independent signs with equal probabilities for $+1$ and $-1$, and set $X_j=c4^{-(j-1)}\varepsilon_j$. These [random variables](../../../../../random-variable-split.md) are independent, have [symmetric distributions](../../../../../symmetric-distribution.md), and obey $|X_j|\leq c$. Nevertheless, the [geometric series](../../../../../geometric-series.md) gives, on every sample path,

$$
|S_n|\geq c-\sum_{j=2}^n c4^{-(j-1)}\geq c-\frac c3=\frac{2c}{3}>\frac c2.
$$

Thus the proposed repeated-return [event](../../../../../event.md) has [probability](../../../../../probability.md) zero, even though none of the increments is degenerate. The [Kolmogorov zero-one law](../../../../../kolmogorov-s-zero-one-law.md) does not determine which of zero and one occurs.

An additional identical-distribution hypothesis makes the intended conclusion true. Here is a full proof of that qualified version, using the [oscillation of a bounded centered iid random walk](../../../../../oscillation-of-a-bounded-centered-iid-random-walk.md). Symmetry and integrability give $\mathbb E X_j=0$, so $S_n$ is a [martingale](../../../../../martingale-split.md) for its [natural filtration](../../../../../natural-filtration.md). If the common [probability distribution](../../../../../probability-distribution.md) is concentrated at zero, every $S_n$ is zero and the conclusion is immediate. Otherwise choose $\delta>0$ with $\mathbb P(|X_1|>\delta)>0$. The [Borel-Cantelli lemmas](../../../../../borel-cantelli-lemmas.md) then give $|X_n|>\delta$ infinitely often [almost surely](../../../../../almost-sure-convergence.md); thus $S_n$ cannot converge to a finite limit.

For $a>0$, let $T_a=\inf\{n:S_n\geq a\}$. Before $T_a$ the sum is below $a$, and at $T_a$ it is at most $a+c$. The [stopped martingale](../../../../../stopped-martingale.md) $a+c-S_{n\wedge T_a}$ is therefore nonnegative. A stopped integrable [martingale](../../../../../martingale-split.md) remains a [martingale](../../../../../martingale-split.md) at these bounded times, and a nonnegative [martingale](../../../../../martingale-split.md) converges finitely [almost surely](../../../../../almost-sure-convergence.md) by the [martingale convergence theorem](../../../../../martingale-convergence-theorem.md). On $\{T_a=\infty\}$ this would force $S_n$ to converge finitely, which has just been ruled out. Hence $T_a<\infty$ [almost surely](../../../../../almost-sure-convergence.md). Apply the same argument to $-S_n$ and take a countable intersection over positive integer $a$. It follows that

$$
\limsup_n S_n=+\infty,\qquad \liminf_n S_n=-\infty\quad\text{almost surely}.
$$

There are therefore arbitrarily late passages from above $c/2$ to below $-c/2$. A path with [bounded increments](../../../../../bounded-increments.md) of magnitude at most $c$ cannot make such a passage without visiting $[-c/2,c/2]$: jumping directly between its two open complementary half-lines would require an increment larger than $c$. There are infinitely many such visits. Thus **with the added identical-distribution hypothesis**, the intended answer is

$$
\boxed{\mathbb P\bigl(|S_n|\leq c/2\text{ infinitely often}\bigr)=1.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
