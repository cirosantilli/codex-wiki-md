<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use homogeneous coordinates $x_0,\ldots,x_r$ on [projective space](../../../../projective-space-split.md) and let

$$
U_i=X\cap D_+(x_i),\qquad 0\leq i\leq r.
$$

These $r+1$ [open subschemes](../../../../open-subscheme.md) cover $X$. Each is a [closed subscheme](../../../../closed-subscheme.md) of the [affine scheme](../../../../affine-scheme.md) $D_+(x_i)$, hence is an [affine scheme](../../../../affine-scheme.md).

Every nonempty finite intersection is affine as well. Indeed, inside $D_+(x_{i_0})$ the intersection with $D_+(x_{i_1}),\ldots,D_+(x_{i_p})$ is the [principal open subscheme](../../../../principal-open-subscheme.md) obtained by inverting

$$
\prod_{j=1}^p\frac{x_{i_j}}{x_{i_0}}.
$$

Intersecting it with the [closed subscheme](../../../../closed-subscheme.md) $X$ gives $U_{i_0}\cap\cdots\cap U_{i_p}$, again an [affine scheme](../../../../affine-scheme.md).

For any [quasi-coherent sheaf](../../../../quasi-coherent-sheaf.md) $F$, [vanishing of quasi-coherent cohomology on an affine scheme](../../../../vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme.md) makes every such intersection acyclic for $F$. The [acyclic cover theorem](../../../../leray-s-theorem.md) therefore identifies the [sheaf cohomology](../../../../sheaf-cohomology.md) of $F$ with the [Čech cohomology](../../../../cech-cohomology.md) of this cover. Its alternating [Čech cochain complex](../../../../cech-cochain-complex.md) has terms

$$
\check C^p(\mathcal U,F)=\prod_{0\leq i_0<\cdots<i_p\leq r}\Gamma(U_{i_0}\cap\cdots\cap U_{i_p},F),
$$

which vanish for $p>r$: one cannot choose $p+1$ distinct indices from $r+1$ indices. Consequently

$$
\boxed{H^k(X,F)=0\quad(k>r),\qquad N=\max\{1,r\}.}
$$

The choice $N=\max\{1,r\}$ meets the strict requirement $N>0$ even when $r=0$. It is independent of $F$, and applies to all [quasi-coherent sheaves](../../../../quasi-coherent-sheaf.md), including those which are not [coherent sheaves](../../../../coherent-sheaf.md). This is the [cohomological dimension bound from an affine cover](../../../../cohomological-dimension-bound-from-an-affine-cover.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
