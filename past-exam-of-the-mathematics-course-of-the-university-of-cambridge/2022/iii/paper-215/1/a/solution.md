<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A stopping time $T$ is a [strong stationary time](../../../../../../strong-stationary-time.md) if

$$
\mathbb P_x(X_T=y,T=t)=\pi(y)\mathbb P_x(T=t)
$$

for every $x,y,t$. Thus $X_T\sim\pi$ and is independent of $T$. The [separation distance](../../../../../../separation-distance.md) is

$$
s(t)=\max_{x,y}\left\{1-\frac{P^t(x,y)}{\pi(y)}\right\}.
$$

For any strong stationary time,

$$
\begin{aligned}
P^t(x,y)
&\geq\mathbb P_x(X_t=y,T\leq t)\\
&=\sum_{j\leq t}\sum_z
\mathbb P_x(T=j,X_j=z)P^{t-j}(z,y)\\
&=\pi(y)\mathbb P_x(T\leq t).
\end{aligned}
$$

**Hence $1-P^t(x,y)/\pi(y)\leq\mathbb P_x(T>t)$, and maximizing proves the claim.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
