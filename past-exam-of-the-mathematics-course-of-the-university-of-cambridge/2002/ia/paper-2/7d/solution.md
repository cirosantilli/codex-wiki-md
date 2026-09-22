<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

Two functions are [linearly dependent](../../../../../linear-dependence.md) if constants $c_1,c_2$, not both zero, satisfy $c_1y_1+c_2y_2=0$ identically. Differentiating also gives $c_1\dot y_1+c_2\dot y_2=0$. Since the determinant of these two equations is the nonzero [Wronskian](../../../../../wronskian.md) $W$, both constants must vanish. Hence **the two solutions are linearly independent.**

Differentiating the [Wronskian](../../../../../wronskian.md) and substituting the [homogeneous linear differential equation](../../../../../homogeneous-linear-differential-equation.md) gives

$$
\dot W=y_1\ddot y_2-y_2\ddot y_1=-p(t)(y_1\dot y_2-y_2\dot y_1)=-p(t)W.
$$

Integrating proves [Abel's identity](../../../../../abel-s-identity.md):

$$
\boxed{W(t)=W(t_0)\exp\left[-\int_{t_0}^t p(s)\,ds\right].}
$$

For [variation of parameters](../../../../../variation-of-parameters.md), impose $\dot a_1y_1+\dot a_2y_2=0$ on the proposed [particular solution](../../../../../particular-solution.md). Then $\dot y=a_1\dot y_1+a_2\dot y_2$, and substitution into the inhomogeneous [differential equation](../../../../../differential-equation-split.md) leaves $\dot a_1\dot y_1+\dot a_2\dot y_2=f$. Solving this two-by-two [linear system](../../../../../system-of-linear-equations.md) gives

$$
\dot a_1=-\frac{fy_2}{W},\qquad \dot a_2=\frac{fy_1}{W},\qquad \boxed{a_1=-\int_{t_0}^t\frac{f(s)y_2(s)}{W(s)}\,ds,\quad a_2=\int_{t_0}^t\frac{f(s)y_1(s)}{W(s)}\,ds.}
$$

Arbitrary constants of integration merely add a [homogeneous solution](../../../../../homogeneous-solution.md).

For the constant positive coefficient $q=\omega^2$, take $\omega>0$. Direct differentiation verifies that $y_1=\cos\omega t$ and $y_2=\sin\omega t$ solve the [homogeneous linear differential equation](../../../../../homogeneous-linear-differential-equation.md); their [Wronskian](../../../../../wronskian.md) is $W=\omega$. The requested integrands are

$$
\frac{fy_1}{W}=\frac{\sin(2\omega t)}{2\omega},\qquad \frac{fy_2}{W}=\frac{1-\cos(2\omega t)}{2\omega}.
$$

Taking $t_0=0$ yields

$$
a_1=-\frac{t}{2\omega}+\frac{\sin(2\omega t)}{4\omega^2},\qquad a_2=\frac{1-\cos(2\omega t)}{4\omega^2}.
$$

Thus **$|a_1(t)|\sim t/(2\omega)$ grows with power one, whereas $a_2$ is bounded.** Their combination simplifies to $y_p=-t\cos(\omega t)/(2\omega)+\sin(\omega t)/(2\omega^2)$; the final sine term is itself a [homogeneous solution](../../../../../homogeneous-solution.md). The secular term is the response to [resonance in a differential equation](../../../../../resonance-in-a-differential-equation.md).

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
