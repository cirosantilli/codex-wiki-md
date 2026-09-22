# Distributional second derivative across a jump

↑ **Parent:** [Distributional derivative](distributional-derivative.md)

Let $y$ be piecewise twice [continuously differentiable](continuously-differentiable-function.md), with finite one-sided values and derivatives at $c$, and write $[y]_c=y(c+)-y(c-)$. Its [distributional derivative](distributional-derivative.md) is $Dy=y'_{\mathrm{reg}}+[y]_c\delta_c$, and differentiating again gives

$$
D^2y=y''_{\mathrm{reg}}+[y']_c\delta_c+[y]_c\delta'_c.
$$

Here $\delta_c$ is the [Dirac delta](dirac-delta-function.md) at $c$, and the subscript reg means the ordinary derivative on the two open intervals, interpreted as a [regular distribution](regular-distribution.md). To prove the first formula, split $-\int y\varphi'$ at $c$ and use [integration by parts](integration-by-parts.md) on each piece for a [test function](test-function.md) $\varphi$. The two boundary contributions add to $[y]_c\varphi(c)$. Applying the same argument to the regular first derivative proves the second formula. Thus a derivative jump produces a delta source, whereas a value jump produces the derivative of a delta source.

## ↑ Ancestors (6)

1. [Distributional derivative](distributional-derivative.md)
2. [Distribution theory](distribution-theory-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-differential-equations-2-course-of-the-university-of-oxford/2017/1/b/i/solution.md)
- [Transmission conditions for a delta coefficient](transmission-conditions-for-a-delta-coefficient.md)
