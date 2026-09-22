<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The Markov property gives $I(X_1;X_4\mid X_3)=I(X_2;X_4\mid X_3)=0$. The chain rule therefore yields

$$
I(X_1;X_3)-I(X_1;X_4)=I(X_1;X_3\mid X_4)
$$

and

$$
I(X_2;X_3)-I(X_2;X_4)=I(X_2;X_3\mid X_4).
$$

Conditional on $X_4$, the factorization of the chain still gives $X_1\to X_2\to X_3$. The [conditional data-processing inequality](../../../../../../conditional-data-processing-inequality.md) thus gives

$$
I(X_1;X_3\mid X_4)\leq I(X_2;X_3\mid X_4).
$$

Rearranging proves

$$
I(X_1;X_3)+I(X_2;X_4)
\leq I(X_1;X_4)+I(X_2;X_3).
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
