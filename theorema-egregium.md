# Theorema Egregium

↑ **Parent:** [Differential geometry](differential-geometry-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Theorema_Egregium)

For [smooth surfaces](smooth-surface.md), [Gaussian curvature](gaussian-curvature.md) depends only on the [first fundamental form](first-fundamental-form.md) and its first two coordinate [derivatives](derivative.md). Consequently any smooth [local isometry](local-isometry.md) $f:M\to N$ satisfies $K_N(f(p))=K_M(p)$. The surprise is that $K$ is defined using the [shape operator](shape-operator.md), which describes bending in space, yet its value can be recovered from measurements made entirely within the surface.

In his 1827 paper, [Carl Friedrich Gauss](carl-friedrich-gauss.md) expressed [Gaussian curvature](gaussian-curvature.md) through the metric coefficients and their [partial derivatives](partial-derivative.md) in Article 11, then stated its invariance under development in Article 12. Article 13 explicitly compares a [plane](plane.md) with surfaces developable onto it, including cylindrical surfaces. The paper was presented on 8 October 1827 and printed in 1828; the Morehead–Hiltebeitel English translation appeared in 1902. [Gauss's original paper in English translation, Articles 11–13 and title pages](https://www.gutenberg.org/files/36856/36856-pdf.pdf)

A [plane](plane.md) and a [circular cylinder](circular-cylinder.md) can have different [principal curvatures](principal-curvature.md) while both have $K=0$. Their matching [first fundamental forms](first-fundamental-form.md) exhibit the actual [local isometry](local-isometry.md). In contrast, no nonempty open patch of a [sphere](sphere.md) of radius $R$ can be flattened smoothly into a [plane](plane.md) while preserving its [first fundamental form](first-fundamental-form.md): $1/R^2$ cannot become zero. Making the patch small reduces practical distortion, but never produces an exact [local isometry](local-isometry.md). This is a geometric obstruction to a perfectly distance-preserving flat map of a spherical world, independent of where one places a seam.

The following proof outline connects the two descriptions of [Gaussian curvature](gaussian-curvature.md). For a [parametric surface](parametric-surface.md) with metric coefficients $g_{ij}$, decompose its second [derivatives](derivative.md) by the [Gauss formula](gauss-formula.md)

$$
X_{ij}=\Gamma^k_{ij}X_k+h_{ij}N.
$$

Taking [tangent vector](tangent-vector.md) [inner products](inner-product.md) determines the lowered [Christoffel symbols](christoffel-symbol.md) solely from the [Riemannian metric](riemannian-metric.md):

$$
\Gamma_{ijk}=\frac12(\partial_i g_{jk}+\partial_j g_{ik}-\partial_k g_{ij}).
$$

Comparing $X_{ijk}$ and $X_{ikj}$ gives the [Gauss equation](gauss-equation.md)

$$
R_{1212}=h_{11}h_{22}-h_{12}^2.
$$

Consequently

$$
K=\frac{h_{11}h_{22}-h_{12}^2}{\det(g_{ij})}
=\frac{R_{1212}}{\det(g_{ij})},
$$

where $R_{1212}$ is the corresponding component of the intrinsic [Riemann curvature tensor](riemann-curvature-tensor.md), with the sign convention in the displayed [Gauss equation](gauss-equation.md). The final expression uses only $g_{ij}$ and its first two [derivatives](derivative.md).

## ↑ Ancestors (5)

1. [Differential geometry](differential-geometry-split.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Differential geometry](differential-geometry-split.md)
- [Gaussian curvature](gaussian-curvature.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-15/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/23h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3/24h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/24h/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/25i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/26f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3/25i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-3/25i/c/solution.md)
