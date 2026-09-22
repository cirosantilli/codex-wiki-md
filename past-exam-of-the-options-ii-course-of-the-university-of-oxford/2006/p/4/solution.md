<h1 id="p/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [cubic spline](../../../../cubic-spline.md) is a twice continuously differentiable function whose restriction to each knot interval is a [polynomial](../../../../polynomial-split.md) of degree at most three. Its second derivative is continuous and piecewise linear. Natural endpoint conditions are $C''(x_0)=C''(x_n)=0$.

Linearity of both the piecewise-polynomial and smoothness conditions, and of the endpoint equations, makes the natural splines a [vector space](../../../../vector-space-split.md) $V$. A continuous piecewise linear second derivative with zero endpoint values is determined freely by its $n-1$ interior nodal values. Integrating twice adds two arbitrary affine constants. Hence

$$
\boxed{\dim V=(n-1)+2=n+1.}
$$

This count includes the case of one interval.

An interpolating [spline](../../../../spline-mathematics.md) has $S(x_i)=f_i$ at every node. Set $e=T-S$, so $e$ vanishes at all nodes. On each open knot interval $S^{(3)}$ is constant. Two integrations by parts give

$$
\int_{x_{i-1}}^{x_i}e''S''dx
=[e'S''-eS^{(3)}]_{x_{i-1}}^{x_i}.
$$

The terms containing $e$ vanish at nodes. When summed, the interior $e'S''$ terms cancel because $e'$ and $S''$ are continuous. The two outer terms vanish by the natural endpoint conditions. Thus

$$
\boxed{\int_{x_0}^{x_n}(T''-S'')S''dx=0.}
$$

Integrating the given square identity now yields the sharper energy decomposition

$$
\int_{x_0}^{x_n}(T'')^2dx
=\int_{x_0}^{x_n}(S'')^2dx+\int_{x_0}^{x_n}(T''-S'')^2dx.
$$

In particular **the natural interpolating [spline](../../../../spline-mathematics.md) minimizes the squared-curvature integral**.

If $T$ is another natural interpolant, the same minimizing argument in both directions makes the two energies equal. The final nonnegative integral then vanishes, so $T''=S''$ everywhere by [continuity](../../../../continuous-function.md). Their difference is affine and zero at all knots, including the two distinct endpoints, so $T=S$. This proves uniqueness.

It also supplies existence if needed: nodal evaluation is a [linear map](../../../../linear-map.md) from the $(n+1)$-dimensional space $V$ to $\mathbb R^{n+1}$. Its [kernel](../../../../kernel-of-a-linear-map-split.md) is zero by the same argument with zero data and the zero competitor. It is therefore [surjective](../../../../surjective-function.md), so every data vector has a natural [spline](../../../../spline-mathematics.md) interpolant.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [P](../../p.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
