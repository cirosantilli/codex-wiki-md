<h1 id="41d/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $C_j(\xi)$ denote the $j$th discrete cosine coefficient of $\xi_n=(-1)^nx_n$. For $0\leq k<N$,

$$
\begin{aligned}
C_{N-1-k}(\xi)
&=\sum_{n=0}^{N-1}(-1)^nx_n
\cos\left(\pi\left(n+\frac12\right)
-\frac{\pi}{N}\left(n+\frac12\right)(k+1)\right)\\
&=\sum_{n=0}^{N-1}x_n
\sin\left(\frac{\pi}{N}\left(n+\frac12\right)(k+1)\right)
=\widetilde Z_k.
\end{aligned}
$$

The identity uses $\cos(\pi(n+1/2)-u)=(-1)^n\sin u$. Sign-modulating the input and reversing the $N$ cosine-transform outputs each cost $O(N)$ operations, so part (c) gives the sine transform in $O(N\log N)$ multiplications.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [41D](../../41d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
