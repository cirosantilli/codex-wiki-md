<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md), [independence](../../../../../../independent-random-variables.md) and the [Rademacher distribution](../../../../../../rademacher-distribution.md) give the [moment-generating function](../../../../../../moment-generating-function.md)

$$
\mathbb E e^{\theta S_n}=\prod_{i=1}^n\mathbb E e^{\theta X_i}=\left(\frac{e^\theta+e^{-\theta}}2\right)^n=(\cosh\theta)^n.
$$

The function $\theta^2/2-\log\cosh\theta$ is even; for $\theta\ge0$ its derivative is $\theta-\tanh\theta\ge0$, since the derivative of $\tanh\theta$ is at most one and $\tanh0=0$. Here $\cosh$ and $\tanh$ are the [hyperbolic cosine](../../../../../../hyperbolic-cosine.md) and [hyperbolic tangent](../../../../../../hyperbolic-tangent.md). Hence **the exponential-moment estimate** is

$$
\boxed{\mathbb E e^{\theta S_n}\le e^{n\theta^2/2}\quad(\theta\in\mathbb R).}
$$

The supplied [exponential maximal bound for a symmetric random walk](../../../../../../exponential-maximal-bound-for-a-symmetric-random-walk.md) now gives $\mathbb P(\max_{k\le n}S_k\ge t\sqrt n)\le\exp(-\theta t\sqrt n+n\theta^2/2)$. For $t>0$, choose $\theta=t/\sqrt n$; for $t=0$, use the elementary bound by one. Thus

$$
\boxed{\mathbb P(\max_{k\le n}S_k\ge t\sqrt n)\le e^{-t^2/2}\quad(t\ge0).}
$$

Fix $a>1$, choose $0<\delta<a^2-1$, and set $n_m=\lfloor(1+\delta)^m\rfloor$. For large $m$ these form an increasing sequence. Apply the preceding [exponential maximal bound for a symmetric random walk](../../../../../../exponential-maximal-bound-for-a-symmetric-random-walk.md) at $n_{m+1}$ with threshold $a\sqrt{2n_m\log\log n_m}$. The resulting probability is at most

$$
\exp\left(-a^2\frac{n_m}{n_{m+1}}\log\log n_m\right).
$$

We have $n_m/n_{m+1}\to(1+\delta)^{-1}$ and $\log\log n_m=\log m+O(1)$. Choose $b$ strictly between $1$ and $a^2/(1+\delta)$; the displayed probabilities are $O(m^{-b})$. By the [Borel-Cantelli first lemma](../../../../../../borel-cantelli-first-lemma.md), [almost surely](../../../../../../almost-sure-convergence.md), eventually $\max_{k\le n_{m+1}}S_k<a\sqrt{2n_m\log\log n_m}$. For every $n_m\le n\le n_{m+1}$, monotonicity of $n\log\log n$ for large $n$ therefore gives

$$
\frac{S_n}{\sqrt{2n\log\log n}}\le a.
$$

Intersect the probability-one events for $a=1+1/r$ to obtain **the [upper law of the iterated logarithm](../../../../../../upper-law-of-the-iterated-logarithm.md)**:

$$
\boxed{\mathbb P\left(\limsup_{n\to\infty}\frac{S_n}{\sqrt{2n\log\log n}}\le1\right)=1.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
