# Quadratic characteristic coordinates for a variable-speed wave equation

↑ **Parent:** [Hyperbolic partial differential equation](hyperbolic-partial-differential-equation.md)

On $x>0$, the [linear partial differential equation](linear-partial-differential-equation.md) $u_{xx}-x^2u_{yy}-u_x/x=0$ has [characteristic curves](characteristic-curve.md) $y\pm x^2/2=\text{constant}$. The [change of variables](change-of-variables-formula.md) $\xi=x^2-2y$, $\eta=x^2+2y$ has [Jacobian determinant](jacobian-determinant.md) $8x\ne0$. The [chain rule](chain-rule.md) gives

$$
u_{xx}-x^2u_{yy}-u_x/x=16x^2U_{\xi\eta}.
$$

Thus its [canonical form of a second-order partial differential equation](canonical-form-of-a-second-order-partial-differential-equation.md) is $U_{\xi\eta}=0$, and its general twice differentiable solution is $u=f(x^2-2y)+g(x^2+2y)$. The first derivative term exactly cancels the derivatives of the coordinate coefficients.

More generally, for positive differentiable $a(x)$, choose $s(x)$ with $s'(x)=a(x)$. Then the same cancellation gives

$$
u_{xx}-a(x)^2u_{yy}-\frac{a'(x)}{a(x)}u_x
=a(x)^2(U_{ss}-U_{yy}).
$$

The [characteristic](characteristic-of-a-field.md) coordinates are $s\pm y$. The quadratic example is $a(x)=x$, $s=x^2/2$, with both coordinates multiplied by two.

## ↑ Ancestors (8)

1. [Hyperbolic partial differential equation](hyperbolic-partial-differential-equation.md)
2. [Principal symbol of a partial differential equation](principal-symbol-of-a-partial-differential-equation.md)
3. [Quasilinear partial differential equation](quasilinear-partial-differential-equation.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford/2012/8/solution.md)
