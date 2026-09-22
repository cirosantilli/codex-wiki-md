<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $M=AQ^{-1}A^T$. Since $\nabla h(z)=b-Mz$, [projected gradient ascent](../../../../../../../projected-gradient-descent.md) on the nonnegative orthant is

$$
\boxed{z_{k+1}=\bigl[z_k+\eta(b-Mz_k)\bigr]_+,}
$$

where the positive part is componentwise and one may take $0<\eta\leq1/L$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
