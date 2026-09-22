<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Both sequents follow directly from the introduction and elimination rules of the [implication-free fragment of intuitionistic propositional logic](../../../../../../implication-free-fragment-of-intuitionistic-propositional-logic.md). From a proof of $\phi\wedge(\psi\vee\chi)$, eliminate the conjunction to obtain $\phi$ and $\psi\vee\chi$. Eliminate the disjunction: in the $\psi$ branch introduce $\phi\wedge\psi$ and then the left disjunct; in the $\chi$ branch introduce $\phi\wedge\chi$ and then the right disjunct. This yields

$$
\phi\wedge(\psi\vee\chi)
\vdash
(\phi\wedge\psi)\vee(\phi\wedge\chi).
$$

Conversely, eliminate the outer disjunction. From $\phi\wedge\psi$, obtain $\phi$ and introduce the left side of $\psi\vee\chi$; from $\phi\wedge\chi$, obtain $\phi$ and introduce its right side. In either branch, conjunction introduction produces $\phi\wedge(\psi\vee\chi)$. Hence

$$
(\phi\wedge\psi)\vee(\phi\wedge\chi)
\vdash
\phi\wedge(\psi\vee\chi).
$$

This is the proof-theoretic form of the [distributive law for lattices](../../../../../../distributive-law-for-lattices.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
