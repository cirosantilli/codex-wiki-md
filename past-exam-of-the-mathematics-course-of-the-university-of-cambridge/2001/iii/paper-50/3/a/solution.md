<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [singular perturbation](../../../../../../singular-perturbation.md) is one for which setting the parameter to zero does not give a regular approximation uniformly over the region of interest. The limiting equation may lose a derivative or boundary condition, or a formally small correction may accumulate over a long time. Here the last mechanism occurs.

At fixed $t$, substitute a regular [asymptotic expansion](../../../../../../asymptotic-expansion.md). The leading equations and initial conditions give $y_0=3$ and $x_0=\sin t$. At first order,

$$
x_1''+x_1=-9\cos t,\qquad y_1'=\sin t-2,
$$

with zero initial corrections. Therefore

$$
x_1=-\frac92t\sin t,\qquad y_1=1-\cos t-2t.
$$

The secular terms become comparable with the leading terms at $t=O(\epsilon^{-1})$. **The fixed-time expansion is not uniform on the slow relaxation time.**

Introduce $\tau=\epsilon t$ through the [method of multiple scales](../../../../../../method-of-multiple-scales.md), and write $x=A(\tau)\sin t+O(\epsilon)$, $y=Y(\tau)+O(\epsilon)$. Average the second equation over the rapid oscillation. Since the sine has zero mean, $Y'=1-Y$, where the prime now denotes $d/d\tau$. With $Y(0)=3$, $Y=1+2e^{-\tau}$.

In the oscillator equation, $2(y')^2$ is of order $\epsilon^2$. The order-$\epsilon$ resonant cosine forcing is $-(2A'+3YA)\cos t$. A bounded first correction requires its coefficient to vanish, so

$$
2A'+3YA=0,\qquad A(0)=1.
$$

Integration gives the [slow oscillator damping by a relaxing auxiliary variable](../../../../../../slow-oscillator-damping-by-a-relaxing-auxiliary-variable.md):

$$
\boxed{A(\tau)=\exp\left[-\frac32\tau-3(1-e^{-\tau})\right].}
$$

Hence the uniform leading solution is

$$
\boxed{x(t)=e^{-3\epsilon t/2-3(1-e^{-\epsilon t})}\sin t+O(\epsilon),\qquad y(t)=1+2e^{-\epsilon t}+O(\epsilon).}
$$

To check the uniform ordering, the instantaneous sine forcing in the auxiliary equation is absorbed by a bounded first correction $-\epsilon A(\tau)\cos t$, plus a bounded slow correction chosen to match the initial data. The resonant first-order oscillator forcing has already been removed. Remaining order-$\epsilon^2$ terms accumulate by at most $O(\epsilon)$ over $0\leq t\leq K/\epsilon$ for fixed $K$. The slow coefficients stay bounded on this interval, and variation of constants for the oscillator and the auxiliary first-order equation gives the displayed uniform errors. Expanding the amplitude near $\tau=0$ gives $A=1-9\tau/2+\cdots$, recovering the secular term of the failed regular expansion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
