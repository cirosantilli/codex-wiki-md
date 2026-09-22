<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We verify that the augmented [partition of an interval](../../../../../../../partition-of-an-interval.md) in part [i](../i.md) has vanishing [mesh of a partition](../../../../../../../mesh-of-a-partition.md). Define $\phi_n(t)=t^2/(t^2+n)$ for $t\geq0$. Its [derivative](../../../../../../../derivative.md) is

$$
\phi_n'(t)=\frac{2tn}{(t^2+n)^2}
=\frac1{\sqrt n}\frac{2u}{(1+u^2)^2},\qquad u=t/\sqrt n.
$$

Since $2u\leq1+u^2$ for $u\geq0$, we have $0\leq\phi_n'(t)\leq1/\sqrt n$. The [mean value theorem](../../../../../../../mean-value-theorem.md) therefore gives

$$
0<x_{k+1,n}-x_{k,n}\leq\frac1{\sqrt n}.
$$

The appended [interval](../../../../../../../interval-mathematics.md) has length $1/(n+1)$, so $\|\mathcal P_n\|\leq\max\{n^{-1/2},(n+1)^{-1}\}\to0$ for the augmented [partition of an interval](../../../../../../../partition-of-an-interval.md).

The [sine](../../../../../../../sine.md) is [continuous](../../../../../../../continuous-function.md), hence [Riemann integrable](../../../../../../../riemann-integrable-function.md) on $[0,1]$. By the [Riemann sum convergence theorem](../../../../../../../riemann-sum-convergence-theorem.md), $T_n\to\int_0^1\sin t\,dt=1-\cos1$, using the [fundamental theorem of calculus](../../../../../../../fundamental-theorem-of-calculus.md) and the [cosine](../../../../../../../cosine.md) [antiderivative](../../../../../../../antiderivative.md). As $T_n-S_n=\sin1/(n+1)\to0$, the answer is

$$
\boxed{\lim_{n\to\infty}S_n=1-\cos1.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
