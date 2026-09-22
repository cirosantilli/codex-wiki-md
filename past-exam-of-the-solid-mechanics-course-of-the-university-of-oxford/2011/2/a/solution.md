<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the classical smooth setting, a [deformation in continuum mechanics](../../../../deformation-mechanics.md) is a sufficiently regular, [injective](../../../../injective-function.md) map $y:\Omega\to\mathbb R^3$ with $\det Dy>0$. [Injectivity](../../../../injective-function.md) excludes material interpenetration, and a positive [determinant](../../../../determinant.md) preserves orientation and local [volume](../../../../volume.md). We use $C^1$ regularity for these kinematics and additional differentiability where stress-divergence identities are applied.

[Cauchy's stress theorem](../../../../cauchy-s-stress-theorem.md) states that the contact [force](../../../../force-split.md) on an oriented surface element at a current point depends on the point and its [unit normal](../../../../unit-normal.md), rather than on the shape of the chosen subbody. Thus the contact [force](../../../../force-split.md) on the [boundary](../../../../boundary-of-a-set.md) of a current subbody $v$ has the form $\int_{\partial v}t(z,n)\,da$. Static [force](../../../../force-split.md) balance, for a [body force](../../../../body-force.md) $b$ per unit current [volume](../../../../volume.md), is

$$
\int_{\partial v}t(z,n)\,da+\int_vb(z)\,dv=0
$$

for every subbody. A shrinking pillbox gives $t(z,-n)=-t(z,n)$; a shrinking tetrahedron then gives linear dependence on the normal, $t(z,n)=S(z)n$. Applying the [divergence theorem](../../../../divergence-theorem.md) and using arbitrary subbodies gives

$$
\boxed{t(z,n)=S(z)n,\qquad\operatorname{div}S+b=0.}
$$

If [body force](../../../../body-force.md) is specified per unit mass instead, replace $b$ by $\rho b$. [Symmetry](../../../../symmetry-physics.md) of $S$ follows additionally from [conservation of angular momentum](../../../../conservation-of-angular-momentum.md) in the absence of body couples; it is not a consequence of [force](../../../../force-split.md) balance alone.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
