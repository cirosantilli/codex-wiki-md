<h1 id="2/c/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

List $\sigma(Y)\setminus Y=\{x_1,\ldots,x_m\}$ and put $Y_j=Y\cup\{x_1,\ldots,x_j\}$. Each $x_j\in\sigma(Y)$ also belongs to $\sigma(Y_{j-1})$ by (iii). Thus the definition of the [closure of a matroid](../../../../../../closure-of-a-matroid.md) gives $r(Y_j)=r(Y_{j-1})$ at every step. Iteration yields

$$
\boxed{r(\sigma(Y))=r(Y_m)=r(Y).}
$$

In particular, collecting all elements that individually fail to increase the [rank of a matroid](../../../../../../rank-of-a-matroid.md) does not create a collective increase.

## ↑ Ancestors (12)

1. [Vi](../vi.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Combinatorial optimisation](../../../../combinatorial-optimisation-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
