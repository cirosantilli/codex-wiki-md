<h1 id="27k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $A_1\in\mathcal A_1$ and let

$$
\mathcal D_{A_1}
=\left\{B\in\mathcal F:
\mathbb P(A_1\cap B)=\mathbb P(A_1)\mathbb P(B)\right\}.
$$

This is a [Dynkin system](../../../../../../dynkin-system.md). It contains $\Omega$. If $B\in\mathcal D_{A_1}$, then

$$
\begin{aligned}
\mathbb P(A_1\cap B^c)
&=\mathbb P(A_1)-\mathbb P(A_1\cap B)\\
&=\mathbb P(A_1)(1-\mathbb P(B))\\
&=\mathbb P(A_1)\mathbb P(B^c),
\end{aligned}
$$

so it is closed under complements. Countable additivity gives closure under countable disjoint unions.

The hypothesis says $\mathcal A_2\subseteq\mathcal D_{A_1}$. Since $\mathcal A_2$ is a [pi-system](../../../../../../pi-system.md), [Dynkin lemma](../../../../../../dynkin-lemma.md) yields

$$
\sigma(\mathcal A_2)\subseteq\mathcal D_{A_1}.
$$

Thus the factorization holds for every $A_1\in\mathcal A_1$ and every $B\in\sigma(\mathcal A_2)$.

Now fix such a $B$ and define

$$
\mathcal E_B
=\left\{A\in\mathcal F:
\mathbb P(A\cap B)=\mathbb P(A)\mathbb P(B)\right\}.
$$

The identical calculation makes $\mathcal E_B$ a Dynkin system. The first step gives $\mathcal A_1\subseteq\mathcal E_B$, so a second application of Dynkin lemma gives

$$
\sigma(\mathcal A_1)\subseteq\mathcal E_B.
$$

Therefore the probability factorization holds for every

$$
A\in\sigma(\mathcal A_1),
\qquad B\in\sigma(\mathcal A_2),
$$

which is precisely independence of the two [sigma-algebras](../../../../../../independent-sigma-algebras.md). This is [independence extended from generating pi-systems](../../../../../../independence-extended-from-generating-pi-systems.md).

## ↑ Ancestors (11)

1. [B](../b.md)
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
