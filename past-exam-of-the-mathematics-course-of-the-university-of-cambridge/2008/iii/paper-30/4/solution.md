<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the convention that level $k$ counts the $k$ nonzero shifts, hence an [arithmetic progression](../../../../../arithmetic-progression.md) of length $k+1$. The [SZ property](../../../../../sz-property.md) at level $k$ means that every measurable set $A$ of positive measure satisfies

$$
\boxed{\liminf_{N\to\infty}\frac1N\sum_{n=1}^N\mu\bigl(A\cap T^{-n}A\cap T^{-2n}A\cap\cdots\cap T^{-kn}A\bigr)>0.}
$$

This is the averaged multiple-recurrence property, stronger than merely finding one positive intersection. Shifting the indexing convention from $k+1$ terms to $k$ terms does not change the all-levels assertion. We work with probability [measure-preserving systems](../../../../../measure-preserving-system.md).

Here is the [Furstenberg correspondence principle](../../../../../furstenberg-correspondence-principle.md) construction proving the [Szemerédi theorem](../../../../../szemeredi-s-theorem.md). Let $D\subseteq\mathbb N$ have positive upper density $\delta=\limsup_N|D\cap\{1,\ldots,N\}|/N$. Put $z\in\{0,1\}^{\mathbb Z}$ equal to the indicator of $D$ on the positive coordinates and zero elsewhere, and let $S$ be the [left shift](../../../../../left-shift.md). The binary [full shift](../../../../../full-shift.md) $\Omega=\{0,1\}^{\mathbb Z}$ is a compact [metric space](../../../../../metric-space.md) in the [product topology](../../../../../product-topology.md), and $S$ is a [homeomorphism](../../../../../homeomorphism.md). Choose $N_i\to\infty$ attaining the upper density and define the [empirical measures](../../../../../empirical-measure.md)

$$
\mu_i=\frac1{N_i}\sum_{m=1}^{N_i}\delta_{S^mz}.
$$

We use the standard weak [compactness](../../../../../compact-space.md) fact that every sequence of [Borel probability measures](../../../../../borel-probability-measure.md) on a compact [metric space](../../../../../metric-space.md) has a weakly convergent subsequence, where weak convergence means convergence of integrals of continuous functions. Pass to a subsequence with limit $\mu$. For every continuous $F$, telescoping gives

$$
\int F\circ S\,d\mu_i-\int F\,d\mu_i
=\frac{F(S^{N_i+1}z)-F(Sz)}{N_i}\longrightarrow0.
$$

Passing to the limit proves $S_*\mu=\mu$. The [cylinder set](../../../../../cylinder-set.md) $A=\{w:w(0)=1\}$ is clopen, so its indicator is continuous and

$$
\mu(A)=\lim_i\mu_i(A)=\delta>0.
$$

If every [measure-preserving system](../../../../../measure-preserving-system.md) has the [SZ property](../../../../../sz-property.md) at level $k$, there is some $n\geq1$ for which $\mu(C_n)>0$, where $C_n=\bigcap_{j=0}^kS^{-jn}A$. This is also a clopen [cylinder set](../../../../../cylinder-set.md), so $\mu_i(C_n)\to\mu(C_n)>0$. For some sufficiently large $i$, at least one term of the empirical average is positive: $S^mz\in C_n$ for some $1\leq m\leq N_i$. Unwinding the coordinates gives

$$
z(m)=z(m+n)=\cdots=z(m+kn)=1.
$$

Therefore **$D$ contains an [arithmetic progression](../../../../../arithmetic-progression.md) of length $k+1$ with positive common difference**. Having the [SZ property](../../../../../sz-property.md) at every level gives the infinite-density form of the [Szemerédi theorem](../../../../../szemeredi-s-theorem.md).

The finite uniform form follows from the same argument. If, for fixed $\delta>0$ and $k$, arbitrarily large $N_i$ admitted sets $D_i\subseteq\{1,\ldots,N_i\}$ with $|D_i|\geq\delta N_i$ and no such [arithmetic progression](../../../../../arithmetic-progression.md), replace $z$ above by the indicator $z_i$ of $D_i$, extended by zero outside that interval. Their empirical measures still have an invariant weak limit with $\mu(A)\geq\delta$. For every fixed positive $n$, however, $\mu_i(C_n)=0$, since a point contributing to that cylinder would be an actual progression in $D_i$. Thus $\mu(C_n)=0$ for all positive $n$, contradicting the [SZ property](../../../../../sz-property.md). Consequently a sufficiently large $N$ depending only on $\delta,k$ forces the required progression.

A [compact measure-preserving system](../../../../../compact-measure-preserving-system.md) is one for which every observable $f\in L^2(\mu)$ has relatively compact forward orbit $\{U^nf:n\geq0\}$ under the [Koopman operator](../../../../../koopman-operator.md) $Uf=f\circ T$. Equivalently, each of these orbits is totally bounded in the global $L^2$ norm; [compactness](../../../../../compact-space.md) refers to observables, not just to the underlying topological space. For an invertible system it is usual to use all integer times. One may also define [compactness](../../../../../compact-space.md) by density of [almost periodic observables](../../../../../almost-periodic-observable.md): the two definitions coincide because $\|U^n(f-g)\|_2=\|f-g\|_2$, so a finite net for an approximating observable is a finite net, with slightly larger radius, for $f$.

To prove the [SZ property](../../../../../sz-property.md), fix $A$ with $a=\mu(A)>0$, put $f=\mathbf1_A$, and choose

$$
\varepsilon^2<\frac{a}{2\sum_{j=1}^kj^2}.
$$

[Compactness](../../../../../compact-space.md) gives a finite $\varepsilon$-net for its orbit with centers $U^{r_1}f,\ldots,U^{r_s}f$, where $r_i\geq0$. Let $M=\max_i r_i$. For every integer $n\geq M+1$, some center satisfies $\|U^nf-U^{r_i}f\|_2<\varepsilon$. Since $U$ is an [isometry](../../../../../isometry.md), cancellation gives

$$
\|U^{n-r_i}f-f\|_2<\varepsilon.
$$

Thus the return set $R=\{r\geq1:\|U^rf-f\|_2<\varepsilon\}$ meets every interval $\{n-M,\ldots,n\}$ for $n\geq M+1$. In particular, $R$ is a [syndetic set](../../../../../syndetic-set.md) with lower density at least $1/(M+1)$. This proves the needed [syndetic near returns of an almost periodic observable](../../../../../syndetic-near-returns-of-an-almost-periodic-observable.md) without any assumption of [ergodicity](../../../../../ergodicity.md).

For $r\in R$, telescoping and the [isometry](../../../../../isometry.md) property give

$$
\|U^{jr}f-f\|_2\leq\sum_{\ell=0}^{j-1}\|U^{\ell r}(U^rf-f)\|_2<j\varepsilon\qquad(1\leq j\leq k).
$$

As $f$ is an indicator, $\|U^{jr}f-f\|_2^2=\mu(A\mathbin\triangle T^{-jr}A)$. The [union bound](../../../../../boole-s-inequality.md) therefore gives

$$
\begin{aligned}
\mu\left(\bigcap_{j=0}^kT^{-jr}A\right)
&\geq a-\sum_{j=1}^k\mu(A\setminus T^{-jr}A)\\
&\geq a-\sum_{j=1}^k\|U^{jr}f-f\|_2^2
>a-\varepsilon^2\sum_{j=1}^kj^2>\frac a2.
\end{aligned}
$$

All other multiple-intersection measures are nonnegative. Averaging over the bounded-gap set $R$ yields

$$
\boxed{\liminf_{N\to\infty}\frac1N\sum_{r=1}^N\mu\left(\bigcap_{j=0}^kT^{-jr}A\right)\geq\frac{a}{2(M+1)}>0.}
$$

Thus **every compact [measure-preserving system](../../../../../measure-preserving-system.md) has the [SZ property](../../../../../sz-property.md) at every level**, including nonergodic systems and, under the forward-orbit definition, noninvertible transformations.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
