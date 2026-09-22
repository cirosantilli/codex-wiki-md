<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $u=u_x$, $w=u_y$ and $B=B_y$. The [isothermal equation of state](../../../../../globally-isothermal-equation-of-state.md) replaces the adiabatic thermal equation by $p=c_s^2\rho$. Since the fields depend only on $x,t$, the solenoidal constraint gives $\partial_xB_x=0$ and the $x$ component of the [ideal magnetohydrodynamic induction equation](../../../../../ideal-magnetohydrodynamic-induction-equation.md) gives $\partial_tB_x=0$. Hence **$B_x$ is constant in both space and time**.

The continuity, two momentum and transverse induction equations are

$$
\begin{aligned}
\rho_t+u\partial_x\rho+\rho\partial_xu&=0,\\
u_t+u\partial_xu+\frac{c_s^2}{\rho}\partial_x\rho+\frac B{\mu_0\rho}\partial_xB&=0,\\
w_t+u\partial_xw-\frac{B_x}{\mu_0\rho}\partial_xB&=0,\\
B_t+u\partial_xB+B\partial_xu-B_x\partial_xw&=0.
\end{aligned}
$$

Here $B$ is the transverse magnetic component and the constant $B_x$ is the longitudinal component. The longitudinal magnetic force is the gradient of transverse [magnetic pressure](../../../../../magnetic-pressure.md); the transverse force is [magnetic tension](../../../../../magnetic-tension.md). In primitive variables the [isothermal coplanar magnetohydrodynamic characteristic matrix](../../../../../isothermal-coplanar-magnetohydrodynamic-characteristic-matrix.md) is

$$
\boxed{\mathbf A=\begin{pmatrix}
u&\rho&0&0\\
c_s^2/\rho&u&0&B/(\mu_0\rho)\\
0&0&u&-B_x/(\mu_0\rho)\\
0&B&-B_x&u
\end{pmatrix},\qquad \mathbf U_t+\mathbf A\mathbf U_x=0.}
$$

The imposed $z$ components stay zero because their corresponding equations have zero right-hand sides under this reduction.

Let $c=v-u$ be a [characteristic speed](../../../../../characteristic-speed.md) relative to the fluid and define the [Alfvén velocity](../../../../../alfven-velocity.md) $\mathbf v_a=\mathbf B/\sqrt{\mu_0\rho}$. To derive the characteristic polynomial, an [eigenvector](../../../../../eigenvector.md) with components $(\delta\rho,\delta u,\delta w,\delta B)$ obeys

$$
\begin{aligned}
c\delta\rho&=\rho\delta u,\\
c\delta u&=(c_s^2/\rho)\delta\rho+(B/\mu_0\rho)\delta B,\\
c\delta w&=-B_x\delta B/(\mu_0\rho),\\
c\delta B&=B\delta u-B_x\delta w.
\end{aligned}
$$

Eliminating $\delta u$ and $\delta w$ on a nondegenerate branch gives

$$
(c^2-c_s^2)\delta\rho=(B/\mu_0)\delta B,\qquad
(c^2-v_{ax}^2)\delta B=(Bc^2/\rho)\delta\rho.
$$

Their consistency yields $(c^2-c_s^2)(c^2-v_{ax}^2)=v_{ay}^2c^2$. Equivalently, direct expansion of $\det(\mathbf A-vI)$ gives the same polynomial without dividing by $c$ or a possibly vanishing field component:

$$
\boxed{(v-u_x)^4-(c_s^2+v_a^2)(v-u_x)^2+c_s^2v_{ax}^2=0.}
$$

Thus

$$
\boxed{v=u_x\pm c_f,\quad u_x\pm c_{\mathrm{slow}},\qquad
c_{f,\mathrm{slow}}^2=\frac12\left[c_s^2+v_a^2
\pm\sqrt{(c_s^2+v_a^2)^2-4c_s^2v_{ax}^2}\right].}
$$

The discriminant is $(c_s^2-v_a^2)^2+4c_s^2v_{ay}^2\geq0$, and both squared speeds are nonnegative. These are the [fast magnetosonic wave](../../../../../fast-magnetosonic-wave.md) and [slow magnetosonic wave](../../../../../slow-magnetosonic-wave.md) families, transported with the mean flow. The equations are hyperbolic; on a generic state the four distinct real [eigenvalues](../../../../../eigenvalue.md) give four characteristic directions. Special field alignments can make speeds coincide or the slow speed vanish. There is no separate entropy characteristic because the thermal model is isothermal, and the independent out-of-plane [Alfvén wave](../../../../../alfven-wave.md) polarization is excluded by $u_z=B_z=0$.

To construct a [simple wave in magnetohydrodynamics](../../../../../simple-wave-in-magnetohydrodynamics.md), take $\mathbf U=\mathbf U(a)$ along a state-space curve whose tangent is a right [eigenvector](../../../../../eigenvector.md) of one selected branch:

$$
\mathbf A(\mathbf U(a))\mathbf U'(a)=v(a)\mathbf U'(a).
$$

Substitution into the partial differential equations then gives the scalar transport equation

$$
\boxed{a_t+v(a)a_x=0.}
$$

Such curves exist locally by integrating the [eigenvector](../../../../../eigenvector.md) field away from degeneracies. For example, parameterizing by $a=\rho$ where its [eigenvector](../../../../../eigenvector.md) density component is nonzero gives the explicit state-curve equations

$$
\frac{du}{d\rho}=\frac c\rho,\qquad
\frac{dB}{d\rho}=\frac{Bc^2}{\rho(c^2-v_{ax}^2)},\qquad
\frac{dw}{d\rho}=-\frac{B_x}{\mu_0\rho c}\frac{dB}{d\rho},
$$

with signed $c$ equal to one of the four relative wave speeds. These formulas are used only where their denominators are nonzero.

A particularly transparent nonlinear example is an [isothermal perpendicular magnetosonic simple wave](../../../../../isothermal-perpendicular-magnetosonic-simple-wave.md). Set the allowed constant $B_x=0$, choose $B=K\rho$ and keep $w$ constant. For the fast branch,

$$
c_f(\rho)=\sqrt{c_s^2+K^2\rho/\mu_0},\qquad
u(\rho)=u_0+\sigma\int_{\rho_0}^{\rho}\frac{c_f(r)}r\,dr,\quad \sigma=\pm1.
$$

These relations satisfy the [eigenvector](../../../../../eigenvector.md) equations and therefore all four original equations whenever

$$
\rho_t+\lambda(\rho)\rho_x=0,\qquad \lambda=u(\rho)+\sigma c_f(\rho).
$$

The amplitude-dependent [characteristic speed](../../../../../characteristic-speed.md) has derivative

$$
\boxed{\lambda'(\rho)=\sigma\left[\frac{c_f}{\rho}
+\frac{K^2}{2\mu_0c_f}\right]\ne0.}
$$

This already proves the existence of genuinely nonlinear waves in the stated system.

More generally, the [method of characteristics](../../../../../method-of-characteristics.md) applied to initial data $a(x,0)=a_0(x)$ gives

$$
x=X+v(a_0(X))t,\qquad a(x,t)=a_0(X),\qquad
 a_x=\frac{a_0'(X)}{1+t\,v'(a_0(X))a_0'(X)}.
$$

If the initial speed decreases towards increasing $x$ somewhere, the denominator reaches zero in finite time. When the negative minimum is attained, the first steepening time is

$$
\boxed{t_*=-\frac1{\min_X\{v'(a_0(X))a_0'(X)\}}.}
$$

Faster trailing states catch slower leading states, giving [shock formation by characteristic intersection](../../../../../shock-formation-by-characteristic-intersection.md). For the right-moving perpendicular fast example, a negative density gradient provides such a compression. Beyond $t_*$ a smooth [simple wave](../../../../../simple-wave.md) is no longer sufficient and an appropriate shock solution is required. Rarefactive profiles instead spread. A [linearly degenerate characteristic field](../../../../../linearly-degenerate-characteristic-field.md) has $v'=0$ along its state curve and avoids this mechanism; the conclusion is that compressive nonlinear magnetosonic simple waves steepen, not that every possible MHD waveform must do so.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
