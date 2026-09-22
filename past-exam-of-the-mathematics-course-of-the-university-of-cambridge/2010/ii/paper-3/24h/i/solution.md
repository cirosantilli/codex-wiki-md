<h1 id="24h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Theorema Egregium](../../../../../../theorema-egregium.md) states that [Gaussian curvature](../../../../../../gaussian-curvature.md) is determined by the first fundamental form, and therefore preserved by local isometries. For a local surface parametrization $r$, write $g_{ij}=r_i\cdot r_j$, choose a [unit normal](../../../../../../unit-normal.md) $N$, and set $b_{ij}=r_{ij}\cdot N$. Decomposing the second [derivatives](../../../../../../derivative.md) into tangent and normal parts gives

$$
r_{ij}=\Gamma_{ij}^k r_k+b_{ij}N,\qquad
N_i=-b_i{}^k r_k,\qquad
\Gamma_{ij}^k=\tfrac12g^{k\ell}(\partial_i g_{j\ell}+\partial_j g_{i\ell}-\partial_\ell g_{ij}).
$$

Commute the third partial [derivatives](../../../../../../derivative.md) of $r$ and take tangent components. The terms involving [derivatives](../../../../../../derivative.md) of $b$ are normal; the tangent terms give the [Gauss equation](../../../../../../gauss-equation.md)

$$
\langle R(\partial_1,\partial_2)\partial_2,\partial_1\rangle
=b_{11}b_{22}-b_{12}^2,
$$

where $R$ is computed from [derivatives](../../../../../../derivative.md) and products of the displayed Christoffel symbols, using $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$. For example the tangent term from differentiating $b_{ij}N$ is $-b_{ij}b_k{}^\ell r_\ell$, which produces exactly the difference of the two products on the right. Consequently

$$
\boxed{K=\frac{b_{11}b_{22}-b_{12}^2}{\det g}
=\frac{\langle R(\partial_1,\partial_2)\partial_2,\partial_1\rangle}{\det g}.}
$$

The last expression depends only on $g$ and its [derivatives](../../../../../../derivative.md). Pulling back $g$ under a local isometry therefore preserves $K$, proving the theorem.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [24H](../../24h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
