<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write the reaction term as $f(u;r)=u(1-u)(u-r)$ and assume $D>0$. At $r=1/2$, multiply the stationary [travelling-wave reduction of a reaction-diffusion system](../../../../../travelling-wave-reduction-of-a-reaction-diffusion-system.md) $DU''+f(U;1/2)=0$ by $U'$ and integrate once. Since $U'=0$ at both asymptotic phases and $\int_0^U f(s;1/2)\,ds=-U^2(1-U)^2/4$, the integration constant is zero:

$$
\frac D2(U')^2-\frac14U^2(1-U)^2=0.
$$

The boundary orientation selects $U'=-U(1-U)/\sqrt{2D}$. Separating variables gives the [logistic front of a bistable cubic equation](../../../../../logistic-front-of-a-bistable-cubic-equation.md), with arbitrary center $q_0$:

$$
\boxed{U(x)=\frac1{1+\exp[(x-q_0)/\sqrt{2D}]}=\frac12\left[1-\tanh\frac{x-q_0}{2\sqrt{2D}}\right].}
$$

The arbitrary [translation](../../../../../translation-geometry.md) is expected from [translation invariance](../../../../../translation-invariance.md).

To develop the requested [perturbation theory](../../../../../perturbation-theory.md), let $r=1/2+\varepsilon a$ with signed $a=\pm1$, introduce slow time $T=\varepsilon t$, and put $z=(x-q(t))/\sqrt D$. Seek

$$
u=U_0(z)+\varepsilon U_1(z,T)+O(\varepsilon^2),\qquad \frac{\dot q}{\sqrt D}=\varepsilon c_1+O(\varepsilon^2),
$$

where $U_0(z)=(1+e^{z/\sqrt2})^{-1}$. The explicit $T$ derivative of $\varepsilon U_1$ is second order. Since $\partial_rf=-u(1-u)$, the first-order equation is

$$
LU_1=-c_1U_0'+aU_0(1-U_0),\qquad L=\frac{d^2}{dz^2}+f_u(U_0;1/2).
$$

Differentiation of $U_0''+f(U_0;1/2)=0$ gives $LU_0'=0$. The [self-adjoint differential operator](../../../../../self-adjoint-differential-operator.md) $L$ has this decaying [translation](../../../../../translation-geometry.md) mode, and $U_1\to0$ at both ends because the phases remain exactly $1$ and $0$. Multiplying the first-order equation by $U_0'$ and integrating by parts makes its left side zero. Therefore the [translation-mode solvability for a bistable front](../../../../../translation-mode-solvability-for-a-bistable-front.md) requires

$$
0=-c_1\int_{-\infty}^{\infty}(U_0')^2\,dz+a\int_{-\infty}^{\infty}U_0'U_0(1-U_0)\,dz.
$$

Both integrals can be evaluated without a special-function formula. The decreasing profile takes $U$ from $1$ to $0$ and has $U_0'=-U(1-U)/\sqrt2$, so

$$
\int U_0'U_0(1-U_0)\,dz=\int_1^0U(1-U)\,dU=-\frac16,
$$

and

$$
\int(U_0')^2\,dz=\int_1^0\left[-\frac{U(1-U)}{\sqrt2}\right]dU=\frac1{6\sqrt2}.
$$

The resulting speed is

$$
\boxed{c_1=-\sqrt2a,\qquad \dot q=-\sqrt{2D}(r-1/2)+O(\varepsilon^2)=\sqrt{D/2}(1-2r)+O(\varepsilon^2).}
$$

This derives the velocity by the [Fredholm solvability condition](../../../../../fredholm-solvability-condition.md), rather than substituting a guessed speed.

With this value, the forcing actually cancels pointwise: $-c_1U_0'+aU_0(1-U_0)=0$. Thus $LU_1=0$. The decaying [kernel](../../../../../kernel-of-a-linear-map.md) is only the [translation](../../../../../translation-geometry.md) direction: an independent solution is $U_0'\int^z(U_0')^{-2}\,d\zeta$, which grows at at least one infinity. Fixing the center by $U_1(0)=0$ consequently gives $\boxed{U_1=0}$. In this particular [bistable cubic reaction-diffusion equation](../../../../../bistable-cubic-reaction-diffusion-equation.md) the absence of shape deformation holds to all orders. Indeed $U_0''+f(U_0;r)=-(r-1/2)U_0(1-U_0)$, and the exact moving-frame equation has left side $-(\dot q/\sqrt D)U_0'$. Therefore

$$
\boxed{u(x,t)=\frac1{1+\exp[(x-q_0-ct)/\sqrt{2D}]},\qquad c=\sqrt{D/2}(1-2r)}
$$

is the exact front for every $0<r<1$. For $r<1/2$, $c>0$ and the $u=1$ phase advances to the right; for $r>1/2$ the $u=0$ phase advances to the left. The small-bias speed is consistent with the prescribed $\dot q/\sqrt D=O(\varepsilon)$ scaling.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
