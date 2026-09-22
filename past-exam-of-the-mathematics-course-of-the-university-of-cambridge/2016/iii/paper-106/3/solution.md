<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Radon-Nikodym theorem](../../../../../radon-nikodym-theorem.md) for positive measures says: if $\mu$ and $\nu$ are [sigma-finite measures](../../../../../sigma-finite-measure.md) on the same [measurable space](../../../../../measurable-space.md), and $\nu$ is absolutely continuous with respect to $\mu$, then there is a nonnegative [measurable function](../../../../../measurable-function.md) $g$, unique $\mu$-almost everywhere, such that

$$
\nu(E)=\int_E g\,d\mu\qquad(E\text{ measurable}).
$$

Here [sigma-finiteness](../../../../../sigma-finite-measure.md) means that the space is a countable union of measurable sets of finite measure; [absolute continuity of measures](../../../../../absolute-continuity-of-measures.md), written $\nu\ll\mu$, means that $\mu(E)=0$ implies $\nu(E)=0$. The function $g=d\nu/d\mu$ is the [Radon-Nikodym derivative](../../../../../radon-nikodym-derivative.md). For a finite signed or [complex measure](../../../../../complex-measure.md) $\nu$ of finite [total variation norm of a measure](../../../../../total-variation-norm-of-a-measure.md), absolutely continuous with respect to a sigma-finite $\mu$, the corresponding density belongs to $L^1(\mu)$. This follows by applying the positive theorem to the positive and negative parts of the real and imaginary parts of $\nu$.

**For every measure space and $1<p<\infty$, $(L^p)^*$ is isometrically $L^q$, where $1/p+1/q=1$.** We use the complex-linear pairing

$$
\Phi_g(h)=\int_\Omega hg\,d\mu.
$$

With the convention $\int h\overline g$, the same identification is conjugate-linear in $g$. By [Hölder's inequality](../../../../../holder-s-inequality.md), $\Phi_g$ is a [bounded linear functional](../../../../../continuous-linear-functional.md) with $\|\Phi_g\|\le\|g\|_q$. If $g\ne0$, set

$$
h=\frac{\overline g\,|g|^{q-2}}{\|g\|_q^{q-1}},
$$

interpreting the numerator as zero where $g=0$. The identity $(q-1)p=q$ gives $\|h\|_p=1$ and $\Phi_g(h)=\|g\|_q$. Thus

$$
\boxed{\|\Phi_g\|=\|g\|_q.}
$$

It remains to represent an arbitrary $\Phi\in(L^p)^*$, rather than merely produce functionals from $L^q$.

We prove [Lp duality on an arbitrary measure space](../../../../../lp-duality-on-an-arbitrary-measure-space.md) without imposing sigma-finiteness on $\mu$. Write $C=\|\Phi\|$. For every [measurable set](../../../../../measurable-set.md) $E$ with $\mu(E)<\infty$, define a [complex measure](../../../../../complex-measure.md) on $E$ by

$$
\nu_E(F)=\Phi(\mathbf1_F)\qquad(F\subseteq E\text{ measurable}).
$$

It is countably additive: for disjoint $F_j\subseteq E$, the partial sums of their [indicator functions](../../../../../indicator-function.md) tend in $L^p$ to $\mathbf1_{\bigcup F_j}$, because the measure of the omitted tail tends to zero. It is absolutely continuous with respect to $\mu|_E$, since [indicator functions](../../../../../indicator-function.md) of [null sets](../../../../../null-set.md) represent zero in $L^p$.

Its [total variation norm of a measure](../../../../../total-variation-norm-of-a-measure.md) is finite. For any finite measurable partition $E=\bigcup_j E_j$, choose scalars $c_j$ of modulus $1$ with $c_j\nu_E(E_j)=|\nu_E(E_j)|$. Then

$$
\sum_j|\nu_E(E_j)|=\Phi\left(\sum_jc_j\mathbf1_{E_j}\right)
\le C\left\|\sum_jc_j\mathbf1_{E_j}\right\|_p
=C\mu(E)^{1/p}.
$$

Taking the supremum over partitions gives the variation bound. Since $\mu|_E$ is finite, the [Radon-Nikodym theorem](../../../../../radon-nikodym-theorem.md) supplies $g_E\in L^1(E)$ with $\nu_E(F)=\int_F g_E\,d\mu$. By uniform approximation with [simple functions](../../../../../simple-function.md),

$$
\Phi(h)=\int_E hg_E\,d\mu
$$

for every bounded measurable $h$ supported in $E$.

To improve $g_E$ from $L^1$ to $L^q$, test with the bounded function

$$
h_N=\overline{g_E}|g_E|^{q-2}\mathbf1_{\{|g_E|\le N\}}\mathbf1_E.
$$

If $I_N=\int_{E\cap\{|g_E|\le N\}}|g_E|^q\,d\mu$, then

$$
I_N=\Phi(h_N)\le C\|h_N\|_p=C I_N^{1/p}.
$$

Thus $I_N^{1/q}\le C$ when $I_N>0$, and the same bound is trivial when it is zero. The [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) gives

$$
\int_E|g_E|^q\,d\mu\le C^q.
$$

If $E,F$ both have finite measure, the densities $g_E,g_F$ agree almost everywhere on $E\cap F$: their integrals over every measurable subset of the intersection equal the same functional value. This is uniqueness in the [Radon-Nikodym theorem](../../../../../radon-nikodym-theorem.md).

We now perform [support localization of an Lp functional](../../../../../support-localization-of-an-lp-functional.md). Set

$$
M=\sup_{\mu(E)<\infty}\int_E|g_E|^q\,d\mu\le C^q.
$$

Choose [finite-measure sets](../../../../../finite-measure-set.md) $E_n$ whose displayed integrals tend to $M$, and let $D_n=E_1\cup\cdots\cup E_n$, $S=\bigcup_nD_n$. If $M=0$, take $E_n=\varnothing$. Compatibility allows us to define a [measurable function](../../../../../measurable-function.md) $g$ on $S$ by taking $g_{D_n}$ on the disjoint [measurable sets](../../../../../measurable-set.md) $D_n\setminus D_{n-1}$, and put $g=0$ off $S$. It agrees almost everywhere with $g_{D_n}$ on every $D_n$. Moreover,

$$
\int_\Omega|g|^q\,d\mu=\lim_n\int_{D_n}|g_{D_n}|^q\,d\mu=M.
$$

Indeed each integral is at most $M$, and it is at least the integral over $E_n$, which tends to $M$.

For any [finite-measure set](../../../../../finite-measure-set.md) $F\subseteq\Omega\setminus S$, compatibility on the disjoint union $D_n\cup F$ gives

$$
\int_{D_n}|g_{D_n}|^q\,d\mu+\int_F|g_F|^q\,d\mu\le M.
$$

Letting $n\to\infty$ forces $g_F=0$ almost everywhere. For an arbitrary [finite-measure set](../../../../../finite-measure-set.md) $E$, compatibility on $E\cap D_n$ and the preceding conclusion on $E\setminus S$ show that $g_E=g$ almost everywhere on $E$. Consequently $\Phi(h)=\int hg\,d\mu$ for every [simple function](../../../../../simple-function.md) supported on a [finite-measure set](../../../../../finite-measure-set.md).

Those [simple functions](../../../../../simple-function.md) are dense in $L^p$ even for this arbitrary [measure space](../../../../../measure-space.md). To see the needed finite-support property, for $h\in L^p$ the sets $\{|h|>1/n\}$ have finite measure, bounded by $n^p\|h\|_p^p$. First truncate $h$ to such sets and to bounded values, then approximate by [simple functions](../../../../../simple-function.md); the discarded $L^p$ integral tends to zero. Continuity of $\Phi$ and [Hölder's inequality](../../../../../holder-s-inequality.md) therefore extend the representation to every $h\in L^p$.

We have constructed $g\in L^q$ with $\Phi=\Phi_g$, and the previously proved norm identity gives $\|g\|_q=\|\Phi\|$. It also proves uniqueness: if $\Phi_g=\Phi_{\widetilde g}$, then $\|g-\widetilde g\|_q=0$. This completes the isometric [duality of Lp spaces](../../../../../duality-of-lp-spaces.md).

**The dominated sequence actually converges to zero in norm, and hence weakly.** The assumptions give $|f_n|^p\le|f|^p\in L^1$ and $|f_n|^p\to0$ almost everywhere. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) yields

$$
\|f_n\|_p^p=\int|f_n|^p\,d\mu\longrightarrow0.
$$

For every $\Phi\in(L^p)^*$, $|\Phi(f_n)|\le\|\Phi\|\|f_n\|_p\to0$. Therefore

$$
\boxed{f_n\xrightarrow{w}0.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
