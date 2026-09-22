<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $A\in\mathcal C$ and $F:\mathcal C\to\mathbf{Set}$, the [Yoneda lemma](../../../../../../yoneda-lemma.md) gives a natural bijection

$$
\operatorname{Nat}(\mathcal C(A,-),F)\cong F(A),
\qquad \alpha\longmapsto\alpha_A(1_A).
$$

Assume $\mathcal C$ is small. For every pair $(A,x)$ with $x\in F(A)$, let $\alpha^{A,x}:\mathcal C(A,-)\to F$ be the corresponding natural transformation. Their copairing is

$$
\coprod_{A\in\mathcal C}\coprod_{x\in F(A)}
\mathcal C(A,-)\longrightarrow F.
$$

At an object $B$, the element $x\in F(B)$ is the image of $1_B$ in the summand indexed by $(B,x)$. The map is therefore pointwise surjective and hence an [epimorphism](../../../../../../epimorphism.md) in the [functor category](../../../../../../functor-category.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
