<h1 id="21i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the common bound be $M$. The derivative bound and the mean-value theorem give

$$
|f_n(x)-f_n(y)|\leq M|x-y|,
$$

so on every compact interval the sequence is uniformly bounded and equicontinuous. Apply the [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) first on $[-1,1]$, then to a subsequence on $[-2,2]$, and so on. The [diagonal subsequence for locally uniform convergence](../../../../../../diagonal-subsequence-for-locally-uniform-convergence.md) gives a strictly increasing $\phi$ such that $f_{\phi(n)}$ converges uniformly on every $[-R,R]$ to a function $f$. The limit is continuous and satisfies $|f(x)|\leq M$.

Global uniform convergence need not follow. Choose a nonzero continuously differentiable bump function $\psi$ supported in $[-1,1]$ and set

$$
f_n(x)=\psi(x-n).
$$

The functions and their derivatives have a common bound. On every fixed compact interval, $f_n$ is eventually zero, so every subsequence converges locally uniformly to $f=0$. Nevertheless

$$
\sup_{x\in\mathbb R}|f_n(x)-f(x)|
=\|\psi\|_\infty>0
$$

for every $n$. Thus the proposed global conclusion is false.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [21I](../../21i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
