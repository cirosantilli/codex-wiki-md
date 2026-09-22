<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $N=\lceil k^{1+\epsilon}\rceil$ and red-blue colour $K_N$. One colour class gives a graph $G$ with

$$
m=e(G)\ge\frac12\binom N2\ge c_0N^2.
$$

Apply part (a) with $s=d$, the common-neighbour target equal to $k$, and an integer

$$
t>\frac{(1+\epsilon)(d-1)}\epsilon.
$$

The first term in its hypothesis is at least $c_1^tN$. The error term satisfies

$$
\binom Nd\left(\frac{k}{N}\right)^t
\le N^d\left(\frac{k}{N}\right)^t
=N\,k^{(1+\epsilon)(d-1)-\epsilon t}
=o(N).
$$

Since $N/k=k^\epsilon\to\infty$, the difference is at least $k$ for all sufficiently large $k$, depending only on $d$ and $\epsilon$. Part (a) therefore gives a $(d,k)$-rich set of size at least $k$, and part (b) embeds $H$ in this colour. Hence

$$
\boxed{r(H)\le k^{1+\epsilon}}
$$

for sufficiently large $k$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
