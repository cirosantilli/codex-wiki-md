<h1 id="2/a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the direct [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) proof with the usual [supremum norm](../../../../../supremum-norm.md), take the [complete metric space](../../../../../complete-metric-space.md)

$$
\mathcal B=\{z\in C([a-h,a+h]):\|z-b\|_\infty\leq k\}
$$

and the [Picard iteration](../../../../../picard-iteration.md) map $Tz(x)=b+\int_a^x f(s,z(s))\,ds$. The estimates are

$$
\|Tz-b\|_\infty\leq Mh,\qquad
\|Tz-Tw\|_\infty\leq Lh\|z-w\|_\infty.
$$

Thus this proof requires

$$
\boxed{Mh\leq k\quad\text{and}\quad Lh<1.}
$$

The first inequality makes $T$ preserve $\mathcal B$; the strict second inequality makes it a [contraction mapping](../../../../../contraction-mapping.md). Its unique [fixed point](../../../../../fixed-point.md) is the desired [solution of a differential equation](../../../../../solution-of-a-differential-equation.md).

This is more restrictive than the preceding [Weierstrass M-test](../../../../../weierstrass-m-test.md) argument: a single application of $T$ must shrink every difference in the [supremum norm](../../../../../supremum-norm.md), whereas repeated [integration](../../../../../integral-split.md) in the other proof produces the [factorial](../../../../../factorial.md) $(n+1)!$ and convergence even when $Lh\geq1$. If $L=0$, the additional condition is automatic. These are conditions for the two stated direct proofs; they are not necessary bounds on the actual existence interval.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
