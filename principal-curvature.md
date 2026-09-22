# Principal curvature

↑ **Parent:** [Shape operator](shape-operator.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Principal_curvature)

At a point of a [smooth surface](smooth-surface.md), a [normal section of a surface](normal-section-of-a-surface.md) can bend by different amounts depending on its [tangent vector](tangent-vector-split.md). The [principal curvatures](principal-curvature.md) are the largest and smallest signed [normal curvatures](normal-curvature.md) among unit [tangent vectors](tangent-vector-split.md). Equivalently they are the two [eigenvalues](eigenvalue.md) $k_1,k_2$ of the [shape operator](shape-operator.md), with an [orthonormal basis](orthonormal-basis.md) $e_1,e_2$ of corresponding [principal directions](principal-direction.md). Here the labels follow the selected directions, without requiring $k_1\leq k_2$. [Ghomi, Lecture Notes 10, §2.3.3: normal curvature and principal curvatures](https://ghomi.math.gatech.edu/Classes/Math497C/LectureNotes10.pdf)

For a unit [tangent vector](tangent-vector-split.md) making [angle](angle.md) $\theta$ with $e_1$, [Euler formula for normal curvature](euler-formula-for-normal-curvature.md) gives

$$
v=\cos\theta\,e_1+\sin\theta\,e_2,\qquad k_n(\theta)=II(v,v)=k_1\cos^2\theta+k_2\sin^2\theta.
$$

The [normal curvature](normal-curvature.md) is a weighted average of the [principal curvatures](principal-curvature.md); the extremes occur in the [principal directions](principal-direction.md). If the [principal curvatures](principal-curvature.md) coincide, every direction in the [tangent plane](tangent-plane.md) is a [principal direction](principal-direction.md): this is an [umbilical point](umbilical-point.md). The [Gaussian curvature](gaussian-curvature.md) and [mean curvature](mean-curvature.md) summarize the pair by

$$
K=k_1k_2,\qquad H=\frac{k_1+k_2}{2}.
$$

For an outward-oriented [sphere](sphere.md) of [radius](radius.md) $R$, both [principal curvatures](principal-curvature.md) are $-1/R$, so the [normal curvature](normal-curvature.md) is $-1/R$ in every direction. For an outward-oriented [circular cylinder](circular-cylinder.md), choose $e_1$ around the circumference and $e_2$ along the axis. The [principal curvatures](principal-curvature.md) are $-1/R,0$, giving $k_n(\theta)=-\cos^2\theta/R$; halfway between the [principal directions](principal-direction.md), $k_n(\pi/4)=-1/(2R)$.

At the origin of the upward-oriented [hyperbolic paraboloid](hyperbolic-paraboloid.md) $z=(x^2-y^2)/2$, the [principal directions](principal-direction.md) are the coordinate axes and the [principal curvatures](principal-curvature.md) are $1,-1$ in the chosen length unit. Thus $k_n(\theta)=\cos(2\theta)$, with zero [normal curvature](normal-curvature.md) at $\theta=\pi/4,3\pi/4$. Zero [normal curvature](normal-curvature.md) in these directions coexists with [Gaussian curvature](gaussian-curvature.md) $-1$: the [shape operator](shape-operator.md) is not zero. The [mean curvature](mean-curvature.md) is zero at this point; this does not say that the whole [hyperbolic paraboloid](hyperbolic-paraboloid.md) is a [minimal surface](minimal-surface.md).

<a id="image-directional-normal-curvature-on-a-sphere-cylinder-and-saddle-with-the-convention-s-dn"></a>
![](principal-normal-curvature-directions.png)

**[Figure 1](#image-directional-normal-curvature-on-a-sphere-cylinder-and-saddle-with-the-convention-s-dn). Directional normal curvature on a sphere, cylinder, and saddle with the convention S=-dN**.

Each graph uses [angle](angle.md) $\theta$ in the [tangent plane](tangent-plane.md), measured from the indicated first [principal direction](principal-direction.md). The [sphere](sphere.md) and [circular cylinder](circular-cylinder.md) have $R=1$; the saddle graph refers only to the origin. Reversing the [unit normal](unit-normal.md) reflects each [normal curvature](normal-curvature.md) graph through zero, negates both [principal curvatures](principal-curvature.md) and the [mean curvature](mean-curvature.md), and preserves their product, the [Gaussian curvature](gaussian-curvature.md).

**Table of contents**

- [Principal direction](principal-direction.md)
- [Umbilical point](umbilical-point.md)

## ↑ Ancestors (7)

1. [Shape operator](shape-operator.md)
2. [Second fundamental form](second-fundamental-form-split.md)
3. [Differential geometry](differential-geometry-split.md)
4. [Geometry and topology](geometry-and-topology-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (50)

- [Catenoid is a minimal surface](catenoid-is-a-minimal-surface.md)
- [Circular cylinder](circular-cylinder.md)
- [Curvature](curvature.md)
- [Curvature-induced melting-temperature depression](curvature-induced-melting-temperature-depression.md)
- [Curvatures of a parametrized surface of revolution](curvatures-of-a-parametrized-surface-of-revolution.md)
- [Differential geometry of surfaces](differential-geometry-of-surfaces.md)
- [Elliptic point](elliptic-point.md)
- [Gaussian curvature](gaussian-curvature.md)
- [Intrinsic flatness of a circular cylinder](intrinsic-flatness-of-a-circular-cylinder.md)
- [Mean curvature](mean-curvature.md)
- [Mean curvature of a catenoid](mean-curvature-of-a-catenoid.md)
- [Mean curvature of a sphere and cylinder](mean-curvature-of-a-sphere-and-cylinder.md)
- [Minimal surface](minimal-surface.md)
- [Non-spherical surface of constant Gaussian curvature one](non-spherical-surface-of-constant-gaussian-curvature-one.md)
- [Parallel surface](parallel-surface.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-15/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3/12a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/24h/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/24h/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/23h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4/24h/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/24h/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-72/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/24i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-71/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-50/1/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/23i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/25i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/25h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/25h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/25h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/11e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/25i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/25i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/25i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3/2e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1/26i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/25g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/25g/b/solution.md)
- [Principal curvature](principal-curvature.md)
- [Principal direction](principal-direction.md)
- [Shape operator](shape-operator.md)
- [Soap film between coaxial rings](soap-film-between-coaxial-rings.md)
- [Stable minimal surface](stable-minimal-surface.md)
- [Supporting-sphere curvature bound](supporting-sphere-curvature-bound.md)
- [Theorema Egregium](theorema-egregium.md)
- [Umbilical point](umbilical-point.md)
- [Young–Laplace equation](young-laplace-equation.md)
