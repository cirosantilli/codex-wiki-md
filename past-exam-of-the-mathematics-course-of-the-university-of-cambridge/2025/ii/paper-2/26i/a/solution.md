<h1 id="26i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A smooth curve $\alpha:I\to\mathbb R^3$ is regular when $\alpha'(t)\ne0$ for every $t\in I$. Its arc-length between parameters $t_0$ and $t_1$ is

$$
L(\alpha)=\int_{t_0}^{t_1}|\alpha'(t)|\,dt.
$$

Fix $t_0$ and define

$$
s(t)=\int_{t_0}^t|\alpha'(r)|\,dr.
$$

Regularity gives $s'(t)=|\alpha'(t)|>0$, so $s$ is strictly increasing and has a smooth inverse $t=t(s)$ on its image. The reparametrized curve $\beta(s)=\alpha(t(s))$ satisfies

$$
|\beta'(s)|=|\alpha'(t(s))|\frac{dt}{ds}=1.
$$

Thus every [regular curve](../../../../../../regular-curve.md) has an [arc-length parametrization](../../../../../../arc-length-parametrization.md).

For a unit-speed curve with nonzero curvature, let

$$
T=\beta',\qquad
\kappa=|T'|,\qquad
N=\frac{T'}{\kappa},\qquad
B=T\times N.
$$

Its torsion is

$$
\tau=-B'\cdot N,
$$

equivalently

$$
\tau=\frac{\det(\beta',\beta'',\beta''')}{|\beta'\times\beta''|^2}.
$$

If the curve lies in an affine plane, all three derivative vectors lie in the parallel two-dimensional vector plane, so their determinant is zero. Hence $\tau=0$ wherever torsion is defined.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26I](../../26i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
