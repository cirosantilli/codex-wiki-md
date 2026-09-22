# Continuous hyperbolic coefficients need not admit smooth characteristic coordinates

↑ **Parent:** [Canonical form of a second-order partial differential equation](canonical-form-of-a-second-order-partial-differential-equation.md)

For a second-order [hyperbolic partial differential equation](hyperbolic-partial-differential-equation.md), the usual reduction to a mixed derivative uses twice continuously differentiable [characteristic coordinates](characteristic-coordinate.md). Continuity of the principal coefficients alone does not ensure this regularity, even locally. Consider $R=0$, $S=1/2$ and $T=|x|$ near the origin; the discriminant $S^2-RT$ is the positive constant $1/4$. A characteristic coordinate must satisfy

$$
\xi_y(\xi_x+|x|\xi_y)=0.
$$

The two characteristic families have first integrals $x$ and $y-x|x|/2$. Locally, any coordinate transverse to the first family has the form $\eta=h(y-x|x|/2)$ with $h'\ne0$. If this were twice continuously differentiable, its restriction at $x=0$ would make $h$ twice continuously differentiable. But its second $x$ derivative approaches $-h'(y)$ from the right and $h'(y)$ from the left, a contradiction. Independent characteristic coordinates cannot both choose the other family. Thus no twice continuously differentiable characteristic coordinate system exists near the origin.

With sufficiently smooth coefficients, the two distinct characteristic direction fields do yield smooth local coordinates. If $J$ is their [Jacobian determinant](jacobian-determinant.md) and $B$ is the transformed mixed coefficient, then $B^2=J^2(S^2-RT)>0$. Division by $2B$ gives the mixed-derivative canonical form, including all lower-order terms produced by the [chain rule](chain-rule.md). This is a local result; global intersections of characteristic curves can create separate obstructions.

## ↑ Ancestors (7)

1. [Canonical form of a second-order partial differential equation](canonical-form-of-a-second-order-partial-differential-equation.md)
2. [Linear partial differential equation](linear-partial-differential-equation.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2007/8/solution.md)
