<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First classify nonzero [polynomial](../../../../polynomial-split.md) solutions of the [differential equation](../../../../differential-equation-split.md) itself. If $y$ has degree $d$ and leading [coefficient](../../../../coefficient.md) $a_d\ne0$, the [coefficient](../../../../coefficient.md) of $x^{d+1}$ is $(d+\lambda)a_d$. Hence $\lambda=-d$ is necessary.

An analytic solution at zero belongs to the exponent-zero Frobenius branch. Its odd-power [coefficients](../../../../coefficient.md) vanish, because $a_1=0$ and the [recurrence relation](../../../../recurrence-relation.md) preserves [parity](../../../../parity.md). For the even-power [coefficients](../../../../coefficient.md),

$$
a_{2j+2}=-\frac{2j+\lambda}{(2j+2)(4j+1)}a_{2j}.
$$

All denominators are nonzero for $j\geq0$. With $\lambda=-2m$, the [coefficients](../../../../coefficient.md) through $a_{2m}$ are nonzero when $a_0\ne0$, the next [coefficient](../../../../coefficient.md) vanishes, and every subsequent [coefficient](../../../../coefficient.md) vanishes. This proves sufficiency as well as the restriction to even [polynomial](../../../../polynomial-split.md) degree:

$$
\boxed{\lambda=-2m,\qquad m=0,1,2,\ldots,\qquad \deg y=2m=-\lambda.}
$$

For example, setting $a_0=1$ gives $1$ when $\lambda=0$, $1+x^2$ when $\lambda=-2$, and $1+2x^2+x^4/5$ when $\lambda=-4$. A [polynomial](../../../../polynomial-split.md) cannot instead begin with a [positive integer](../../../../positive-integer.md) power: its lowest power must have an [indicial exponent](../../../../indicial-exponent.md), and the only [integer](../../../../integer-split.md) [indicial exponent](../../../../indicial-exponent.md) is zero. This also proves that no odd-degree family was missed. The finite-series mechanism is a [terminating Frobenius series](../../../../terminating-frobenius-series.md).

**If the additional endpoint conditions from part (b) are imposed on this part too, there is no nonzero [polynomial](../../../../polynomial-split.md) solution:** every nonzero [polynomial](../../../../polynomial-split.md) just classified has $y(0)=a_0\ne0$. The displayed family and degree answer therefore concern the [differential equation](../../../../differential-equation-split.md) without those extra endpoint conditions.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the differential equations 2 course of the University of Oxford](../../../split.md)
5. [Differential equations 2 course of the University of Oxford](../../../../differential-equations-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
