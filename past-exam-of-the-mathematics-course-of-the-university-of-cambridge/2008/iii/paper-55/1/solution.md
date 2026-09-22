<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Differentiating the density with respect to the field and its first derivatives gives

$$
\mathcal L_\theta=-\sin\theta,\qquad
\mathcal L_{\theta_t}=\theta_t+A_1,\qquad
\mathcal L_{\theta_x}=-\theta_x-A_0.
$$

The [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) is consequently

$$
\boxed{\theta_{tt}-\theta_{xx}+\sin\theta+
(\partial_tA_1-\partial_xA_0)=0.}
$$

The external term is the [electric field](../../../../../electric-field.md) $E$ in the convention of the question. The derivative coupling is the [electromagnetic coupling of a sine-Gordon topological current](../../../../../electromagnetic-coupling-of-a-sine-gordon-topological-current.md): $j^0=\theta_x$, $j^1=-\theta_t$, so $\partial_\mu j^\mu=0$ identically.

When $E=0$ and $X=X_0+ut$, both $u$ and $\gamma=(1-u^2)^{-1/2}$ are constant. Put $y=\gamma(x-X)$ and $K(y)=\theta_K(y)$. Direct differentiation, or a [Lorentz boost](../../../../../lorentz-boost.md), gives

$$
\theta_x=\gamma K',\quad \theta_t=-\gamma uK',\quad
\theta_{tt}-\theta_{xx}=\gamma^2(u^2-1)K''=-K''.
$$

The static [Sine-Gordon kink](../../../../../sine-gordon-kink.md) equation $K''=\sin K$ then proves that **every stated constant-velocity boosted profile is an exact solution**. The range $|u|<1$ makes the boost real and subluminal.

To evaluate the proposed [collective-coordinate effective Lagrangian](../../../../../collective-coordinate-effective-lagrangian-for-a-soliton.md), use the instantaneous-boost prescription $u=\dot X$ and the stated velocity field $-\gamma uK'$, with the external electromagnetic [gauge potential](../../../../../gauge-field.md) $A_1=0$, $A_0=xf(t)$. The kink has

$$
K'=2\operatorname{sech}y,\qquad
1-\cos K=2\operatorname{sech}^2y=\frac12(K')^2,
$$

so

$$
\int_{\mathbb R}(K')^2dy=8,\qquad
\int_{\mathbb R}K'dy=2\pi,\qquad
\int_{\mathbb R}yK'dy=0.
$$

The last identity uses the evenness of $K'$. With $dx=dy/\gamma$, the kinetic and gradient terms combine to

$$
\frac12\int(\theta_t^2-\theta_x^2)dx
=\frac{\gamma(u^2-1)}2\int(K')^2dy=-\frac4\gamma,
$$

and the potential term is $-4/\gamma$. The external coupling is

$$
-\int xf(t)\theta_x\,dx
=-f(t)\int\left(X+\frac y\gamma\right)K'(y)dy=-2\pi Xf(t).
$$

Thus the [instantaneous-boost effective action for a sine-Gordon kink](../../../../../instantaneous-boost-effective-action-for-a-sine-gordon-kink.md) is

$$
\boxed{S_{\rm eff}=-\int\left[8\sqrt{1-\dot X^2}+2\pi Xf(t)\right]dt.}
$$

Its canonical [momentum](../../../../../momentum.md) is $P=8\gamma\dot X$. The resulting [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is

$$
\boxed{\frac d{dt}(8\gamma\dot X)=-2\pi f(t),\qquad
8\gamma^3\ddot X=-2\pi f(t).}
$$

Equivalently $P(t)=P(t_0)-2\pi\int_{t_0}^tf(s)ds$ and $\dot X=P/\sqrt{64+P^2}$. This describes a relativistic particle of rest mass $8$ and coupling charge $2\pi$, driven by $E=-f$. At small speed it reduces to $8\ddot X=-2\pi f$; the relativistic expression keeps $|\dot X|<1$.

There is also an exact force check at field level. For $P_{\rm field}=-\int\theta_t\theta_xdx$, the field equation and integration by parts give $\dot P_{\rm field}=\int E\theta_xdx$ when boundary stresses cancel. If $E=-f(t)$ and the field has kink boundary difference $2\pi$, this is $-2\pi f(t)$. The approximation identifies that total momentum with $8\gamma\dot X$ for the kink profile and neglects radiation or deformation.

The approximation's scope is important. An accelerating profile with $\gamma=\gamma(t)$ has actual derivative

$$
\partial_tK(\gamma(x-X))=
[\dot\gamma(x-X)-\gamma\dot X]K',
$$

whereas the velocity prescribed in the question omits the first term. Its contribution linear in $\dot\gamma$ integrates to zero by parity, but its square adds $\dot\gamma^2\int y^2(K')^2dy/(2\gamma^3)$ to the integrated density. Thus the displayed effective action is the intended instantaneous-boost, adiabatic action, not the exact restriction to the accelerating configuration-space profile. It is exact on the constant-velocity family when $E=0$; small forcing motivates neglecting the [acceleration correction for an instantaneous boosted kink](../../../../../acceleration-correction-for-an-instantaneous-boosted-kink.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
