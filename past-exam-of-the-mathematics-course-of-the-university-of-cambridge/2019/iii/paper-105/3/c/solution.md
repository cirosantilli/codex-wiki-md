<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Expanding the equation gives

$$
u_{xx}-(1-y^2)^2u_{yy}+4y(1-y^2)u_y=0,
$$

so its [principal symbol](../../../../../../principal-symbol-of-a-partial-differential-equation.md) is

$$
p(y,\xi)=\xi_x^2-(1-y^2)^2\xi_y^2.
$$

If a [characteristic curve](../../../../../../characteristic-curve.md) is locally a graph $y=y(x)$, its conormal is proportional to $(-y',1)$. The characteristic equation is therefore

$$
(y')^2-(1-y^2)^2=0,
\qquad
\frac{dy}{dx}=\pm(1-y^2).
$$

On each region separated by $y=\pm1$, separation of variables gives

$$
\frac12\log\left|\frac{1+y}{1-y}\right|=\pm x+C.
$$

Thus all the characteristic curves are

$$
\boxed{
\begin{cases}
y=\tanh(\pm x+C),&|y|<1,\\
y=\coth(\pm x+C),&|y|>1,\\
y=1\text{ or }y=-1.&
\end{cases}}
$$

The inner curves approach the horizontal characteristics $y=\pm1$ as $x\to\pm\infty$; the outer hyperbolic-cotangent branches have vertical asymptotes and also approach $y=\pm1$. This describes the requested sketch.

The initial line $x=0$ has conormal $(1,0)$, and $p(y,1,0)=1$, so it is a [non-characteristic hypersurface](../../../../../../non-characteristic-hypersurface.md) at every point. Since the coefficients and prescribed data are real analytic, the [Cauchy-Kovalevskaya theorem](../../../../../../cauchy-kovalevskaya-theorem.md) gives a unique real analytic solution in a neighborhood of each point of $\{x=0\}$, hence in a neighborhood of that line.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
