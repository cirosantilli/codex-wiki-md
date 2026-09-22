<h1 id="26k/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First, $\mathcal B\subseteq\mathcal C$ by taking $B=A$. If $A\in\mathcal C$, then

$$
A^c\mathbin\triangle B^c=A\mathbin\triangle B,
$$

so $\mathcal C$ is closed under complements. Now let $A_i\in\mathcal C$ and put $A=\bigcup_iA_i$. Because $\mu(X)<\infty$, [continuity from below of a measure](../../../../../../../continuity-from-below-of-a-measure.md) gives an $N$ such that

$$
\mu\left(A\setminus\bigcup_{i=1}^NA_i\right)<\frac\epsilon2.
$$

Choose $B_i\in\mathcal B$ with $\mu(A_i\triangle B_i)<\epsilon/(2N)$ and let $B=\bigcup_{i=1}^NB_i\in\mathcal B$. The union bound for symmetric differences gives

$$
\mu(A\triangle B)<\epsilon.
$$

Thus $\mathcal C$ is a sigma-algebra containing $\mathcal B$, and

$$
\boxed{\sigma(\mathcal B)\subseteq\mathcal C}.
$$

Finiteness is essential. Take $X=\mathbb N$ with counting measure and let $\mathcal B$ be the finite-cofinite [Boolean algebra of sets](../../../../../../../field-of-sets.md). Then $\sigma(\mathcal B)=\mathcal P(\mathbb N)$. For $\epsilon<1$, the condition $\mu(A\triangle B)<\epsilon$ forces $A=B$, so $\mathcal C=\mathcal B$. Any infinite coinfinite subset of $\mathbb N$ belongs to $\sigma(\mathcal B)$ but not to $\mathcal C$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [26K](../../../26k.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
