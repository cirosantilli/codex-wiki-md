<h1 id="17h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

We first derive the [Erdős-Gallai path edge bound](../../../../../../erdos-gallai-path-edge-bound.md) from part b. If an $n$-vertex graph has no path of length $t$, then

$$
e(G)\leq\frac{(t-1)n}{2}.
$$

Induct on $n$, component by component. A component with at most $t$ vertices satisfies the bound trivially. A larger connected component cannot have minimum degree at least $t/2$ by part b, so delete a vertex of degree less than $t/2$ and apply induction; the integer degree removed is at most $(t-1)/2$, which preserves the bound.

Now set

$$
n=(s-1)t+1
$$

and consider a red-blue colouring of $K_n$. If there is no red $K_s$, part a with $r=s-1$ gives

$$
e_R\leq\left(1-\frac1{s-1}\right)\frac{n^2}{2}.
$$

Consequently

$$
\begin{aligned}
e_B
&=\binom n2-e_R\\
&\geq\frac12\left(\frac{n^2}{s-1}-n\right)\\
&=\frac n2\left(t-1+\frac1{s-1}\right)
>\frac{(t-1)n}{2}.
\end{aligned}
$$

The path edge bound forces a blue $P_t$. Together with part c this proves the [clique-path Ramsey number](../../../../../../clique-path-ramsey-number.md)

$$
\boxed{r(K_s,P_t)=(s-1)t+1.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [17H](../../17h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
