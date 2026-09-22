<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

Nonnegativity and symmetry of the [maximum product metric](../../../../../maximum-product-metric.md) follow from those of the two factor metrics. Its value is zero precisely when both coordinates agree. For three points $u=(x,x')$, $v=(y,y')$, $w=(z,z')$, the two [triangle inequalities](../../../../../triangle-inequality.md) give

$$
D(u,w)\le\max\{d(x,y)+d(y,z),d'(x',y')+d'(y',z')\}
\le D(u,v)+D(v,w).
$$

All metric axioms therefore hold.

When the two factors are the same [metric space](../../../../../metric-space.md), consider an off-diagonal point $(x,y)$ and set $\delta=d(x,y)>0$. A product-metric ball of radius $\delta/3$ cannot contain any $(z,z)$: such membership would imply $d(x,z),d(y,z)<\delta/3$ and then $d(x,y)<2\delta/3$, a contradiction. The complement of the diagonal is thus open, so

$$
\boxed{\Delta\text{ is closed in }X\times X.}
$$

This proves the [closed diagonal of a metric space](../../../../../closed-diagonal-of-a-metric-space.md). Equality of the factors here means equality as metric spaces, as intended; merely sharing an underlying set while allowing unrelated metrics would be a different assertion.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
