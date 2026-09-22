<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [Poisson process](../../../../poisson-process-split.md), $q_n=g$ and $r_n=0$, so

$$
\partial_tF=g(z-1)F,\qquad F(z,0)=1.
$$

This is an [ordinary differential equation](../../../../ordinary-differential-equation.md) in time for each fixed $z$, with solution

$$
\boxed{F(z,t)=e^{gt(z-1)}=e^{-gt}\sum_{n=0}^{\infty}\frac{(gt)^n}{n!}z^n.}
$$

Consequently

$$
\boxed{P_n(t)=e^{-gt}\frac{(gt)^n}{n!},\qquad n=0,1,2,\ldots.}
$$

The initial condition is interpreted as $P_0(0)=1$, with all other initial [probabilities](../../../../probability.md) zero. Normalization follows from $F(1,t)=1$. The [mean](../../../../expected-value-split.md) and [variance](../../../../variance-split.md) are both $gt$, as expected for independent events arriving at constant rate.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
