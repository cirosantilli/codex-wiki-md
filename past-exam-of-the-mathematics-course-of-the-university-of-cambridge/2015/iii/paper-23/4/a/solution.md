<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [quantifier rank](../../../../../../quantifier-rank.md) measures maximum nesting depth:

$$
\begin{aligned}
\operatorname{qr}(\theta)&=0 &&\text{for atomic }\theta,\\
\operatorname{qr}(\neg\varphi)&=\operatorname{qr}(\varphi),\\
\operatorname{qr}(\varphi\wedge\psi)&=\operatorname{qr}(\varphi\vee\psi)=\max(\operatorname{qr}(\varphi),\operatorname{qr}(\psi)),\\
\operatorname{qr}(\exists x\varphi)&=\operatorname{qr}(\forall x\varphi)=1+\operatorname{qr}(\varphi).
\end{aligned}
$$

Two [first-order structures](../../../../../../first-order-structure.md) are [rank-n equivalent](../../../../../../rank-n-equivalence-of-structures.md) if they agree on all [first-order sentences](../../../../../../first-order-sentence.md) of [quantifier rank](../../../../../../quantifier-rank.md) at most $n$. For tuples one similarly compares all such formulas evaluated at the tuples.

In the $n$-round [Ehrenfeucht-Fraïssé game](../../../../../../ehrenfeucht-fraisse-game.md), player I, the Spoiler, chooses an element from either structure each round; player II, the Duplicator, chooses an element in the other. After $n$ rounds the corresponding chosen tuples must define a [partial isomorphism of structures](../../../../../../partial-embedding.md): all atomic formulas, including equality and the interpretations of constants, have matching truth values. Repetitions must be respected. Failure of this condition is a loss for II.

The precise finite-vocabulary [Ehrenfeucht-Fraïssé theorem](../../../../../../ehrenfeucht-fraisse-theorem.md) is: **for a finite relational language, allowing finitely many constants,**

$$
\boxed{\mathcal M\equiv_n\mathcal N\iff\text{II has a winning strategy in }G_n(\mathcal M,\mathcal N).}
$$

The tuple version has the same conclusion when the corresponding tuples are fixed before play. The implication from a winning strategy to rank equivalence holds for arbitrary languages, by induction on formulas. For the converse, finite relational vocabulary ensures only finitely many rank-bounded types in a fixed tuple of variables; their defining formulas let one transfer the type of the next move. Without a finiteness hypothesis, the converse for the full atomic-diagram game need not hold. This qualification matters in the next part.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
