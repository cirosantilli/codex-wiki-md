<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The quantity inside a fixed interval changes by influx at its left endpoint minus outflux at its right endpoint:

$$
\frac d{dt}\int_a^b\rho\,dx=q(\rho(a,t))-q(\rho(b,t)).
$$

In a smooth region the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) turns this into $\int_a^b[\rho_t+\partial_xq(\rho)]\,dx=0$. Since the interval is arbitrary, the local [conservation law](../../../../../conservation-law.md) is $\boxed{\rho_t+\partial_xq(\rho)=0}$.

For a jump at $x=S(t)$, write the two smooth pieces using a [step function](../../../../../step-function.md). The singular part of $\rho_t$ is $-S'[\rho]\delta(x-S)$ and that of $\partial_xq$ is $[q]\delta(x-S)$. Cancellation gives the [Rankine-Hugoniot condition](../../../../../rankine-hugoniot-conditions.md)

$$
\boxed{S'[\rho]=[q],\qquad S'=[q]/[\rho]\quad\text{when }[\rho]\ne0.}
$$

The same identity follows by applying conservation to a shrinking moving control interval across the [shock](../../../../../shock-wave.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
