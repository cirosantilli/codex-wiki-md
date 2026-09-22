<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take $\epsilon\to0^+$. There are two real branches, on different scales. For a root tending to zero, the [Taylor series](../../../../../taylor-series.md) gives

$$
-\frac{x^3}{6}+O(x^5)=\epsilon(1-x^2).
$$

The [dominant balance](../../../../../dominant-balance.md) is $x^3\sim-6\epsilon$, so a [fractional-power root expansion](../../../../../fractional-power-root-expansion.md) yields

$$
\boxed{x_-\sim-(6\epsilon)^{1/3}}.
$$

More precisely $x_-=-(6\epsilon)^{1/3}+O(\epsilon)$. An ordinary [power series](../../../../../power-series.md) in integer powers of $\epsilon$ would miss this scale.

There is also a root escaping to positive infinity. Boundedness of the [sine](../../../../../sine.md) term makes the leading [dominant balance](../../../../../dominant-balance.md) $x-\epsilon x^2=0$. The nonzero branch is

$$
\boxed{x_+\sim\epsilon^{-1}}.
$$

Indeed the equation rearranges to $\epsilon x_+^2-x_+=\epsilon-\sin x_+$, which yields $x_+=\epsilon^{-1}+O(1)$ on this branch. The bounded oscillatory correction need not have a constant limiting value.

To check that these are all the real solutions, solve for the parameter:

$$
\epsilon=E(x):=\frac{x-\sin x}{x^2-1}.
$$

Positive values occur only on $(-1,0)$ and $(1,\infty)$; $x=\pm1$ are not roots. A useful exact [derivative](../../../../../derivative.md) is

$$
E'(x)=-\frac{2\{x\cos(x/2)-\sin(x/2)\}^2}{(x^2-1)^2}\leq0.
$$

It vanishes only at isolated points, so $E$ is strictly decreasing on each of these intervals. Its endpoint limits are $+\infty$ and zero on each interval. This [monotone parametrization of sine perturbation roots](../../../../../monotone-parametrization-of-sine-perturbation-roots.md) gives exactly one root in each interval for every $\epsilon>0$, proving that both asymptotic branches, and no others, have been included. If negative small parameters are allowed, the transformation $(x,\epsilon)\mapsto(-x,-\epsilon)$ reflects these two branches and gives all real solutions for that sign as well.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
