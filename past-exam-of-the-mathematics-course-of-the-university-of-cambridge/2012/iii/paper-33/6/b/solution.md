<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $X_i$ be [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) with mean $0$ and [variance](../../../../../../variance-split.md) $\sigma^2\in(0,\infty)$, and put $S_0=0$, $S_k=\sum_{i=1}^kX_i$. Define the polygonal interpolation

$$
W_n(s)=\frac{S_{\lfloor ns\rfloor}+(ns-\lfloor ns\rfloor)X_{\lfloor ns\rfloor+1}}{\sigma\sqrt n}\qquad(0\leq s\leq1),
$$

with the endpoint $W_n(1)=S_n/(\sigma\sqrt n)$. The [Donsker invariance principle](../../../../../../donsker-s-theorem.md) states

$$
\boxed{W_n\ \Rightarrow\ B\quad\text{in }C([0,1])\text{ with the uniform topology},}
$$

where $B$ is standard one-dimensional [Brownian motion](../../../../../../brownian-motion-split.md) and the arrow denotes [weak convergence of probability measures](../../../../../../weak-convergence-of-probability-measures.md) on this path space. Equivalently, the step interpolation converges in the [Skorokhod space](../../../../../../skorokhod-space.md) with its $J_1$ topology. The continuous interpolation version is sufficient for the maximum in part (c).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
