<h1 id="27k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Dynkin lemma](../../../../../../dynkin-lemma.md), also called the pi-lambda theorem, states that if a [Dynkin system](../../../../../../dynkin-system.md) $\mathcal D$ contains a [pi-system](../../../../../../pi-system.md) $\mathcal P$, then

$$
\sigma(\mathcal P)\subseteq\mathcal D.
$$

Let $\lambda(\mathcal P)$ be the smallest Dynkin system containing $\mathcal P$. It is enough to prove that $\lambda(\mathcal P)$ is a [sigma-algebra](../../../../../../sigma-algebra.md), because then

$$
\sigma(\mathcal P)\subseteq\lambda(\mathcal P)\subseteq\mathcal D.
$$

First fix $A\in\mathcal P$ and define

$$
\mathcal G_A
=\{B\in\lambda(\mathcal P):A\cap B\in\lambda(\mathcal P)\}.
$$

This is a Dynkin system. It contains $\Omega$ because $A\in\lambda(\mathcal P)$; closure under relative complements follows from

$$
A\cap B^c=A\setminus(A\cap B),
$$

and closure under disjoint unions follows by distributing $A\cap-$ over the union. Since $\mathcal P$ is closed under intersections, $\mathcal P\subseteq\mathcal G_A$. Minimality therefore gives

$$
\lambda(\mathcal P)\subseteq\mathcal G_A.
$$

Thus $A\cap B\in\lambda(\mathcal P)$ whenever $A\in\mathcal P$ and $B\in\lambda(\mathcal P)$.

Now fix $B\in\lambda(\mathcal P)$ and define

$$
\mathcal H_B
=\{A\in\lambda(\mathcal P):A\cap B\in\lambda(\mathcal P)\}.
$$

The same argument shows that $\mathcal H_B$ is a Dynkin system, and the preceding paragraph shows that it contains $\mathcal P$. Hence $\mathcal H_B=\lambda(\mathcal P)$. We have proved that $\lambda(\mathcal P)$ is itself a pi-system.

A Dynkin system that is also a pi-system is a sigma-algebra: it is closed under arbitrary finite intersections, hence finite unions by complements, and any countable union can be disjointified before using closure under disjoint unions. Therefore $\lambda(\mathcal P)=\sigma(\mathcal P)$, proving the lemma.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27K](../../27k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
