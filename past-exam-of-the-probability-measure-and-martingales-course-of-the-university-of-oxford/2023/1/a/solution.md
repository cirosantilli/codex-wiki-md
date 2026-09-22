<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix $A\in\mathcal A_1$ and define

$$
\mathcal D_A=\{B\in\mathcal G_2:\mathbb P(A\cap B)=\mathbb P(A)\mathbb P(B)\}.
$$

This is a [Dynkin system](../../../../dynkin-system.md): it contains $\Omega$; taking [complements](../../../../complement-of-a-set.md) preserves the equality because $\mathbb P(A\cap B^c)=\mathbb P(A)-\mathbb P(A\cap B)$; and [countable additivity](../../../../countable-additivity.md) preserves it under disjoint [unions](../../../../set-union.md). The hypothesis says that $\mathcal D_A$ contains the [pi-system](../../../../pi-system.md) $\mathcal A_2$. Hence [Dynkin lemma](../../../../dynkin-lemma.md) gives $\mathcal D_A=\mathcal G_2$.

Now fix any $B\in\mathcal G_2$ and put

$$
\mathcal E_B=\{A\in\mathcal G_1:\mathbb P(A\cap B)=\mathbb P(A)\mathbb P(B)\}.
$$

The same [complement](../../../../complement-of-a-set.md) and disjoint-[union](../../../../set-union.md) calculations make this a [Dynkin system](../../../../dynkin-system.md). The first step shows that it contains $\mathcal A_1$, so [Dynkin lemma](../../../../dynkin-lemma.md) gives $\mathcal E_B=\mathcal G_1$. Thus

$$
\boxed{\mathbb P(A\cap B)=\mathbb P(A)\mathbb P(B)\quad(A\in\mathcal G_1,\ B\in\mathcal G_2).}
$$

This is precisely the definition of [independent sigma-algebras](../../../../independent-sigma-algebras.md), and proves [independence extended from generating pi-systems](../../../../independence-extended-from-generating-pi-systems.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../split.md)
5. [Probability, measure and martingales course of the University of Oxford](../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
