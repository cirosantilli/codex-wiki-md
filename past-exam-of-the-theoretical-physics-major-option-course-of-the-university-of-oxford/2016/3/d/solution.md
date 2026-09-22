<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Keep the same measure normalization as in the free [generating functional](../../../../generating-functional.md) and define

$$
W[J]=\mathcal N\int_{\rm periodic}\mathcal Dx\,
\exp\left[-S_0[x]-\int_0^\beta d\tau\left(\frac\lambda{4!}x^4+\frac\mu{6!}x^6\right)+\int_0^\beta d\tau\,Jx\right].
$$

Here $W$ is the source-dependent [partition function](../../../../canonical-partition-function.md), despite the common alternative convention in which that letter denotes its logarithm. A [functional derivative](../../../../functional-derivative.md) of $e^{\int Jx}$ brings down one factor $x(\tau)$ at the differentiated point. Expanding the interaction exponential and replacing each such factor by $\delta/\delta J(\tau)$ therefore gives

$$
\boxed{W[J]=\exp\left[-\int_0^\beta d\tau\left\{\frac\lambda{4!}\left(\frac\delta{\delta J(\tau)}\right)^4+
\frac\mu{6!}\left(\frac\delta{\delta J(\tau)}\right)^6\right\}\right]W_0[J].}
$$

Completing the square in the free [Gaussian integral](../../../../gaussian-integral.md) gives $W_0[J]=W_0[0]\exp(\tfrac12\int JG^{(0)}J)$ because $G^{(0)}=D^{-1}$ with periodic [boundary conditions](../../../../boundary-condition.md). Restoring $\hbar$ replaces the upper limit by $\hbar\beta$ and the interaction coefficients by $\lambda/(4!\hbar)$ and $\mu/(6!\hbar)$, exactly as in the source.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../e/solution.md)
