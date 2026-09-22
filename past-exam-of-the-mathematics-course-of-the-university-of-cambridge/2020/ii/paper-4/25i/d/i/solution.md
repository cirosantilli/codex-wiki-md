<h1 id="25i/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**False with the $\limsup$ printed in the paper.** Let the even-indexed surfaces be one fixed unit sphere and the odd-indexed surfaces one fixed ring torus. Then

$$
\limsup_{n\to\infty}\inf_{x\in S_n}K_n(x)=1>0,
$$

but infinitely many surfaces are tori. The two fixed surfaces lie in one ball and have uniformly bounded area. Their [injectivity radii](../../../../../../../injectivity-radius.md) have a positive common lower bound, and compactness gives a common bound on $|\nabla K|$, hence on every radial derivative $|\partial_rK|$. Thus this alternating sequence satisfies all four additional conditions as well.

The intended statement becomes true if $\limsup$ is replaced by

$$
\liminf_{n\to\infty}\inf_{x\in S_n}K_n(x)\geq0.
$$

Here is the proof. Put $\delta_n=\max(0,-\inf_{S_n}K_n)$, so $\delta_n\to0$. Choose $p_n$ maximizing distance from the centre of the fixed containing ball. The [supporting-sphere curvature bound](../../../../../../../supporting-sphere-curvature-bound.md) gives

$$
K_n(p_n)\geq\kappa:=R^{-2}>0.
$$

Write $K_0=K_n(p_n)$ and $j(r,\theta)=\sqrt{G(r,\theta)}$ in [geodesic polar coordinates](../../../../../../../geodesic-polar-coordinates.md). Choose a fixed sufficiently small $c>0$ and set $\rho_n=cK_0^{-1/2}$. Conditions (3) and (4) allow $c$ to be chosen so that $\rho_n\leq\epsilon_0$ and

$$
\frac12K_0\leq K_n(r,\theta)\leq\frac32K_0\qquad(0\leq r\leq\rho_n).
$$

The [Jacobi equation](../../../../../../../jacobi-equation.md) $j_{rr}=-K_nj$, with $j(0)=0$ and $j_r(0)=1$, and the [Sturm comparison theorem](../../../../../../../sturm-comparison-theorem.md) then give $j(r,\theta)\geq c_1r$ on this ball for a constant $c_1>0$ independent of $n$. Consequently

$$
\int_{B(p_n,\rho_n)}K_n\,dA
\geq\int_0^{2\pi}\int_0^{\rho_n}\frac{K_0}{2}c_1r\,dr\,d\theta
=\frac{\pi c_1c^2}{2}=:c_0>0.
$$

Since $K_n\geq-\delta_n$ elsewhere and $\operatorname{Area}(S_n)\leq M$,

$$
\int_{S_n}K_n\,dA\geq c_0-M\delta_n>0
$$

for all sufficiently large $n$. [Gauss-Bonnet](../../../../../../../gauss-bonnet-theorem.md) forces $\chi(S_n)>0$, and the [classification theorem for surfaces](../../../../../../../classification-theorem-for-surfaces.md) makes each such $S_n$ a sphere.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [25I](../../../25i.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
