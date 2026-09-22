<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [orthogonal complement](../../../../orthogonal-complement.md) is

$$
\boxed{Y^\perp=\{w\in X:\langle w,y\rangle=0\text{ for every }y\in Y\}.}
$$

It is a [linear subspace](../../../../vector-subspace.md) and is closed, since it is an intersection of [kernels](../../../../kernel-of-a-linear-map-split.md) of the continuous [linear functionals](../../../../linear-functional.md) $w\mapsto\langle w,y\rangle$. Continuity follows from the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md).

The minimizing point and orthogonality proved below write every $x$ as $x=y_0+(x-y_0)\in Y+Y^\perp$. If $w\in Y\cap Y^\perp$, then $\|w\|^2=\langle w,w\rangle=0$, so the intersection is zero. Consequently

$$
\boxed{X=Y\oplus Y^\perp.}
$$

In particular the minimizing point is unique: an alternative orthogonal decomposition would have a difference in this zero intersection.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
