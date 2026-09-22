# Circular arc maximizes area below a fixed chord

↑ **Parent:** [Isoperimetric constraint](isoperimetric-constraint.md)

For a single-valued [curve](curve.md) below the chord joining $(-a,0)$ to $(a,0)$, with length $2a<L\leq\pi a$, the maximum enclosed area is attained by the lower minor [circular arc](circular-arc.md). Equivalently it minimizes $\int_{-a}^a y\,dx$ at fixed length. Its equation and length are

$$
y=\sqrt{R^2-a^2}-\sqrt{R^2-x^2},\qquad
R\geq a,\qquad L=2R\arcsin(a/R).
$$

To prove global minimality for $R>a$, augment the objective by $R\int\sqrt{1+y'^2}\,dx$. The augmented integrand is linear in $y$ and strictly convex in $y'$. The displayed arc satisfies its [Euler-Lagrange equation](euler-lagrange-equation.md), so the supporting-line inequality for the convex slope dependence, followed by [integration by parts](integration-by-parts.md), proves it minimizes the augmented [functional](functional.md) among [curves](curve.md) with the prescribed endpoints. On the fixed-length class the multiplier term is constant. The [semicircle](semicircle.md) endpoint follows by a limit; its endpoint tangents are vertical but its length is finite.

## ↑ Ancestors (6)

1. [Isoperimetric constraint](isoperimetric-constraint.md)
2. [Euler-Lagrange equation](euler-lagrange-equation.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1/5/solution.md)
