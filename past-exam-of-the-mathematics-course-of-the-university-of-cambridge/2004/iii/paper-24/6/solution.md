<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Identify the [space of infinite subsets of the natural numbers](../../../../../space-of-infinite-subsets-of-the-natural-numbers.md) with their increasing enumerations, with the [ordinary topology on infinite subsets](../../../../../ordinary-topology-on-infinite-subsets.md) inherited from the discrete product $\omega^\omega$. This is the [sequence](../../../../../sequence.md) convention in the [Open Ramsey theorem](../../../../../open-ramsey-theorem.md). For a general infinite ground [set](../../../../../set-split.md), first choose a countably infinite [subset](../../../../../subset.md) and use its enumeration. The theorem cannot mean unrestricted [sequences](../../../../../sequence.md) with repetitions: the [clopen](../../../../../clopen-set.md) partition according as the first two entries agree or differ has both colours over every infinite ground [set](../../../../../set-split.md).

For a finite [finite stem](../../../../../finite-stem-of-an-infinite-subset.md) $s$ and an infinite tail $B$ above $\max s$, write

$$
[s,B]=\{s\cup X:X\in[B]^\omega\},
$$

where the enumeration of $s$ precedes the tail. Let $O$ be [open](../../../../../open-set.md). The tail $B$ accepts $s$ if $[s,B]\subseteq O$; it rejects $s$ if no infinite subtail accepts it. Both properties persist on infinite subtails, and any stem can be decided by thinning: choose an accepting subtail if one exists; otherwise the current tail already rejects it.

Use [deciding all finite stems by fusion](../../../../../deciding-all-finite-stems-by-fusion.md). At stage $n$, choose a new element $b_n$ from the current tail, then thin the remaining tail to decide each of the finitely many [subsets](../../../../../subset.md) of $\{b_0,\ldots,b_n\}$. First decide the empty stem as well. The final selected [set](../../../../../set-split.md) $B$ decides every finite stem from $B$, because all subsequent selections lie in the tail that decided that stem. If $B$ accepts the empty stem, $[B]^\omega\subseteq O$ and we are done.

Otherwise the empty stem is rejected. If a stem $s\subset B$ is rejected, only finitely many $a\in B$ above $\max s$ can have the tail $B/a$ accepting $s\cup\{a\}$. Indeed, if infinitely many such $a$ formed $D$, then every $X\in[D]^\omega$ starts with one of them and has its remaining tail in $B/a$. It follows that $[s,D]\subseteq O$, contradicting rejection of $s$. All other one-point extensions are rejected, since the first fusion has already decided them.

Build an infinite $C\subseteq B$ recursively. Maintain that every [subset](../../../../../subset.md) of the finite selected prefix is rejected. To select its next element, avoid the finite [union](../../../../../set-union.md) of the finitely many accepting-extension obstructions for these rejected stems. Such an element exists, and all the new stems remain rejected. Hence every finite stem from $C$ is rejected. If some $X\in[C]^\omega$ were in $O$, openness would supply a finite initial segment $s$ of $X$ whose entire ordinary cylinder is contained in $O$. The tail $C/\max s$ would accept $s$, a contradiction. Thus

$$
\boxed{[C]^\omega\cap O=\varnothing
\quad\text{or}\quad[B]^\omega\subseteq O.}
$$

In particular every [open](../../../../../open-set.md) payoff has an infinite [homogeneous set](../../../../../homogeneous-set-for-a-colouring.md). A finite partition into [open](../../../../../open-set.md) colour classes can be handled by successive application of this two-colour assertion.

For an arbitrary partition use [finite-symmetric-difference parity colouring](../../../../../finite-symmetric-difference-parity-colouring.md). On the infinite [subsets](../../../../../subset.md) of the ground [set](../../../../../set-split.md), declare $X\sim Y$ when $X\mathbin\triangle Y$ is finite, and choose a representative $R$ from each [equivalence class](../../../../../equivalence-class.md). Colour $X$ by

$$
c(X)=|X\mathbin\triangle R_{[X]}|\pmod2.
$$

For any infinite $H$, removing one member gives an infinite $H'$ in the same class and reverses the parity. Thus $H$ and $H'$ have opposite colours, so neither colour contains all infinite [subsets](../../../../../subset.md) of any infinite ground [set](../../../../../set-split.md). **This two-colouring has no infinite homogeneous [set](../../../../../set-split.md).** Representative selection uses [choice](../../../../../axiom-of-choice.md); the construction is deliberately unrestricted by topological regularity.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
