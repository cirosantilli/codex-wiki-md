<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $f(x)=\|x\|_\infty$. Away from ties and zero coordinates, its [gradient](../../../../../gradient.md) is $\nabla f(x)=\pm e_i$ for a maximizing coordinate $i$. Conditional on $X$, the random variable $\langle\nabla f(X),Y\rangle$ is centered Gaussian with variance at most one. The supplied [Gaussian concentration inequality](../../../../../gaussian-concentration-inequality.md) therefore gives

$$
\mathbb E\exp\{\lambda(f(X)-\mathbb Ef(X))\}
\leq\exp\left(\frac{\lambda^2\pi^2}{8}\right).
$$

A [Chernoff bound](../../../../../chernoff-bound.md), optimized at $\lambda=4u/\pi^2$, yields

$$
\mathbb P(f(X)>\mathbb Ef(X)+u)
\leq e^{-2u^2/\pi^2}.
$$

It remains to bound the mean. For $t>0$, Jensen's inequality and the Gaussian moment-generating function give

$$
\begin{aligned}
t\mathbb E\|X\|_\infty
&\leq\log\mathbb E e^{t\|X\|_\infty}\\
&\leq\log\sum_{i=1}^d
\mathbb E(e^{tX_i}+e^{-tX_i})\\
&\leq\log(2d)+\frac{t^2}{2}.
\end{aligned}
$$

Taking $t=\sqrt{2\log(2d)}$ gives $\mathbb E\|X\|_\infty\leq\sqrt{2\log(2d)}$. Consequently

$$
\boxed{
\mathbb P\left(\|X\|_\infty>
\sqrt{2\log(2d)}+u\right)
\leq e^{-2u^2/\pi^2}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
