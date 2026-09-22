<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The **[Szemerédi theorem](../../../../../szemeredi-s-theorem.md)** says that for every integer $k\geq2$ and every $\delta>0$, there is $N_0(k,\delta)$ such that, for $N\geq N_0$, every $A\subseteq\{1,\ldots,N\}$ with $|A|\geq\delta N$ contains a nonconstant [arithmetic progression](../../../../../arithmetic-progression.md)

$$
\boxed{a,a+n,\ldots,a+(k-1)n\quad(n\geq1).}
$$

Equivalently, every subset of the positive integers with positive [upper asymptotic density](../../../../../upper-asymptotic-density.md) contains [arithmetic progressions](../../../../../arithmetic-progression.md) of every finite length. Length one is immediate.

The **[Furstenberg multiple recurrence theorem](../../../../../furstenberg-multiple-recurrence-theorem.md)** states that for every probability [measure-preserving system](../../../../../measure-preserving-system.md), every measurable $B$ with $\mu(B)>0$, and every integer $k\geq2$, there is $n\geq1$ with

$$
\boxed{\mu\left(\bigcap_{j=0}^{k-1}T^{-jn}B\right)>0.}
$$

Here $T^{-jn}B$ means a preimage, so invertibility is unnecessary. The [Furstenberg multiple recurrence theorem](../../../../../furstenberg-multiple-recurrence-theorem.md) also does not assume an [ergodic transformation](../../../../../ergodicity.md).

We prove the implication to the finite [Szemerédi theorem](../../../../../szemeredi-s-theorem.md) by constructing the [Furstenberg correspondence principle](../../../../../furstenberg-correspondence-principle.md) explicitly. Suppose, to the contrary, that for fixed $k$ and $\delta>0$ there are $N_\ell\to\infty$ and $A_\ell\subseteq\{1,\ldots,N_\ell\}$ with $|A_\ell|\geq\delta N_\ell$, but with no length-$k$ [arithmetic progression](../../../../../arithmetic-progression.md) of positive [common difference](../../../../../common-difference.md). In the binary [full shift](../../../../../full-shift.md) $\Omega=\{0,1\}^{\mathbb Z}$, encode $A_\ell$ as $x^{(\ell)}_j=\mathbf1_{A_\ell}(j)$, taking all coordinates outside $A_\ell$ to be zero. Let $S$ be the [left shift](../../../../../left-shift.md), $(S\omega)_j=\omega_{j+1}$, and set

$$
C=\{\omega:\omega_0=1\},\qquad
\nu_\ell=\frac1{N_\ell}\sum_{a=1}^{N_\ell}\delta_{S^ax^{(\ell)}}.
$$

The [cylinder set](../../../../../cylinder-set.md) $C$ is a [clopen set](../../../../../clopen-set.md), and $\nu_\ell(C)=|A_\ell|/N_\ell\geq\delta$. The binary [full shift](../../../../../full-shift.md) is a [compact metric space](../../../../../compact-metric-space.md), so [compactness of probability measures on a compact metric space](../../../../../compactness-of-probability-measures-on-a-compact-metric-space.md) gives a subsequence of these [empirical measures](../../../../../empirical-measure.md) with [weak convergence of probability measures](../../../../../weak-convergence-of-probability-measures.md) to a [Borel probability measure](../../../../../borel-probability-measure.md) $\nu$.

For every continuous $h$ on the [full shift](../../../../../full-shift.md),

$$
\int(h\circ S-h)\,d\nu_\ell
=\frac{h(S^{N_\ell+1}x^{(\ell)})-h(Sx^{(\ell)})}{N_\ell}\longrightarrow0.
$$

Passing to the weak limit shows that $\nu$ is an [invariant measure](../../../../../invariant-measure.md) for the continuous [left shift](../../../../../left-shift.md). Thus $(\Omega,\mathcal B,\nu,S)$ is a probability [measure-preserving system](../../../../../measure-preserving-system.md). Since the [indicator function](../../../../../indicator-function.md) of $C$ is continuous, $\nu(C)\geq\delta$.

Apply the [Furstenberg multiple recurrence theorem](../../../../../furstenberg-multiple-recurrence-theorem.md) to $C$. For some $n\geq1$, the [clopen set](../../../../../clopen-set.md)

$$
D=\bigcap_{j=0}^{k-1}S^{-jn}C
$$

has $\nu(D)>0$. Its continuous [indicator function](../../../../../indicator-function.md) gives $\nu_\ell(D)\to\nu(D)>0$. For large $\ell$, at least one $S^ax^{(\ell)}$ in the defining [empirical measure](../../../../../empirical-measure.md) therefore belongs to $D$. The choice of [left shift](../../../../../left-shift.md) implies

$$
x^{(\ell)}_{a+jn}=1\quad(0\leq j<k),
$$

so $a,a+n,\ldots,a+(k-1)n$ lies in $A_\ell$. This contradicts the assumed absence of [arithmetic progressions](../../../../../arithmetic-progression.md) and proves the finite [Szemerédi theorem](../../../../../szemeredi-s-theorem.md). Applying the finite [Szemerédi theorem](../../../../../szemeredi-s-theorem.md) on intervals where an infinite set has density bounded below proves the stated [upper asymptotic density](../../../../../upper-asymptotic-density.md) formulation.

For **[multiple recurrence for circle rotations](../../../../../multiple-recurrence-for-circle-rotations.md)**, write $\mathbb T=\mathbb R/\mathbb Z$ and $R_\alpha x=x+\alpha$, with normalized [Lebesgue measure](../../../../../lebesgue-measure.md) $m$, which is the [Haar measure](../../../../../haar-measure.md) of the [circle group](../../../../../circle-group.md). Fix a measurable $B\subseteq\mathbb T$ with $m(B)>0$ and $k\geq2$. If $\alpha$ is rational, there is $q\geq1$ with $R_\alpha^q$ the identity, and $n=q$ gives an intersection of measure $m(B)$.

For irrational $\alpha$, the [pigeonhole principle](../../../../../pigeonhole-principle.md) applied to $0,\alpha,\ldots,Q\alpha$ in $Q$ equal arcs gives $1\leq n\leq Q$ with $\|n\alpha\|_{\mathbb T}\leq1/Q$. In particular there are arbitrarily small nonzero returns to zero for the [irrational rotation of the circle](../../../../../irrational-rotation.md).

We also need [translation continuity in L1 on the circle](../../../../../translation-continuity-in-l1-on-the-circle.md). Given a measurable $B$, approximate its [indicator function](../../../../../indicator-function.md) in the [L1 norm](../../../../../l1-norm.md) by a continuous $g$ on the [circle group](../../../../../circle-group.md). Such approximation follows from regularity of [Lebesgue measure](../../../../../lebesgue-measure.md), or approximation by finite unions of intervals. Translation invariance and [uniform continuity](../../../../../uniform-continuity.md) give

$$
\|\mathbf1_B(\cdot+t)-\mathbf1_B\|_1
\leq2\|\mathbf1_B-g\|_1+\|g(\cdot+t)-g\|_1
\longrightarrow0\quad(t\to0),
$$

where the approximation error is first made arbitrarily small. Equivalently, $m(B\mathbin\triangle(B-t))\to0$.

Choose a return time $n\geq1$ so small modulo one that for each $1\leq j<k$,

$$
m(B\mathbin\triangle R_\alpha^{-jn}B)<\frac{m(B)}{2(k-1)}.
$$

This is possible because multiplication by each fixed $j$ is continuous on the [circle group](../../../../../circle-group.md) and [translation continuity in L1 on the circle](../../../../../translation-continuity-in-l1-on-the-circle.md) applies to the finitely many translates. The [union bound](../../../../../boole-s-inequality.md) now gives

$$
\boxed{m\left(\bigcap_{j=0}^{k-1}R_\alpha^{-jn}B\right)
\geq m(B)-\sum_{j=1}^{k-1}m(B\setminus R_\alpha^{-jn}B)
>\frac{m(B)}2>0.}
$$

This proves the [Furstenberg multiple recurrence theorem](../../../../../furstenberg-multiple-recurrence-theorem.md) for every circle rotation with its normalized [Lebesgue measure](../../../../../lebesgue-measure.md), including both rational and irrational angles.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 108](../../paper-108-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
