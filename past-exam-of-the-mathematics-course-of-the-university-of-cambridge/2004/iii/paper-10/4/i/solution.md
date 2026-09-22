<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume the compact space is nonempty. Write $M_n=\sup_K f_n$. Each $M_n$ is finite and attained, and the sequence decreases to a number $L\geq0$. Since $f\leq f_n$, certainly $\sup_K f\leq L$.

For any $t<L$, the sets $E_n=\{x\in K:f_n(x)\geq t\}$ are nonempty closed sets, and $E_{n+1}\subseteq E_n$. The [finite intersection property](../../../../../../finite-intersection-property.md) and compactness give a point in their intersection. At that point $f\geq t$, so $\sup_K f\geq t$. Let $t\uparrow L$; together with the reverse bound this proves

$$
\boxed{\sup_K f_n\longrightarrow\sup_K f.}
$$

This is [supremum convergence for decreasing continuous functions](../../../../../../supremum-convergence-for-decreasing-continuous-functions.md). The limit need not be continuous, so the conclusion does not assert the uniform convergence of the [Dini theorem](../../../../../../dini-s-theorem.md). It is precisely the interchange of these decreasing suprema and pointwise limit needed in the next part.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
