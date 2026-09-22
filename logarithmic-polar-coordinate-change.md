# Logarithmic polar coordinate change

↑ **Parent:** [Polar coordinates](polar-coordinates.md)

This [change of variables](change-of-variables-formula.md) replaces radius by its negative [logarithm](logarithm.md): $r=\sqrt{x^2+y^2}=e^{-s}$. The angular convention in the title measures $t$ from the positive $y$ axis toward the positive $x$ axis. Its [Jacobian determinant](jacobian-determinant.md) is $e^{-2s}>0$, so it supplies local coordinates on the punctured [plane](plane.md). For a single-valued [function](function-split.md) $u$, its expression $v(s,t)=u(x,y)$ is periodic in $t$ with period $2\pi$.

The [multivariable chain rule](multivariable-chain-rule.md) gives

$$
v_s=-xu_x-yu_y,\qquad v_t=yu_x-xu_y,
$$

and, for a twice continuously differentiable [function](function-split.md),

$$
v_{tt}-v_s=y^2u_{xx}-2xyu_{xy}+x^2u_{yy}.
$$

The first-order correction comes from differentiating the coefficients $x,y$ in the angular operator. Consequently the [partial differential equation](partial-differential-equation-split.md) with the right-hand expression equal to zero becomes the [heat equation](heat-equation.md) $v_s=v_{tt}$, with the logarithmic radial coordinate acting as the evolution variable.

## ↑ Ancestors (9)

1. [Polar coordinates](polar-coordinates.md)
2. [Change of variables formula](change-of-variables-formula.md)
3. [Multivariable calculus](multivariable-calculus-split.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-2/11/a/solution.md)
