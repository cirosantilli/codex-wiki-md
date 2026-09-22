<h1 id="g/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $K[y]=\int_a^bG(x,y,y')dx$. At a regular constrained extremal, the [first variation](../../../../first-variation.md) of $K$ is not identically zero. Choose a variation $\zeta$ for which $\delta K[\zeta]\neq0$; the [implicit function theorem](../../../../implicit-function-theorem.md) supplies a correction in the $\zeta$ direction to each other variation so that $K$ remains one. Stationarity of $J$ on these corrected variations implies $\delta J=\lambda\delta K$ for one scalar $\lambda$.

Put $L=F-\lambda G$. [Integration by parts](../../../../integration-by-parts.md) gives, for an arbitrary twice continuously differentiable variation $\eta$,

$$
0=\delta(J-\lambda K)[\eta]
=\int_a^b\left(L_y-\frac d{dx}L_{y'}\right)\eta\,dx
+[L_{y'}\eta]_a^b.
$$

Taking variations with zero endpoint values and using the stated [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) gives the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md). The remaining endpoint values are free and independent, giving the natural boundary conditions:

$$
\boxed{F_y-\lambda G_y-\frac d{dx}(F_{y'}-\lambda G_{y'})=0,\qquad
(F_{y'}-\lambda G_{y'})(a)=(F_{y'}-\lambda G_{y'})(b)=0.}
$$

If the constraint is not regular, the general multiplier statement permits an abnormal pair $\lambda_0F-\lambda_1G$ with $\lambda_0=0$; the source's general normal-form derivation implicitly excludes that case. In its quadratic example, regularity follows automatically from normalization: $\delta K[y]=2\int wy^2=2$.

For that example $L=py'^2-qy^2-\lambda wy^2$, so the equation and endpoint conditions reduce to

$$
(py')'+qy+\lambda wy=0,\qquad py'(a)=py'(b)=0.
$$

Multiply the equation by $y$ and integrate. The boundary term $[py'y]_a^b$ vanishes, giving

$$
-\int_a^bpy'^2dx+\int_a^bqy^2dx+\lambda\int_a^bwy^2dx=0.
$$

The last integral equals one, so **$\lambda=J[y]$**, the [functional](../../../../functional.md) value at the constrained extremal.

Finally multiply the equation for $y_1$ by $y_2$ and the equation for $y_2$ by $y_1$, then subtract and integrate. The derivative terms give only the vanishing boundary term $[p(y_2y_1'-y_1y_2')]_a^b$, while the $q$ terms cancel. Therefore $(\lambda_1-\lambda_2)\int_a^bwy_1y_2dx=0$. For distinct multipliers this proves

$$
\boxed{\int_a^bwy_1y_2dx=0.}
$$

## ↑ Ancestors (12)

1. [2](../2.md)
2. [G](../../g.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
