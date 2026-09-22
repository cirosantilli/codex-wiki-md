<h1 id="9a/solution">Solution</h1>

↑ **Parent:** [9A](../9a.md)

For an arbitrary smooth variation $q_i\mapsto q_i+\varepsilon\eta_i$ vanishing at both endpoints,

$$
\delta S=\int_{t_1}^{t_2}\sum_i\left(L_{q_i}\eta_i+L_{\dot q_i}\dot\eta_i\right)dt
=\int_{t_1}^{t_2}\sum_i\left(L_{q_i}-\frac d{dt}L_{\dot q_i}\right)\eta_i\,dt.
$$

The endpoint term in [integration by parts](../../../../../integration-by-parts.md) is zero. [stationarity](../../../../../stationary-process.md) for every variation and the [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md) imply the [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) $d(L_{\dot q_i})/dt=L_{q_i}$. Least action here means stationary action, not necessarily a global minimum. The [conjugate momentum](../../../../../canonical-momentum.md) is $p_i=L_{\dot q_i}$; a [cyclic coordinate](../../../../../cyclic-coordinate.md), $L_{q_i}=0$, makes $p_i$ constant.

For the [symmetric top](../../../../../symmetric-top.md), $\psi$ and $\phi$ are cyclic. Thus

$$
p_\psi=I_3(\dot\psi+\dot\phi\cos\theta)=I_3\omega_3,\qquad
p_\phi=I_1\dot\phi\sin^2\theta+I_3\omega_3\cos\theta
$$

are constant, and consequently so is $\omega_3$. [Conservation of energy from time-translation invariance](../../../../../conservation-of-energy-from-time-translation-invariance.md) also supplies the conserved [energy](../../../../../energy.md)

$$
E=\frac12I_1(\dot\theta^2+\dot\phi^2\sin^2\theta)+\frac12I_3\omega_3^2+V(\theta).
$$

These give the requested additional conserved quantities $p_\phi$ and $E$. The $\theta$ equation is

$$
I_1\ddot\theta=I_1\dot\phi^2\sin\theta\cos\theta-I_3\omega_3\dot\phi\sin\theta-V'(\theta).
$$

For constant $\theta$ and constant [precession](../../../../../precession.md) rate $\dot\phi$, it reduces to

$$
\boxed{I_1\dot\phi^2\sin\theta\cos\theta-I_3\omega_3\dot\phi\sin\theta=V'(\theta).}
$$

Conversely, choose constants satisfying this balance and set $\dot\psi=\omega_3-\dot\phi\cos\theta$. The cyclic equations and $\theta$ equation are then all satisfied, so this constructs uniform [precession](../../../../../precession.md) wherever the Euler-angle chart is regular.

## ↑ Ancestors (10)

1. [9A](../9a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
