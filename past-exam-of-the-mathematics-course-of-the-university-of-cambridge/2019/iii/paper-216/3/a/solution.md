<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put

$$
S(x)=\sum_{i=1}^dp(x,i).
$$

The normalizing identity

$$
\int S(x)\nu(dx)
=\sum_i\int\nu(dx_{-i})\int\mu(dx_i\mid x_{-i})=d
$$

shows that

$$
\boxed{\pi(dx)=\frac{S(x)}d\nu(dx)}
$$

is a probability measure. If $x$ and $y$ differ only in coordinate $i$, the transition density from $x$ to $y$ is $p(x,i)\mu(y_i\mid x_{-i})/S(x)$. Therefore

$$
\begin{aligned}
\pi(x)K(x,y)
&=\frac1d\nu(x)p(x,i)\mu(y_i\mid x_{-i})\\
&=\frac1d\nu(x_{-i})
\mu(x_i\mid x_{-i})\mu(y_i\mid x_{-i}),
\end{aligned}
$$

which is symmetric in $x_i,y_i$. Thus detailed balance holds and the [Tempered Gibbs sampler](../../../../../../tempered-gibbs-sampler.md) is $\pi$-reversible.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
