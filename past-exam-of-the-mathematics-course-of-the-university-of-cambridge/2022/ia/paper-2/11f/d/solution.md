<h1 id="11f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $E_j$ be the expected additional number of tosses when the current terminal run contains $j$ consecutive heads. Then $E_k=0$, and for $0\leq j<k$,

$$
E_j=1+pE_{j+1}+(1-p)E_0.
$$

For $0<p<1$, iterating this recurrence from $j=k-1$ down to $0$ gives

$$
E_0=\bigl(1+(1-p)E_0\bigr)
\frac{1-p^k}{1-p}.
$$

Solving,

$$
\boxed{
E_0=\frac{1-p^k}{(1-p)p^k}}.
$$

When $p=1$, the waiting time is deterministically $k$, which is also the continuous limit of this formula as $p\to1$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
