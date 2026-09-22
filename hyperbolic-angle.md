# Hyperbolic angle

↑ **Parent:** [Hyperbolic function](hyperbolic-function.md)

A [hyperbolic angle](hyperbolic-angle.md) $t$ is twice the signed [area](surface-area.md) $A$ enclosed by the two rays from the origin to $(1,0)$ and $(\cosh t,\sinh t)$ and the intervening arc of the unit [hyperbola](hyperbola.md). Counterclockwise traversal is positive: $t>0$ gives an ordinary [area](surface-area.md) $t/2$ above the horizontal axis, and $t<0$ gives signed [area](surface-area.md) $t/2$ below it. This parallels the [unit circle](complex-unit-circle.md), whose sector has [area](surface-area.md) $\theta/2$ for an [angle](angle.md) $\theta$ measured in [radians](radian.md).

To check the [area](surface-area.md) interpretation, write $x(u)=\cosh u$ and $y(u)=\sinh u$. [Green's theorem](green-theorem.md) expresses the signed [area](surface-area.md) as a [line integral](line-integral.md); the straight radial edges contribute zero, leaving

$$
A(t)=\frac12\int_0^t\bigl(x(u)y'(u)-y(u)x'(u)\bigr)\,du=\frac12\int_0^t\bigl(\cosh^2u-\sinh^2u\bigr)\,du=\frac t2.
$$

Thus $t$ is an [area](surface-area.md) parameter, rather than the ordinary [angle](angle.md) of the ray. For $t>0$, that ordinary [angle](angle.md) is $\arctan(\tanh t)$; it stays below $\pi/4$ even as the [hyperbolic angle](hyperbolic-angle.md) grows without bound.

## ↑ Ancestors (8)

1. [Hyperbolic function](hyperbolic-function.md)
2. [Exponential function](exponential-function.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Hyperbolic angle](hyperbolic-angle.md)
- [Hyperbolic function](hyperbolic-function.md)
