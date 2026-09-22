<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\psi=\theta+\varphi$, $U=\beta_r+\gamma_r$ and $V=\beta_i+\gamma_i$. The polar [amplitude equations](../../../../../../amplitude-equation.md) are

$$
\begin{aligned}
\dot R&=R(\mu-\beta_rR^2-\gamma_rS^2)+\nu S\cos\psi,\\
R\dot\theta&=-R(\beta_iR^2+\gamma_iS^2)-\nu S\sin\psi,
\end{aligned}
$$

with their reflected counterparts. On the equal-amplitude [standing wave](../../../../../../standing-wave.md) branch $R=S>0$, [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) requires

$$
Vz+\nu\sin\psi=0,\qquad \mu-Uz+\nu\cos\psi=0,\qquad z=R^2.
$$

Squaring and adding eliminates the phase:

$$
(U^2+V^2)z^2-2\mu Uz+\mu^2-\nu^2=0.
$$

For $U^2+V^2>0$ the candidate squared amplitudes are

$$
\boxed{z_\pm=\frac{\mu U\pm\sqrt{(U^2+V^2)\nu^2-\mu^2V^2}}{U^2+V^2}.}
$$

For each positive root, set $\sin\psi=-Vz/\nu$ and $\cos\psi=(Uz-\mu)/\nu$. The quadratic identity ensures these define a phase. Conversely these phase equations imply the quadratic, so a nonzero phase-locked branch exists exactly when the [discriminant](../../../../../../discriminant.md) is nonnegative **and at least one root is positive**.

Since $|\cos\chi|=|V|/\sqrt{U^2+V^2}$, the [discriminant](../../../../../../discriminant.md) condition is the printed $|\mu\cos\chi/\nu|\le1$ for $\nu\ne0$. It is sufficient under the usual above-onset supercritical assumptions $\mu>0,U>0$, because then the plus root is positive. Without these assumptions the condition is not sufficient: $\mu=-1,U=1,V=0,\nu=1/2$ satisfies it but gives $z=-1\pm1/2<0$. This is the [positivity condition for a phase-locked standing wave](../../../../../../positivity-condition-for-a-phase-locked-standing-wave.md), not a removable algebraic detail. The zero solution always exists and is distinct from the nonzero branch. For $\nu=0$, the undivided equations must be used; a nonzero [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) in this fixed rotating frame requires $V=0$ and $z=\mu/U>0$. If $U=V=0$, nonzero [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) require $\mu^2=\nu^2$ and a compatible phase, with no cubic amplitude selection.

Strong enough forcing can overcome the nonlinear frequency shift, lock the sum phase to the external signal and produce a [standing wave](../../../../../../standing-wave.md) at half the forcing frequency. The difference phase remains free through [spatial translation](../../../../../../spatial-translation.md). The amplitude inequality is an existence condition, not a stability theorem: attraction requires the linearized forced [amplitude equations](../../../../../../amplitude-equation.md), and nonlinear coefficients have not been restricted enough here to promise stability of every root.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
