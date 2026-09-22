# Box spline

↑ **Parent:** [Spline approximation](spline-approximation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Box_spline)

For a spanning direction matrix $\Xi=(\xi_1,\ldots,\xi_m)$ in $\mathbb R^d$, the [box spline](box-spline.md) is the density of the pushforward of uniform measure on $[0,1]^m$ under $t\mapsto\Xi t$. Equivalently,

$$
\int_{\mathbb R^d}M_\Xi(x)\varphi(x)\,dx=\int_{[0,1]^m}\varphi(\Xi t)\,dt.
$$

Its support is the [zonotope](zonotope.md) $\sum_j[0,1]\xi_j$. It is piecewise polynomial of total degree at most $m-d$. For integer directions, splitting each integration interval in half yields its binary refinement symbol

$$
2^d\prod_{j=1}^m\frac{1+z^{\xi_j}}2,
$$

up to the monomial specifying the choice of origin. If $r$ is the smallest number of directions whose removal leaves a nonspanning set, the usual [box spline](box-spline.md) smoothness criterion gives $C^{r-2}$ regularity. Repeated directions increase smoothness while enlarging support.

**Table of contents**

- [Unit-direction univariate box spline](unit-direction-univariate-box-spline.md)
- [Quadratic four-direction box spline](quadratic-four-direction-box-spline.md)
- [Twice-smoothed four-direction box spline](twice-smoothed-four-direction-box-spline.md)

## ↑ Ancestors (7)

1. [Spline approximation](spline-approximation.md)
2. [Spline (mathematics)](spline-mathematics.md)
3. [Uniform approximation](uniform-approximation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Box spline](box-spline.md)
- [Extraordinary subdivision vertex](extraordinary-subdivision-vertex.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-68/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-68/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66/6/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/5/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/5/e/solution.md)
- [Quadratic four-direction box spline](quadratic-four-direction-box-spline.md)
- [Twice-smoothed four-direction box spline](twice-smoothed-four-direction-box-spline.md)
- [Unit-direction univariate box spline](unit-direction-univariate-box-spline.md)
- [Zonotope](zonotope.md)
