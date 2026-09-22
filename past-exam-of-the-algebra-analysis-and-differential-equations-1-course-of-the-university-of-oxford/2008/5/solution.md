<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [hyperbolic cosine](../../../hyperbolic-cosine.md) is entire and $\cosh0=1$. Continuity makes it nonzero in a neighborhood of zero, so its reciprocal is holomorphic there and has a convergent [Taylor series](../../../taylor-series.md). Since $\cosh$ and its reciprocal are even, all odd coefficients vanish.

Multiply the proposed expansion by $\cosh z$:

$$
(1+c_2z^2+c_4z^4+\cdots)(1+\tfrac12z^2+\tfrac1{24}z^4+\cdots)=1.
$$

Coefficient comparison gives $c_2+1/2=0$ and $c_4+c_2/2+1/24=0$, hence

$$
\boxed{c_2=-\tfrac12,\qquad c_4=\tfrac5{24}.}
$$

The zeros of $\cosh z$ solve $e^{2z}=-1$, so they are $z=i(\pi/2+k\pi)$, $k\in\mathbb Z$. The nearest ones are $\pm i\pi/2$, and they are simple because $\sinh$ is nonzero there. The [hyperbolic secant](../../../hyperbolic-secant.md) has genuine poles at these points and is holomorphic in the disk of radius $\pi/2$. The [radius of convergence](../../../radius-of-convergence.md) of its Taylor series is therefore

$$
\boxed{R=\pi/2.}
$$

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2008](../../2008-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
