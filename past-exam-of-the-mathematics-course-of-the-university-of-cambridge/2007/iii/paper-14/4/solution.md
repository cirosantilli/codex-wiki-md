<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $[M]^\omega$ for the [set](../../../../../set-split.md) of all infinite [subsets](../../../../../subset.md) of $M$. A family $Y\subseteq[\mathbb N]^\omega$ is a [Ramsey family in the homogeneous-cone sense](../../../../../ramsey-family-in-the-homogeneous-cone-sense.md) if there is an infinite $M$ such that either $[M]^\omega\subseteq Y$ or $[M]^\omega\cap Y=\varnothing$. Thus membership in $Y$ is constant on an infinite homogeneous cone. We will prove the stronger version for open families: such a cone exists inside every prescribed infinite ground [set](../../../../../set-split.md), as in the definition of a [Ramsey set of infinite subsets](../../../../../ramsey-set-of-infinite-subsets.md).

The symbols in the question refer to the [ordinary topology on infinite subsets](../../../../../ordinary-topology-on-infinite-subsets.md) $\tau$ and the [Ellentuck topology](../../../../../ellentuck-topology.md) $*$. For a [finite set](../../../../../finite-set.md) $s$, let

$$
[s]=\{X\in[\mathbb N]^\omega:s\text{ is the initial segment of }X\}.
$$

These [sets](../../../../../set-split.md) form a [topological basis](../../../../../basis-of-a-topology.md) for $\tau$, equivalently the [subspace topology](../../../../../subspace-topology.md) inherited from the [product topology](../../../../../product-topology.md) on $\{0,1\}^{\mathbb N}$. For an infinite $A$ with $\max s<\min A$, the [sets](../../../../../set-split.md)

$$
[s,A]=\{s\cup B:B\in[A]^\omega\}
$$

form a [topological basis](../../../../../basis-of-a-topology.md) for $*$; take $\max\varnothing=0$. In particular $[s]=[s,\{n:n>\max s\}]$, so $*$ is finer than $\tau$.

For a non-Ramsey example use the [finite-symmetric-difference parity colouring](../../../../../finite-symmetric-difference-parity-colouring.md). On $[\mathbb N]^\omega$, define the [equivalence relation](../../../../../equivalence-relation.md) $X\sim Z$ if their [symmetric difference](../../../../../symmetric-difference.md) $X\mathbin\triangle Z$ is finite. By the [axiom of choice](../../../../../axiom-of-choice.md), select a representative $R$ in every [equivalence class](../../../../../equivalence-class.md). Give $X$ the colour

$$
c(X)=|X\mathbin\triangle R_X|\pmod2,
$$

where $R_X$ is its class representative. Deleting one point stays in the same class and toggles the parity. Thus for every infinite $M$, the [sets](../../../../../set-split.md) $M$ and $M\setminus\{\min M\}$ are both in $[M]^\omega$ but have opposite colours. Either [colour class](../../../../../colour-class.md), regarded as a family $Y$, is therefore **not Ramsey**.

Now let $U$ be $\tau$-open. We prove that for every infinite $A_0$ there is an infinite $C\subseteq A_0$ with $[C]^\omega\subseteq U$ or $[C]^\omega\cap U=\varnothing$. The proof uses [acceptance and rejection of finite stems](../../../../../acceptance-and-rejection-of-finite-stems.md), which we define explicitly. For a [finite stem](../../../../../finite-stem-of-an-infinite-subset.md) $s$ and an infinite tail $A$ above $\max s$, say that $A$ accepts $s$ if $[s,A]\subseteq U$, and rejects $s$ if no infinite [subset](../../../../../subset.md) of $A$ accepts $s$. Both properties persist on taking infinite [subsets](../../../../../subset.md). Every tail has an infinite [subset](../../../../../subset.md) that decides $s$: take an accepting [subset](../../../../../subset.md) if one exists, and otherwise it already rejects $s$.

First thin $A_0$ to decide the empty stem. Then construct $b_1<b_2<\cdots$ and nested infinite tails. At step $n$, choose $b_n$ from the current tail, discard its points at most $b_n$, and successively thin what remains to decide every stem $s\subseteq\{b_1,\ldots,b_n\}$. There are only finitely many such stems, so an infinite tail remains. Let $B=\{b_1,b_2,\ldots\}$ and write $B/s=\{b\in B:b>\max s\}$. For every finite $s\subseteq B$, the tail $B/s$ decides $s$, since it lies in the tail obtained at the stage when the largest point of $s$ was selected. The empty stem is also decided. This is [deciding all finite stems by fusion](../../../../../deciding-all-finite-stems-by-fusion.md).

If $B$ accepts the empty stem, then $[B]^\omega\subseteq U$, as required. Otherwise $B$ rejects it. We need the [finitely many accepting extensions of a rejected stem](../../../../../finitely-many-accepting-extensions-of-a-rejected-stem.md) observation. Suppose a tail $B/s$ rejects $s$. Only finitely many $a\in B/s$ can have $B/a$ accepting $s\cup\{a\}$. Indeed, if infinitely many such $a$ formed a [set](../../../../../set-split.md) $D$, every member of $[s,D]$ would have some first new point $a$ and all later points in $B/a$, hence would lie in $U$. This would make $D$ an accepting [subset](../../../../../subset.md) of $B/s$, contradicting rejection.

Choose $c_1<c_2<\cdots$ in $B$ recursively so that for every finite $s\subseteq\{c_1,\ldots,c_n\}$, the tail $B/s$ rejects $s$. The empty stem satisfies this initially. At the next step, each of the finitely many previous stems has only finitely many accepting one-point extensions by the observation. Choose $c_{n+1}$ larger than all previous points and outside all those finite exceptional [sets](../../../../../set-split.md). The first fusion ensured that the tail for every new stem decides it; since it does not accept it, it rejects it. This maintains the recursion.

Put $C=\{c_1,c_2,\ldots\}$. If some $X\in[C]^\omega$ belonged to $U$, ordinary openness would give a finite initial segment $s$ of $X$ with $[s]\subseteq U$. In particular $[s,C/s]\subseteq U$. But $C/s$ is an infinite [subset](../../../../../subset.md) of $B/s$, which rejects $s$, a contradiction. Hence $[C]^\omega\cap U=\varnothing$. We have proved

$$
\boxed{\text{Every }\tau\text{-open family is Ramsey, even inside every infinite ground set}.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
