<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The difference of two successive [Picard iterates](../../../../../picard-iterate.md) factors as

$$
y_{n+1}(t)-y_n(t)=\int_0^tK(t,s)\bigl(y_n(s)+y_{n-1}(s)\bigr)\bigl(y_n(s)-y_{n-1}(s)\bigr)\,ds.
$$

The preceding bound and the kernel estimate therefore give

$$
\boxed{\|y_{n+1}-y_n\|_\infty\leq\frac{4B}{C_1}\|y_n-y_{n-1}\|_\infty
=\gamma\|y_n-y_{n-1}\|_\infty.}
$$

Moreover $D_1:=\|y_1-y_0\|_\infty\leq B^2/C_1$. Summing the resulting [geometric series](../../../../../geometric-series.md), for $m>n$,

$$
\|y_m-y_n\|_\infty\leq D_1\sum_{j=n}^{m-1}\gamma^j
\leq\frac{D_1\gamma^n}{1-\gamma}.
$$

Thus there is a [uniform limit](../../../../../uniform-limit.md) $y$ on $[0,\infty)$, continuous by the [uniform limit theorem](../../../../../uniform-limit-theorem.md), with $\|y\|_\infty\leq2B$. The integral passes to this limit because

$$
\sup_{t\geq0}\left|\int_0^tK(t,s)\bigl(y_n(s)^2-y(s)^2\bigr)\,ds\right|
\leq\frac{4B}{C_1}\|y_n-y\|_\infty\longrightarrow0.
$$

Therefore $y$ satisfies the [Volterra integral equation](../../../../../volterra-integral-equation.md), and hence the [initial value problem](../../../../../initial-value-problem.md). This proves global existence by [Global Picard iteration with a decaying kernel](../../../../../global-picard-iteration-with-a-decaying-kernel.md). The same estimate gives the useful error bound

$$
\boxed{\|y-y_n\|_\infty\leq\frac{B^2\gamma^n}{C_1(1-\gamma)}.}
$$

If $b=0$, every iterate is zero and the convergence assertion is immediate.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
