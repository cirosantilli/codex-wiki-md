<h1 id="35d/solution">Solution</h1>

↑ **Parent:** [35D](../35d.md)

Use a [Lorentz boost](../../../../../lorentz-boost.md) along positive $x$ with $v=E/B$. Since $E<cB$, its dimensionless speed $\beta=E/(cB)$ is less than one. The given transformation of the [electric field](../../../../../electric-field.md) and [magnetic field](../../../../../magnetic-field.md) yields $E'_y=\gamma(\beta)(E-vB)=0$ and

$$
\boxed{\beta=\frac{E}{cB},\qquad B'=B\sqrt{1-\beta^2}=\sqrt{B^2-E^2/c^2}}.
$$

All other electric components vanish. In this frame a [magnetic field](../../../../../magnetic-field.md) does no work, so the particle's speed $u<c$ and [Lorentz factor](../../../../../lorentz-factor.md) $\gamma_u=(1-u^2/c^2)^{-1/2}$ are constant. In [proper time](../../../../../proper-time.md), the [Lorentz force](../../../../../lorentz-force.md) equations are $d(\gamma_u u_x')/d\tau=(qB'/m)\gamma_u u_y'$ and $d(\gamma_u u_y')/d\tau=-(qB'/m)\gamma_u u_x'$. Thus, choosing the phase and origin,

$$
ct'=\gamma_uc\tau,\qquad x'=\frac{\gamma_uu}{\omega}\sin\omega\tau,\qquad y'=\frac{\gamma_uu}{\omega}\cos\omega\tau,
\qquad\boxed{\omega=\frac{qB'}m}.
$$

This is the signed proper-time [cyclotron frequency](../../../../../cyclotron-frequency.md); the frequency with respect to $t'$ is $\omega/\gamma_u$. The inverse [Lorentz boost](../../../../../lorentz-boost.md) gives

$$
\boxed{\begin{aligned}
ct&=\gamma_u\gamma(\beta)\left(c\tau+\frac{\beta u}{\omega}\sin\omega\tau\right),\\
x&=\gamma_u\gamma(\beta)\left(\beta c\tau+\frac{u}{\omega}\sin\omega\tau\right),\\
y&=\frac{\gamma_uu}{\omega}\cos\omega\tau.
\end{aligned}}
$$

In particular the average drift speed is $\beta c=E/B$ along $\mathbf E\times\mathbf B$.

For $u>0$, $q\ne0$, set $s=\omega\tau$ and $d=\beta c/u$. The dimensionless spatial curve is

$$
\boxed{\widetilde x=\gamma(\beta)(ds+\sin s),\qquad\widetilde y=\cos s}.
$$

The drift between successive cycles is $2\pi\gamma(\beta)d$. When $2\pi\beta\ll u/c$, this is small compared with the oscillation size: the curve consists of nearly closed loops with slow rightward drift. When $2\pi\beta\gg u/c$, the longitudinal drift is large, producing a progressing oscillatory curve. More precisely $d\widetilde x/ds=\gamma(\beta)(d+\cos s)$: loops occur for $d<1$, cusps at $d=1$, and monotone progression for $d>1$. The stated large-drift inequality compares the drift over a full cycle, so an example of that regime with $d>1$ is shown; that comparison alone does not replace the exact loop criterion.

<a id="35d/image-the-relativistic-drift-of-a-charged-particle"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1-relativistic-drift.png)

**[Figure 3](#35d/image-the-relativistic-drift-of-a-charged-particle). The relativistic drift of a charged particle**.

Reversing $q$ reverses the cyclotron orientation; the drift remains along positive $x$. If $u=0$ the trajectory is pure straight drift and the dimensionless coordinates are undefined. If $q=0$ the particle is inertial and the displayed $1/\omega$ parametrization must be replaced by its inertial limit.

## ↑ Ancestors (10)

1. [35D](../35d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
