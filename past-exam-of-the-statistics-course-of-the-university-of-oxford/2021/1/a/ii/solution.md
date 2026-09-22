<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Using the [raw moments](../../../../../raw-moment.md) from part (i), the [variance](../../../../../variance-split.md) of one observation is

$$
\operatorname{Var}_\theta(X)=\frac{\theta}{\theta+2}-\frac{\theta^2}{(\theta+1)^2}
=\frac{\theta}{(\theta+1)^2(\theta+2)}.
$$

The [central limit theorem](../../../../../central-limit-theorem.md) for the independent [statistical sample](../../../../../statistical-sample.md) gives

$$
\sqrt n(\bar X-\mu)\xrightarrow d
N\left(0,\frac{\theta}{(\theta+1)^2(\theta+2)}\right).
$$

For $g(x)=x/(1-x)$, its [derivative](../../../../../derivative.md) at the [mean](../../../../../expected-value-split.md) is $g'(\mu)=(1-\mu)^{-2}=(\theta+1)^2$. The [delta method](../../../../../delta-method.md) therefore gives

$$
\boxed{\sqrt n(T_1-\theta)\xrightarrow d
N\left(0,\frac{\theta(\theta+1)^2}{\theta+2}\right)}.
$$

Equivalently, the large-sample [normal approximation](../../../../../normal-approximation.md) is

$$
T_1\ \mathrel{\dot\sim}\ N\left(\theta,\frac{\theta(\theta+1)^2}{n(\theta+2)}\right),
\qquad v(T_1)=\frac{\theta(\theta+1)^2}{n(\theta+2)}.
$$

Here $v$ denotes the leading [asymptotic variance](../../../../../asymptotic-variance.md), rather than an assertion about an exact finite-sample [variance](../../../../../variance-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
