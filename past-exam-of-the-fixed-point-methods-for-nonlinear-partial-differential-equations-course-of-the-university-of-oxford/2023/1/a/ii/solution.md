<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The native paper prints $n\geq1$ while specifying $x_0$ alone. This does not determine $x_1$. We use the intended convention $x_{n+1}=\sin x_n$ for $n\geq0$; even with an independently chosen real $x_1$, the same proof gives the requested convergence.

For the [sine fixed-point iteration](../../../../../sine-fixed-point-iteration.md), after one step $x_1\in[-1,1]$. On this [interval](../../../../../interval-mathematics.md), the [sine](../../../../../sine.md) has the same sign as its argument, and

$$
0<\sin t<t\qquad(0<t\leq1).
$$

For example, $t-\sin t=\int_0^t(1-\cos s)\,ds>0$, since the [integrand](../../../../../integrand.md) is positive for $0<s\leq1$. By oddness of the [sine](../../../../../sine.md), $a_n=|x_n|$ consequently satisfies $a_{n+1}=\sin a_n\leq a_n$ for $n\geq1$. This [monotone sequence](../../../../../monotone-sequence.md) is bounded below by zero, so it has a limit $a\in[0,1]$. The [continuity](../../../../../continuous-function.md) of the [sine](../../../../../sine.md) gives $a=\sin a$, and the strict inequality above forces $a=0$.

Hence $x_n\to0$, and $0$ is a [fixed point](../../../../../fixed-point.md) of the [sine](../../../../../sine.md). It is the only real [fixed point](../../../../../fixed-point.md): every such point has absolute value at most one, where the preceding strict inequality applies. Thus

$$
\boxed{\lim_{n\to\infty}x_n=0\quad\text{for every real initial value}.}
$$

The [Banach fixed-point theorem](../../../../../contraction-mapping-theorem.md) does not directly apply to the [sine](../../../../../sine.md) on $[-1,1]$: the ratios $|\sin t-\sin0|/|t-0|$ tend to one as $t\to0$, so no uniform [contraction mapping](../../../../../contraction-mapping.md) constant smaller than one exists there.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../split.md)
6. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
