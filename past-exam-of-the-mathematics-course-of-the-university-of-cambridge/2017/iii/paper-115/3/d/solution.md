<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the double [covering map](../../../../../../covering-space.md) $\pi:S^n\to\mathbb{RP}^n$ and its deck [involution](../../../../../../involution.md), the [antipodal map](../../../../../../antipodal-map.md) $a(x)=-x$. The given sphere [cohomology](../../../../../../cohomology-split.md) vanishes outside degrees $0,n$, so only those degrees can survive as invariant classes. The degree-zero action is the identity because the sphere is connected for $n\geq1$.

For the top degree, orient $S^n$ as the boundary of the unit ball. A positive tangent basis $(v_1,\ldots,v_n)$ at $x$ means that $(x,v_1,\ldots,v_n)$ has positive [determinant](../../../../../../determinant.md) in $\mathbb R^{n+1}$. Under the antipodal map every one of these $n+1$ vectors changes sign, so the [orientation](../../../../../../orientation-of-a-simplex.md) sign is $(-1)^{n+1}$. Equivalently, the sphere [volume form](../../../../../../volume-form.md) is

$$
\omega_x(v_1,\ldots,v_n)=\det(x,v_1,\ldots,v_n),\qquad
\boxed{a^*\omega=(-1)^{n+1}\omega.}
$$

Its [cohomology](../../../../../../cohomology-split.md) class is nonzero by the integral argument and therefore generates the one-dimensional top [de Rham cohomology](../../../../../../de-rham-cohomology.md). Thus the top class is invariant precisely when $n$ is an [odd integer](../../../../../../odd-integer.md). Applying the quotient result yields

$$
\boxed{H^p_{\mathrm{dR}}(\mathbb{RP}^n)\cong
\begin{cases}
\mathbb R,&p=0,\\
\mathbb R,&p=n\text{ and }n\text{ is odd},\\
0,&\text{otherwise},
\end{cases}\qquad n\geq1.}
$$

In particular $\mathbb{RP}^1$ has one copy of $\mathbb R$ in each of degrees zero and one. These are real [cohomology](../../../../../../cohomology-split.md) groups; integral torsion is not detected by [de Rham cohomology](../../../../../../de-rham-cohomology.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
