<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

Let $x_{ij}\ge0$ be shipped amounts, with column sums equal to shop demand and row sums at most 15. Total demand is 42, so three units of warehouse stock need not be shipped. A feasible [transportation problem](../../../../../transportation-problem.md) allocation is

$$
\boxed{X=\begin{pmatrix}9&6&0&0&0\\0&0&12&3&0\\0&0&0&2&10\end{pmatrix}.}
$$

Its row sums are $(15,15,12)$ and its column sums meet every demand. The cost is $18+18+12+3+4+10=65$.

For a [transportation dual certificate with capacity inequalities](../../../../../transportation-dual-certificate-with-capacity-inequalities.md), choose warehouse potentials $u=(0,-1,0)$ and shop potentials $v=(2,3,2,2,1)$. They have $u_i\le0$ and $u_i+v_j\le c_{ij}$ for every cell. Any feasible allocation therefore has

$$
\sum_{ij}c_{ij}x_{ij}\ge\sum_i u_i\sum_jx_{ij}+\sum_jv_jd_j
\ge15\sum_i u_i+\sum_jv_jd_j
=-15+80=65.
$$

The second inequality has this direction because $u_i\le0$ and warehouse use is at most 15. **The exhibited allocation attains the lower bound, so the minimum cost is $\boxed{65}$.**

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
