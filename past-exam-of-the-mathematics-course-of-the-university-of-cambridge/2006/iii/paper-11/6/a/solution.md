<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Identify $[\mathbb N]^\omega$ with increasing infinite sequences, with the product topology. A [Ramsey set of infinite subsets](../../../../../../ramsey-set-of-infinite-subsets.md) $\mathcal A$ is one such that for every infinite $M$, some infinite $L\subseteq M$ satisfies $[L]^\omega\subseteq\mathcal A$ or $[L]^\omega\cap\mathcal A=\varnothing$. We prove this for open $\mathcal A$.

For a finite increasing stem $s$ and an infinite tail $B$ above it, say that $B$ accepts $s$ if every infinite $N\subseteq B$ has $s^\frown N\in\mathcal A$. Say that $B$ rejects $s$ if no infinite subset of $B$ accepts it. Either a tail has an accepting refinement, or it rejects. Both acceptance and rejection persist under passage to infinite subsets.

Starting with any infinite ground set $M$, use fusion to obtain an infinite $B$ deciding every finite subset of $B$: after selecting its first $n$ elements, refine the remaining tail successively to decide each of the finitely many subsets of that prefix. Then select the next element from the refined tail. The final tail beyond a decided stem is contained in the tail which decided it, so the decision survives. In particular $B$ decides the empty stem.

If $B$ accepts the empty stem, it is homogeneous inside $\mathcal A$. Otherwise it rejects. We thin it further so that every finite subset is rejected. The key observation is that if $B/s$ rejects $s$, there can be only finitely many $n\in B$ above $s$ for which $B/n$ accepts $s^\frown n$. If there were infinitely many, call their set $C$. For any infinite $N\subseteq C$, its first element $n$ and the accepting tail $B/n$ would imply $s^\frown N\in\mathcal A$. Thus $C$ would accept $s$, contradicting rejection.

Build $L$ inductively. Given a finite prefix whose subsets are all rejected, exclude the finitely many bad next elements for each of those subsets, and choose the next element outside their union. All new stems are decided by the first fusion and are not accepted, hence are rejected. This preserves the induction.

If an infinite $N\subseteq L$ belonged to the open set $\mathcal A$, some finite initial segment $s$ of $N$ would have every infinite extension above $\max s$ in $\mathcal A$. Then $B/s$ would accept $s$, contradicting the rejection just arranged. Therefore $[L]^\omega$ misses $\mathcal A$. We have proved

$$
\boxed{\text{every open subset of }[\mathbb N]^\omega\text{ is Ramsey}.}
$$

Taking complements gives the same result for closed subsets. The proof also works with any fixed finite stem, yielding the stronger finite-stem version when desired.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
