<h1 id="11/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define a common displacement coordinate $X=(x_1+qx_2)/(1+q)$ and a relative displacement $\delta=x_1-x_2$. Adding and subtracting the equations of motion gives

$$
\ddot X=0,\qquad
\ddot\delta+\omega^2\delta=0.
$$

The general real motions of the two [normal modes](../../../../normal-mode.md) are therefore

$$
\begin{aligned}
\text{zero mode:}\quad &(x_1,x_2)=(C+Dt)(1,1),\\
\text{oscillatory mode:}\quad &(x_1,x_2)=
\bigl(A\cos\omega t+B\sin\omega t\bigr)(1,-1/q).
\end{aligned}
$$

Here $C,D,A,B$ are independent real constants. The [zero mode](../../../../zero-mode.md) includes uniform drift as well as a static common displacement; writing only a constant times $\cos0t$ would miss the independent linear-in-time solution. Their [superposition](../../../../superposition-principle.md) is

$$
\boxed{x_1=C+Dt+A\cos\omega t+B\sin\omega t,\qquad
x_2=C+Dt-\frac1q(A\cos\omega t+B\sin\omega t).}
$$

In the oscillatory [normal mode](../../../../normal-mode.md), $m_1x_1+m_2x_2=0$ and the two [amplitudes](../../../../wave-amplitude.md) have ratio $1/q$, with opposite [phases](../../../../phase-waves.md). Equivalently the oscillatory motion has zero total [angular momentum](../../../../angular-momentum.md) about the hoop center.

As $q\to\infty$ with $m_1,k$ fixed, $\omega\to\sqrt{2k/m_1}$ and the heavier particle's oscillatory [amplitude](../../../../wave-amplitude.md) tends to zero for fixed lighter-particle [amplitude](../../../../wave-amplitude.md). The lighter particle then oscillates against two effectively anchored [springs](../../../../spring.md) with combined [spring constant](../../../../spring-constant.md) $2k$. A common uniform [rotation](../../../../rotation-mathematics.md) remains an allowed [zero mode](../../../../zero-mode.md); the heavy particle is stationary in the limit only if the initial common drift is zero or tends to zero, as it does for bounded total [angular momentum](../../../../angular-momentum.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [11](../../11.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
