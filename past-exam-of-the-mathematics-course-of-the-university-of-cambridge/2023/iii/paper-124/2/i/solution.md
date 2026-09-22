<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a family $A\subseteq[n]^{(\leq l)}$, let $\langle A\rangle$ be the set of graphs on $[n]$ containing the clique on some $W\in A$. Write $A^*$ for its [Razborov closure](../../../../../../razborov-closure.md): whenever $W_1,\ldots,W_r\in A$ and

$$
W_i\cap W_j\subseteq W\qquad(i\ne j),
$$

with all sets of size at most $l$, closure adjoins $W$. A family is $r$-closed when $A=A^*$.

For closed $A,B$, define the lattice operations

$$
\langle A\rangle\square\langle B\rangle
=\langle A\cap B\rangle,
\qquad
\langle A\rangle\sqcup\langle B\rangle
=\langle(A\cup B)^*\rangle.
$$

The corresponding error sets are

$$
\delta_\cap(X,Y)=(X\cap Y)-(X\square Y),
\qquad
\delta_\cup(X,Y)=(X\sqcup Y)-(X\cup Y).
$$

The [Razborov gate-by-gate approximation lemma](../../../../../../razborov-gate-by-gate-approximation-lemma.md) says that if a monotone circuit of size at most $M$ computes a graph family $S$, and $\widetilde S$ is obtained by evaluating the same circuit with $\square,\sqcup$, then there are at most $M$ pairs of intermediate lattice elements such that

$$
S\setminus\widetilde S
\subseteq\bigcup\delta_\cap(X_j,Y_j),
\qquad
\widetilde S\setminus S
\subseteq\bigcup\delta_\cup(X_j,Y_j).
$$

This follows by induction through the circuit: an AND gate can introduce only a $\delta_\cap$ error, and an OR gate only a $\delta_\cup$ error.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
