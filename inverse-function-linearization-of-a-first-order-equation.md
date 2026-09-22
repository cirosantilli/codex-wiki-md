# Inverse-function linearization of a first-order equation

↑ **Parent:** [Ordinary differential equation](ordinary-differential-equation.md)

On a branch where a differentiable [function](function-split.md) $y(x)$ has a nonzero [derivative](derivative.md), the [inverse function theorem](inverse-function-theorem.md) allows the [ordinary differential equation](ordinary-differential-equation.md) to be rewritten for $x(y)$. A nonlinear equation in one direction can become a [linear ordinary differential equation](linear-ordinary-differential-equation-split.md) in the other. For example, $y'=y/(x+y+c)$ becomes

$$
\frac{dx}{dy}-\frac{x}{y}=1+\frac{c}{y},\qquad y\ne0.
$$

The [integrating factor](integrating-factor.md) $1/y$ gives $(x/y)'=1/y+c/y^2$, hence $x+c=y(\ln|y|+C)$. This family must retain the original denominator restriction $x+y+c\ne0$. The separate zero solution $y=0$ on intervals avoiding $x=-c$ is lost by the inversion and must be restored.

## ↑ Ancestors (6)

1. [Ordinary differential equation](ordinary-differential-equation.md)
2. [Differential equation](differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/13/b/solution.md)
