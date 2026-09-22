<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Cramér's theorem](../../../../../../cramer-s-theorem.md) states that the means of [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) in $\mathbb R^d$ satisfy a [large deviation principle](../../../../../../large-deviation-principle.md) at [large-deviation speed](../../../../../../large-deviation-speed.md) $n$, with [good rate function](../../../../../../good-rate-function.md) equal to the [Legendre-Fenchel transform](../../../../../../convex-conjugate.md) of their [cumulant-generating function](../../../../../../cumulant-generating-function.md), provided the [moment-generating function](../../../../../../moment-generating-function.md) is finite on a neighborhood of zero.

Here the [exponential distribution](../../../../../../exponential-distribution.md) has

$$
\Lambda(\theta)=\log\frac{\lambda}{\lambda-\theta}\quad(\theta<\lambda),
\qquad \Lambda(\theta)=\infty\quad(\theta\ge\lambda).
$$

For $x>0$, maximize $\theta x-\Lambda(\theta)$. Its [derivative](../../../../../../derivative.md) is $x-(\lambda-\theta)^{-1}$ and its second [derivative](../../../../../../derivative.md) is negative, so the maximizing parameter is $\theta_x=\lambda-x^{-1}$. Therefore the [rate function of an exponential sample mean](../../../../../../rate-function-of-an-exponential-sample-mean.md) is

$$
\boxed{I(x)=\begin{cases}\lambda x-1-\log(\lambda x),&x>0,\\+\infty,&x\le0.\end{cases}}
$$

For $x\le0$, letting $\theta\to-\infty$ in the same supremum gives $+\infty$, including the logarithmic divergence when $x=0$. The [moment-generating function](../../../../../../moment-generating-function.md) is finite near zero, so [Cramér's theorem](../../../../../../cramer-s-theorem.md) supplies the full [large deviation principle](../../../../../../large-deviation-principle.md).

The [rate function](../../../../../../rate-function.md) is nonnegative, with its unique minimum at $\mu=\lambda^{-1}$; $I''(x)=x^{-2}>0$. It tends to infinity both as $x\downarrow0$ and as $x\to\infty$. Its finite [sublevel sets](../../../../../../sublevel-set.md) are closed bounded intervals contained in $(0,\infty)$, hence [compact](../../../../../../compact-space.md). Thus it is a [good rate function](../../../../../../good-rate-function.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
