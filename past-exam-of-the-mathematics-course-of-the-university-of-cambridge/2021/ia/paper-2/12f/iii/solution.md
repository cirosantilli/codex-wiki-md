<h1 id="12f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Because $f$ is continuous on the compact interval $[0,1]$, it is uniformly continuous and bounded; write $|f|\leq M$. Given $\epsilon>0$, choose $\delta>0$ such that

$$
|x-y|\leq\delta
\quad\Longrightarrow\quad
|f(x)-f(y)|\leq\epsilon.
$$

Then

$$
\begin{aligned}
|B_n(p)-f(p)|
&\leq
\mathbb E\left|f(S_n/n)-f(p)\right|\\
&\leq
\epsilon
+2M\mathbb P\left(\left|S_n/n-p\right|>\delta\right)\\
&\leq
\epsilon+\frac{M}{2n\delta^2}.
\end{aligned}
$$

The bound is independent of $p$. Taking the supremum, then $n\to\infty$, gives a limit superior at most $\epsilon$. Since $\epsilon$ is arbitrary,

$$
\boxed{
\sup_{p\in[0,1]}|f(p)-B_n(p)|\longrightarrow0}.
$$

This is the [Bernstein polynomial](../../../../../../bernstein-polynomial.md) proof of the [Weierstrass approximation theorem](../../../../../../weierstrass-approximation-theorem.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
