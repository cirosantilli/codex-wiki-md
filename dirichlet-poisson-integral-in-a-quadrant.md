# Dirichlet Poisson integral in a quadrant

↑ **Parent:** [Poisson integral](poisson-integral.md)

The [conformal map](conformal-map.md) $w=z^2$ sends $x,y>0$ to the [complex upper half-plane](upper-half-plane-complex-analysis.md). For bounded continuous boundary values $g_2$ on the horizontal axis and $g_1$ on the vertical axis with equal corner values, set $f(s)=g_2(\sqrt s)$ for $s>0$ and $f(s)=g_1(\sqrt{-s})$ for $s<0$. The bounded [harmonic function](harmonic-function.md) with those [Dirichlet boundary conditions](dirichlet-boundary-condition.md) is

$$
u(z)=\frac1\pi\int_{\mathbb R}\frac{\operatorname{Im}(z^2)f(s)}{|s-z^2|^2}\,ds.
$$

Equivalently, if $z^2=a+ic$ with $c>0$, this is $\frac{2c}{\pi}\int_0^\infty r\left[g_2(r)/((r^2-a)^2+c^2)+g_1(r)/((r^2+a)^2+c^2)\right]dr$. The [Poisson kernel](poisson-kernel-for-the-upper-half-plane.md) is a positive [approximate identity](approximate-identity.md), so the prescribed edge values are attained. Boundedness is essential for uniqueness on this unbounded domain.

**Table of contents**

- [Bounded Dirichlet uniqueness in a quadrant](bounded-dirichlet-uniqueness-in-a-quadrant.md)
- [Zero-boundary harmonic growth in a quadrant](zero-boundary-harmonic-growth-in-a-quadrant.md)
- [Holomorphic derivative of a quadrant Dirichlet solution](holomorphic-derivative-of-a-quadrant-dirichlet-solution.md)

## ↑ Ancestors (8)

1. [Poisson integral](poisson-integral.md)
2. [Poisson kernel for the upper half-space](poisson-kernel-for-the-upper-half-space.md)
3. [Poisson equation](poisson-equation.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Holomorphic derivative of a quadrant Dirichlet solution](holomorphic-derivative-of-a-quadrant-dirichlet-solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-328/3/solution.md)
