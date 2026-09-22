<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

Take $a,b,c>0$ as the semiaxis lengths. For a centered axis-aligned box with positive half-edge lengths $x,y,z$, the [volume](../../../../../volume.md) is $V=8xyz$. Maximize $xyz$ under $g=x^2/a^2+y^2/b^2+z^2/c^2=1$. The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations are

$$
yz=2\lambda x/a^2,\qquad xz=2\lambda y/b^2,\qquad xy=2\lambda z/c^2.
$$

Multiplying by $x,y,z$, respectively, shows that $x^2/a^2=y^2/b^2=z^2/c^2$. The constraint makes each value $1/3$. All boundary boxes with a zero edge have zero volume, while the positive stationary box exists. [Compactness](../../../../../compact-space.md) therefore gives the [maximum box volume in an ellipsoid](../../../../../maximum-box-volume-in-an-ellipsoid.md)

$$
\boxed{x=a/\sqrt3,\quad y=b/\sqrt3,\quad z=c/\sqrt3,\qquad V_{\max}=\frac{8abc}{3\sqrt3}.}
$$

Allowing a displaced or differently oriented rectangular box cannot improve this result. Let $A=\operatorname{diag}(a,b,c)$, let $c_0$ be its center, and let $u_1,u_2,u_3$ be its perpendicular half-edge vectors. Averaging $|A^{-1}(c_0+\sum\varepsilon_i u_i)|^2\le1$ over the eight signs gives $|A^{-1}c_0|^2+\sum|A^{-1}u_i|^2\le1$. The determinant bound $|\det(A^{-1}u_1,A^{-1}u_2,A^{-1}u_3)|\le\prod|A^{-1}u_i|$, followed by the [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md), makes its volume at most $8abc/(3\sqrt3)$. The box found above attains the bound.

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
