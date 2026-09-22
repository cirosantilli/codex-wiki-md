<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Group the edge indicators into $n-1$ independent blocks

$$
B_i=(X_{ij}:j>i),
\qquad1\leq i<n.
$$

All edges in one block share vertex $i$. Replacing the entire block can change the maximum matching number by at most one: after deleting the at most one matched edge incident to $i$, a matching from either graph remains valid in the other. Applying [McDiarmid inequality](../../../../../../mcdiarmid-s-inequality.md) to these $n-1$ blocks gives

$$
\boxed{\mathbb P(f(G)-\mathbb Ef(G)\geq t),
\quad
\mathbb P(f(G)-\mathbb Ef(G)\leq-t)
\leq\exp\!\left(-\frac{2t^2}{n-1}\right).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
