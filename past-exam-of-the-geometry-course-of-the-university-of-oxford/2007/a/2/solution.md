<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a nonconstant [holomorphic map](../../../../holomorphic-map.md) of degree $d$ between compact connected [Riemann surfaces](../../../../riemann-surfaces-split.md),

$$
\boxed{2g_X-2=d(2g_Y-2)+\sum_{p\in X}(e_p-1),}
$$

where the [analytic ramification index](../../../../ramification-index-of-a-holomorphic-map.md) $e_p$ is the exponent in local coordinates $w\circ f=z^{e_p}$ after coordinate changes. A [meromorphic function](../../../../meromorphic-function.md) maps its [poles](../../../../pole.md) to infinity; the target coordinate $1/w$ is then holomorphic and vanishes at a [pole](../../../../pole.md), so this defines a [holomorphic map](../../../../holomorphic-map.md) to the [Riemann sphere](../../../../riemann-sphere.md). A [pole](../../../../pole.md) of order $m$ has local degree $m$.

Let $\Lambda$ be the [period lattice](../../../../period-lattice.md). The induced function $\wp:T=\mathbb C/\Lambda\to\mathbb{CP}^1$ has just one [pole](../../../../pole.md), of order two, so its degree is two. The [Riemann-Hurwitz formula](../../../../riemann-hurwitz-formula.md) gives total ramification four. The [pole](../../../../pole.md) contributes one; every [analytic ramification index](../../../../ramification-index-of-a-holomorphic-map.md) is at most two, so there are exactly three further [ramification points](../../../../ramification-point-of-a-holomorphic-map.md), each simple. Evenness of $\wp$, obtained by reindexing its lattice sum, identifies them with the three nonzero half-periods. Their values $e_1,e_2,e_3$ are distinct: two points of local degree two cannot lie in one degree-two fiber.

The functions $\wp'^2$ and $\prod_i(\wp-e_i)$ have double zeros at these same three points and a [pole](../../../../pole.md) of order six at zero. Their ratio is a holomorphic nowhere-zero function on the compact [torus](../../../../torus.md), hence constant. From $\wp(z)=z^{-2}+O(z^2)$ and $\wp'(z)=-2z^{-3}+O(z)$ its value is four. Therefore

$$
\boxed{\wp'^2=4(\wp-e_1)(\wp-e_2)(\wp-e_3),\qquad e_i\ne e_j\ (i\ne j).}
$$

**The printed additional assertion that all $e_i$ are nonzero is false.** The [square-lattice Weierstrass function has a zero branch value](../../../../square-lattice-weierstrass-function-has-a-zero-branch-value.md): for $\mathbb Z+i\mathbb Z$, reindexing gives $\wp(iz)=-\wp(z)$. At the half-period $h=(1+i)/2$, one has $ih=h-1$, so periodicity gives $\wp(h)=-\wp(h)$ and hence $\wp(h)=0$. Thus one branch value is zero, while the three remain distinct.

The [derivative](../../../../derivative.md) has a single triple [pole](../../../../pole.md), so **$\deg\wp'=3$**, and the [Riemann-Hurwitz formula](../../../../riemann-hurwitz-formula.md) gives **total ramification $\sum(e_p-1)=6$**. The number of distinct [ramification points](../../../../ramification-point-of-a-holomorphic-map.md) requires a further distinction. The absent constant term in the [Laurent expansion](../../../../laurent-series.md) gives $e_1+e_2+e_3=0$, so write $\wp'^2=4\wp^3-g_2\wp-g_3$. Differentiation yields $\wp''=6\wp^2-g_2/2$. If $g_2\ne0$, each of the two values $\pm\sqrt{g_2/12}$ has two distinct preimages under $\wp$ and none is a branch value, since a common zero of the cubic and its [derivative](../../../../derivative.md) would be a repeated cubic root. Thus there are four simple finite [ramification points](../../../../ramification-point-of-a-holomorphic-map.md) of $\wp'$ and its triple [pole](../../../../pole.md), giving **five distinct points**. If $g_2=0$, the nonsingularity of the cubic forces $g_3\ne0$. The two simple zeros of $\wp$ make $\wp''$ vanish to order two, so each has [analytic ramification index](../../../../ramification-index-of-a-holomorphic-map.md) three for $\wp'$. Together with its triple [pole](../../../../pole.md) there are **three distinct points**. This second case occurs for a hexagonal lattice: its sixth-root rotational symmetry forces the $z^2$ Laurent coefficient, and hence $g_2$, to vanish. The weighted count is six in both cases.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the geometry course of the University of Oxford](../../../split.md)
5. [Geometry course of the University of Oxford](../../../../geometry-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
