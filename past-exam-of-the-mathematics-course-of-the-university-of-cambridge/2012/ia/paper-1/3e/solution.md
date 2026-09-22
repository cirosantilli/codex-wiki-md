<h1 id="3e/solution">Solution</h1>

↑ **Parent:** [3E](../3e.md)

A [continuous function](../../../../../continuous-function.md) at $x_0$ satisfies the following quantified condition:

$$
\boxed{\forall\varepsilon>0\ \exists\delta>0\ \forall x\in\mathbb R:\quad |x-x_0|<\delta\ \Longrightarrow\ |f(x)-f(x_0)|<\varepsilon.}
$$

The choice of $\delta$ may depend on $x_0$ and $\varepsilon$.

For the bounded example, take

$$
\boxed{f(x)=(1-x)\sin(1/x),\qquad 0<x\leq1.}
$$

This is a [continuous function](../../../../../continuous-function.md) on its domain and $|f(x)|\leq1-x<1$. Along $x_n=(\pi/2+2\pi n)^{-1}$ its values tend to $1$, while along $y_n=(3\pi/2+2\pi n)^{-1}$ its values tend to $-1$. Hence the [supremum](../../../../../supremum.md) is $1$ and the [infimum](../../../../../infimum.md) is $-1$, and neither is attained. “Upper and lower bound” here means the least upper and greatest lower bounds.

For the nonnegative function on the whole real line, if $f\equiv0$ the conclusion is immediate. Otherwise choose $x_*$ with $m=f(x_*)>0$. The limits at both infinities give $R>|x_*|$ such that $f(x)<m/2$ whenever $|x|>R$. By the [extreme value theorem](../../../../../extreme-value-theorem.md), a [continuous function](../../../../../continuous-function.md) on the compact interval $[-R,R]$ has a maximum $M=f(\alpha)$ there. Since $M\geq m$, it also exceeds every value outside this interval. Thus **$f$ is bounded above and attains its global maximum**. Nonnegativity ensures that either the function is zero or such a positive comparison value exists; without it, a function such as $-e^{-x^2}$ would have an unattained [supremum](../../../../../supremum.md) of zero.

## ↑ Ancestors (10)

1. [3E](../3e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
