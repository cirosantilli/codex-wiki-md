<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The initial values are $\beta_0(t)=1$ and $\beta_1(t)=0$. Repeatedly applying the [Brownian moment recursion](../../../../../../brownian-moment-recursion.md) to odd indices reduces them to $\beta_1$, so every odd moment vanishes. For even indices, if the formula holds at $2k-2$, then

$$
\begin{aligned}
\beta_{2k}(t)&=k(2k-1)\int_0^t\frac{(2k-2)!s^{k-1}}{2^{k-1}(k-1)!}\,ds\\
&=\frac{(2k)!}{2^kk!}t^k.
\end{aligned}
$$

The base case $k=0$ is $\beta_0=1$. Thus

$$
\boxed{\beta_{2k+1}(t)=0,\qquad\beta_{2k}(t)=\frac{(2k)!t^k}{2^kk!}\qquad(k\ge0).}
$$

Equivalently the even moments are $(2k-1)!!\,t^k$, the familiar Gaussian moment formula with [variance](../../../../../../variance-split.md) $t$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
