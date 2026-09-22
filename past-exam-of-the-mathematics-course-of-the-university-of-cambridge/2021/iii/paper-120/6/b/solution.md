<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**No.** The complement of the [finite validity problem for first-order logic](../../../../../../finite-validity-problem-for-first-order-logic.md) is computably enumerable: enumerate finite structures in the sentence's finite vocabulary, evaluate the sentence in each, and halt when a countermodel appears.

For the converse hardness, fix a Turing machine $P$ and input $w$. Effectively construct a first-order sentence $\sigma_{P,w}$ describing a halting computation tableau. Use finite linearly ordered sets for times and tape positions, predicates for the state, head position, and tape symbol at each cell, and first-order local clauses saying that the first row is the initial configuration, consecutive rows obey the transition table, and the final row is halting. Then

$$
\sigma_{P,w}\text{ has a finite model}
\quad\Longleftrightarrow\quad
P\text{ halts on }w.
$$

A halting run gives its finite tableau; conversely, the linear orders and local transition clauses make every finite model decode to such a run.

If the sentences true in every finite structure were computably enumerable, then for each $(P,w)$ we could enumerate until either a finite model of $\sigma_{P,w}$ appeared or $\neg\sigma_{P,w}$ appeared among the finite validities. This would decide the halting problem. Equivalently, $\neg\sigma_{P,w}$ is finitely valid exactly when $P$ does not halt, so finite validity cannot be computably enumerable. This is [Trakhtenbrot theorem](../../../../../../trakhtenbrot-s-theorem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
