<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A multiset $\mathcal C$ of subsets of $[n]$ is a [uniform cover](../../../../../uniform-cover.md) of multiplicity $k$ when each coordinate occurs in exactly $k$ members. The [uniform covers theorem](../../../../../uniform-covers-theorem.md) states that every [Euclidean body](../../../../../euclidean-body.md) $S\subseteq\mathbb R^n$ satisfies

$$
\boxed{|S|^k\leq\prod_{A\in\mathcal C}|S_A|,}
$$

where $S_A$ is the [coordinate projection of a Euclidean body](../../../../../coordinate-projection-of-a-euclidean-body.md) onto the coordinates in $A$.

We prove it by induction on $n$. Split the cover into $\mathcal C^-$, whose members omit $n$, and $\mathcal C^+$, whose members contain $n$. Exactly $k$ members lie in $\mathcal C^+$. For a last-coordinate value $x$, let $S(x)\subseteq\mathbb R^{n-1}$ be the corresponding slice. Removing $n$ from the members of $\mathcal C^+$ and retaining the members of $\mathcal C^-$ gives a $k$-uniform cover of $[n-1]$. The inductive hypothesis and [Fubini's theorem](../../../../../fubini-s-theorem.md) give

$$
\begin{aligned}
|S|
&=\int |S(x)|\,dx\\
&\leq
\prod_{A\in\mathcal C^-}|S_A|^{1/k}
\int\prod_{A\in\mathcal C^+}|S(x)_{A\setminus\{n\}}|^{1/k}\,dx.
\end{aligned}
$$

Apply [Hölder's inequality](../../../../../holder-s-inequality.md) to the $k$ factors in the integral. Since

$$
\int|S(x)_{A\setminus\{n\}}|\,dx=|S_A|,
$$

we obtain $|S|\leq\prod_{A\in\mathcal C}|S_A|^{1/k}$, which is the result after taking the $k$th power. The one-dimensional base case is immediate.

The [Bollobas--Thomason box theorem](../../../../../box-theorem.md) states that for every body $S\subseteq\mathbb R^n$ there is an [axis-parallel box](../../../../../axis-parallel-box.md) $B$ such that

$$
\boxed{|B|=|S|\quad\text{and}\quad |B_A|\leq|S_A|\text{ for every }A\subseteq[n].}
$$

An [irreducible uniform cover](../../../../../irreducible-uniform-cover.md) cannot be decomposed into two smaller uniform covers. There are only finitely many such covers of $[n]$: encode a cover by its multiplicity vector in $\mathbb N^{2^n}$ and apply the [Dickson lemma](../../../../../dickson-s-lemma.md).

Choose a componentwise minimal positive array $(x_A)_{A\subseteq[n]}$ satisfying

$$
x_A\leq|S_A|,
\qquad
|S|^k\leq\prod_{A\in\mathcal C}x_A
$$

for every irreducible $k$-uniform cover $\mathcal C$, together with

$$
x_A\leq\prod_{i\in A}x_{\{i\}}.
$$

The actual projection volumes are feasible by the [uniform covers theorem](../../../../../uniform-covers-theorem.md), and finiteness gives a minimal array. Every uniform cover is a disjoint union of irreducible ones, so its cover inequality also holds for this array.

Minimality implies that, for each coordinate $i$, some tight uniform-cover inequality can be chosen whose cover contains the singleton $\{i\}$. Indeed, either such an inequality already blocks decreasing $x_{\{i\}}$, or a tight product inequality $x_A=\prod_{j\in A}x_{\{j\}}$ does; in the latter case take a tight cover containing $A$ and replace that occurrence of $A$ by its singleton coordinates. Let these tight covers be $\mathcal C_i$, of multiplicities $k_i$, and let $K=\sum_i k_i$. Their multiset union is a $K$-uniform cover. Removing one copy of every singleton leaves a $(K-1)$-uniform cover, so comparison of its cover inequality with the product of all the tight equalities yields

$$
\prod_{i=1}^n x_{\{i\}}\leq|S|.
$$

The singleton cover gives the reverse inequality, hence

$$
\prod_i x_{\{i\}}=|S|.
$$

For any $A\subseteq[n]$, the one-uniform cover consisting of $A$ and the singletons $\{i\}$ for $i\notin A$ now gives $x_A\geq\prod_{i\in A}x_{\{i\}}$. The defining product inequality gives the reverse bound. Thus all these quantities are equal. Taking the side lengths of $B$ to be $x_{\{1\}},\ldots,x_{\{n\}}$ proves the theorem.

Finally suppose that the proper body $S\subseteq\mathbb R^3$ satisfies

$$
|S|^2=|S_{12}|\,|S_{13}|\,|S_{23}|.
$$

This is equality in the three-dimensional [Loomis--Whitney inequality](../../../../../loomis-whitney-inequality.md). In its proof, equality must hold in both applications of [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). Their equality conditions force the three projection indicators to factor through one-dimensional measurable sets $E_1,E_2,E_3$, and force

$$
S=E_1\times E_2\times E_3
$$

up to a set of [Lebesgue measure](../../../../../lebesgue-measure.md) zero; this is [Equality in the three-dimensional Loomis--Whitney inequality](../../../../../equality-in-the-three-dimensional-loomis-whitney-inequality.md).

Because $S$ is connected, each one-coordinate projection is connected and hence is an interval. Because $S$ is a finite union of positive-volume [axis-parallel boxes](../../../../../axis-parallel-box.md), a proper difference between $S$ and the product of those three intervals would contain a positive-volume rectangular cell in a common finite subdivision. That would contradict equality up to measure zero. Consequently the equality is exact and

$$
\boxed{S\text{ is an axis-parallel box}.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 109](../../paper-109-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
