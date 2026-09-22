<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Normalize the [discrete valuation](../../../../../../discrete-valuation.md) on $L$ by $v_L(L^\times)=\mathbb Z$, set $v_L(0)=+\infty$, and write $\mathcal O_L$ for its [valuation ring](../../../../../../valuation-ring.md). For a finite [Galois extension](../../../../../../finite-galois-extension.md) of [local fields](../../../../../../local-field.md), define $G_{-1}=G=\operatorname{Gal}(L/K)$ and, for integers $i\geq0$,

$$
\boxed{G_i=\{\sigma\in G:v_L(\sigma(a)-a)\geq i+1\text{ for every }a\in\mathcal O_L\}.}
$$

Equivalently, $G_i$ is the kernel of the action on $\mathcal O_L/\mathfrak m_L^{i+1}$. These are the [lower ramification numbering](../../../../../../lower-ramification-numbering.md) of the [ramification groups](../../../../../../ramification-group.md). In particular, $G_0$ is the [inertia group](../../../../../../inertia-group.md), the kernel of the action on the [residue field](../../../../../../residue-field.md), and $G_1$ is the [wild inertia group](../../../../../../wild-inertia-group.md). They form a decreasing sequence of [normal subgroups](../../../../../../normal-subgroup.md), eventually trivial.

For a real index $t\geq-1$, extend by $G_t=G_{\lceil t\rceil}$. Define the [Herbrand function](../../../../../../herbrand-function.md) by

$$
\varphi_{L/K}(t)=\int_0^t\frac{ds}{[G_0:G_s]}\quad(t\geq0),\qquad\varphi_{L/K}(t)=t\quad(-1\leq t\leq0).
$$

It is continuous, strictly increasing and piecewise linear; denote its inverse by $\psi_{L/K}$. The [upper ramification numbering](../../../../../../upper-ramification-numbering.md) is

$$
\boxed{G^u=G_{\psi_{L/K}(u)}\qquad(u\geq-1).}
$$

The definition includes the placement of the groups at break endpoints: the group at a break is the group before the drop. Lower numbering is compatible with subgroups; upper numbering is the one compatible with quotients. In a [totally ramified extension](../../../../../../totally-ramified-extension.md), the [uniformizer criterion for lower ramification groups](../../../../../../uniformizer-criterion-for-lower-ramification-groups.md) permits testing the defining [valuation](../../../../../../valuation.md) inequality on one [uniformizer](../../../../../../uniformizer.md) instead of on every integral element.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 123](../../../paper-123-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
