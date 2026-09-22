<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $R=R(C_5)$ be the fixed [graph Ramsey number](../../../../../../graph-ramsey-number.md) of the five-cycle. Partition $\lfloor n/R\rfloor R$ vertices into $\lfloor n/R\rfloor$ disjoint blocks of size $R$. For any one block, the probability that $G(n,1/2)$ induces a complete graph is

$$
q=2^{-\binom R2}>0.
$$

These events are independent for the disjoint blocks. Therefore the probability that none of them induces $K_R$ is

$$
(1-q)^{\lfloor n/R\rfloor}\longrightarrow0.
$$

With probability tending to one, $G$ contains a copy of $K_R$. Every red-blue colouring of this copy contains a monochromatic $C_5$ by the definition of $R(C_5)$. Hence

$$
\boxed{\lim_{n\to\infty}\mathbb P(G\to C_5)=1.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
