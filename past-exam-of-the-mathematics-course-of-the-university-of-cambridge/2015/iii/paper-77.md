# Paper 77

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_77.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_77.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)

## 1

↑ **Parent:** [Paper 77](paper-77.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Let $r=|\mathbf x|$, $n_i=x_i/r$, and let the source have size $\ell$. The [retarded acoustic Green function](../../../wave-equation.md#retarded-acoustic-green-function) gives the outgoing solution of [Lighthill acoustic analogy](../../../linear-acoustics.md#lighthill-acoustic-analogy) as

$$
\rho'(\mathbf x,t)=\frac1{4\pi c_0^2}\partial_{x_i}\partial_{x_j}\int\frac{T_{ij}(\mathbf y,t-|\mathbf x-\mathbf y|/c_0)}{|\mathbf x-\mathbf y|}\,d^3y.
$$

This follows by integrating the source derivatives by parts in the retarded convolution. Assume the source is localized and the boundary terms vanish. In the [acoustic compact-source approximation](../../../linear-acoustics.md#acoustic-compact-source-approximation), $k_0\ell\ll1$, the retardation across the source can be neglected, while $r\gg\ell$ permits replacement of the denominator by $r$. The integral becomes $S_{ij}(t-r/c_0)/r$.

In the radiation region $k_0r\gg1$, derivatives of the retarded argument dominate derivatives of the spreading factor. Since $\partial_{x_i}(t-r/c_0)=-n_i/c_0$, the leading [acoustic quadrupole](../../../linear-acoustics.md#acoustic-quadrupole) field is

$$
\boxed{\rho'(\mathbf x,t)\sim\frac{n_in_j\ddot S_{ij}(t-r/c_0)}{4\pi c_0^4r}=\frac{x_ix_j\ddot S_{ij}(t-r/c_0)}{4\pi c_0^4r^3}.}
$$

The two negative retardation derivatives give a positive sign. This is a far-field approximation, with smaller near-field terms omitted.

For low-[Mach number](../../../compressible-flow.md#mach-number) aerodynamic fluctuations of speed $U$ and advective time $\ell/U$, take $T_{ij}=O(\rho_0U^2)$, $S_{ij}=O(\rho_0U^2\ell^3)$, and two time derivatives of order $(U/\ell)^2$. Therefore

$$
\boxed{\frac{\rho'}{\rho_0}=O\left[\left(\frac U{c_0}\right)^4\frac\ell r\right]=O(m^4\ell/r).}
$$

The quoted fourth power is the [compact acoustic quadrupole Mach-number scaling](../../../linear-acoustics.md#compact-acoustic-quadrupole-mach-number-scaling), with geometric spreading shown explicitly. It assumes the source strength and time scale just stated; the source must be acoustically compact, and the observation point must remain in the radiation region.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Use complex amplitudes with time dependence $e^{i\omega t}$, so the outgoing two-dimensional [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) kernel has phase $e^{-ik_0r}$. Dividing the harmonic form of [Lighthill acoustic analogy](../../../linear-acoustics.md#lighthill-acoustic-analogy) by $c_0^2$ and integrating the two source derivatives by parts gives an amplitude proportional to

$$
\widetilde\rho'\sim\frac{k_0^2}{c_0^2}\frac{e^{-ik_0r}}{\sqrt{k_0r}}\,n_in_j\int\widetilde T_{ij}(\mathbf y)\,d^2y.
$$

Only the magnitude is needed here; the specified kernel omits its constant phase and normalization. In the [acoustic compact-source approximation](../../../linear-acoustics.md#acoustic-compact-source-approximation), $\int\widetilde T_{ij}d^2y=O(\rho_0U^2\ell^2)$. With $\omega=O(U/\ell)$, hence $k_0\ell=O(m)$, the [two-dimensional compact quadrupole scaling](../../../linear-acoustics.md#two-dimensional-compact-quadrupole-scaling) is

$$
\frac{|\widetilde\rho'|}{\rho_0}=O\left[\frac{U^2}{c_0^2}(k_0\ell)^2(k_0r)^{-1/2}\right]=\boxed{O\left(m^{7/2}\sqrt{\ell/r}\right).}
$$

The half-power difference from three dimensions comes from cylindrical spreading, including its $k_0^{-1/2}$ factor. As in part (i), the [Mach number](../../../compressible-flow.md#mach-number) power is stated with the geometrical range factor separated; $k_0r\gg1$ is still required.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Choose the [shock wave](../../../partial-differential-equation.md#shock-wave) normal to point from $S<0$ to $S>0$:

$$
\mathbf n=\frac{\nabla S}{|\nabla S|},\qquad v_n=\mathbf v\cdot\mathbf n=-\frac{S_t}{|\nabla S|}.
$$

The latter identity follows by differentiating $S(\mathbf x_s(t),t)=0$ along the moving surface. Write $[a]=a^+-a^-$ and $[\mathbf b]=\mathbf b^+-\mathbf b^-$. The [distributional derivative of the Heaviside step function](../../../distribution-theory.md#distributional-derivative-of-the-heaviside-step-function) is $\partial_tH(S)=S_t\delta(S)$ and $\nabla H(S)=\nabla S\,\delta(S)$. The regular terms cancel using the conservation equations on each side, leaving

$$
\partial_ta+\nabla\cdot\mathbf b=\left([a]S_t+[\mathbf b]\cdot\nabla S\right)\delta(S)=\left([\mathbf b]-\mathbf v[a]\right)\cdot\mathbf n\,|\nabla S|\delta(S).
$$

Thus the explicitly requested vector is

$$
\boxed{\mathbf f=[\mathbf b]-\mathbf v[a].}
$$

Only its normal component matters; adding tangential velocity to the surface parametrization changes neither result. The invariant [surface delta distribution](../../../distribution-theory.md#surface-delta-distribution) is $\delta_s=|\nabla S|\delta(S)$, so the formula is the [moving-interface conservation jump identity](../../../compressible-flow.md#moving-interface-conservation-jump-identity) $\partial_ta+\nabla\cdot\mathbf b=([\mathbf b]\cdot\mathbf n-v_n[a])\delta_s$.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Apply the [moving-interface conservation jump identity](../../../compressible-flow.md#moving-interface-conservation-jump-identity) first to mass, then to each momentum component. Write $j_i=\rho u_i$ and $\Pi_{ij}=\rho u_iu_j+p\delta_{ij}-\sigma_{ij}$, with all quantities understood piecewise on the two sides. Define the jumps of flux relative to the moving [shock wave](../../../partial-differential-equation.md#shock-wave) by

$$
Q=[\rho(\mathbf u-\mathbf v)\cdot\mathbf n],\qquad L_i=[\rho u_i(\mathbf u-\mathbf v)\cdot\mathbf n+p n_i-\sigma_{ij}n_j].
$$

The global distributional conservation equations are

$$
\partial_t\rho+\partial_ij_i=Q\delta_s,\qquad\partial_tj_i+\partial_j\Pi_{ij}=L_i\delta_s.
$$

Differentiate the first in time and subtract the divergence of the second. With $\rho'=\rho-\rho_0$ and the piecewise [Lighthill stress tensor](../../../linear-acoustics.md#lighthill-stress-tensor) $T_{ij}=\rho u_iu_j+(p'-c_0^2\rho')\delta_{ij}-\sigma_{ij}$, this gives

$$
\boxed{(\partial_t^2-c_0^2\nabla^2)\rho'=\partial_i\partial_jT_{ij}+\partial_t(Q\delta_s)-\partial_i(L_i\delta_s).}
$$

Derivatives act on the complete distributions, including their moving support. The [acoustic quadrupole](../../../linear-acoustics.md#acoustic-quadrupole) term represents momentum-stress fluctuations throughout the volume. The time derivative of the surface mass-flux defect is an [acoustic monopole](../../../linear-acoustics.md#acoustic-monopole), representing injection or removal of mass/volume. The divergence of the surface momentum-flux defect is an [acoustic dipole](../../../linear-acoustics.md#acoustic-dipole), representing a force sheet. This is the [distributional acoustic analogy across a moving interface](../../../linear-acoustics.md#distributional-acoustic-analogy-across-a-moving-interface).

For an actual freely propagating fluid [shock wave](../../../partial-differential-equation.md#shock-wave) with no singular mass or momentum supply, the [Rankine-Hugoniot conditions](../../../partial-differential-equation.md#rankine-hugoniot-conditions) give **$Q=0$ and $L_i=0$**. Such a shock does not acquire independent monopole and force-sheet sources merely because it is discontinuous. Its effects remain in the distributional derivatives of $T_{ij}$, including singular derivatives of its jump. Nonzero surface sources are appropriate for an interface with exchange/forcing or for a formulation that omits one side of the fluid.

**A shock does not, by itself, justify retaining the $m^4$ scaling.** That estimate required a low-[Mach number](../../../compressible-flow.md#mach-number) stress $O(\rho_0U^2)$ varying on the slow time $\ell/U$. Fast shock motion, short time scales, or thermodynamic deviations can invalidate that estimate. If these same compact, slow-source assumptions remain valid for the integrated [Lighthill stress tensor](../../../linear-acoustics.md#lighthill-stress-tensor), its quadrupole estimate still follows, even distributionally. There is no universal replacement power deducible from the mere presence of a shock; nor should vanished physical flux defects be treated as additional independent radiation sources.

## 2

↑ **Parent:** [Paper 77](paper-77.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use the [Fourier transform](../../../analysis.md#fourier-transform) convention $\widehat p(k,y)=\int_{\mathbb R}e^{ikx}p(x,y)dx$. Let $\gamma(k)^2=k^2-k_0^2$, choosing $\operatorname{Re}\gamma>0$ on the real contour with $\operatorname{Im}\omega<0$. For time dependence $e^{i\omega t}$, this is the decaying continuation of the outgoing [Sommerfeld radiation condition](../../../inverse-problem.md#sommerfeld-radiation-condition).

The transformed [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) has upper and lower solutions $P(k)e^{-\gamma y}$ and $Q(k)e^{\gamma y}$. The two kinematic traces give $-\gamma P=\rho_0\omega^2\widehat\eta=\gamma Q$, hence

$$
Q=-P,\qquad P=-\frac{\rho_0\omega^2}{\gamma}\widehat\eta,\qquad[\widehat p]=-\frac{2\rho_0\omega^2}{\gamma}\widehat\eta.
$$

The [elastic membrane](../../../continuum-mechanics.md#elastic-membrane) equation gives $[\widehat p]=(m\omega^2-Tk^2)\widehat\eta$. Therefore the [acoustic wave on a tensioned massive membrane](../../../linear-acoustics.md#acoustic-wave-on-a-tensioned-massive-membrane) has [dispersion relation](../../../wave-equation.md#dispersion-relation)

$$
\boxed{D(\omega,k)=m\omega^2-Tk^2+\frac{2\rho_0\omega^2}{\gamma(k)}=0.}
$$

Equivalently, $Tk^2=\omega^2(m+2\rho_0/\gamma)$. The fluid on both sides supplies a positive [added mass of an evanescent fluid layer](../../../linear-acoustics.md#added-mass-of-an-evanescent-fluid-layer), which is a useful independent check on the sign. In particular, the incident [pressure](../../../thermodynamics.md#pressure) is

$$
p_I(x,y)=-\operatorname{sgn}(y)\frac{\rho_0\omega^2}{\gamma_I}e^{-ik_Ix-\gamma_I|y|},\qquad\gamma_I=\gamma(k_I).
$$

The symbol $m$ here denotes [elastic membrane](../../../continuum-mechanics.md#elastic-membrane) mass per area, rather than the fluctuating [Mach number](../../../compressible-flow.md#mach-number) used in Question 1.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Linearity permits subtraction of the incident [acoustic membrane wave](../../../linear-acoustics.md#acoustic-wave-on-a-tensioned-massive-membrane). The scattered [pressure](../../../thermodynamics.md#pressure) solves the homogeneous [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation), and the kinematic relation defines its line displacement $\eta'$ on both halves. On $x<0$, subtracting the incident [elastic membrane](../../../continuum-mechanics.md#elastic-membrane) equation gives the scattered dynamic equation. On $x>0$, there is no [elastic membrane](../../../continuum-mechanics.md#elastic-membrane), so the total [pressure](../../../thermodynamics.md#pressure) jump must vanish, giving $[p']=-[p_I]$. The pinned endpoint has $\eta(0)=0$, hence **$\eta'(0)=-1$**, rather than zero.

Use full and [Half-range Fourier transforms](../../../analysis.md#half-range-fourier-transform) with the same $e^{ikx}$ convention as part (a), and put

$$
\beta=\rho_0\omega^2,\quad a(k)=m\omega^2-Tk^2,\quad A=\eta_x(0),\quad\kappa=k-k_I.
$$

Write $P^-$ for the left transform of the upper scattered [pressure](../../../thermodynamics.md#pressure), $P^+$ for its right transform, and $\eta^\pm$ for the corresponding transforms of $\eta'$. Outgoing antisymmetry in $y$ implies

$$
\eta^-+\eta^+=-\frac\gamma\beta(P^-+P^+),\qquad P^+=\frac{i\beta}{\kappa\gamma_I}.
$$

The second relation comes from the prescribed [pressure](../../../thermodynamics.md#pressure) cancellation on $x>0$.

The endpoint terms in the left [Fourier transform](../../../analysis.md#fourier-transform) of $\eta'_{xx}$ are crucial:

$$
\int_{-\infty}^0e^{ikx}\eta'_{xx}dx=\eta'_x(0)-ik\eta'(0)-k^2\eta^-=A+i(k+k_I)-k^2\eta^-.
$$

Thus $2P^-=a\eta^-+TA+iT(k+k_I)$. Eliminating $\eta^-$ gives the [Wiener-Hopf equation](../../../differential-equation.md#wiener-hopf-equation)

$$
\boxed{K(k)P^-(k)+\eta^+(k)=\frac{TA}{a(k)}+\frac{iT(k+k_I)}{a(k)}-\frac{i\gamma(k)}{(k-k_I)\gamma_I},\qquad K(k)=\frac2{a(k)}+\frac{\gamma(k)}\beta.}
$$

There is a defect in the printed right side: with the stated incident exponential, [pressure](../../../thermodynamics.md#pressure) jump, and pinned total displacement, it omits the incident endpoint term and has the opposite sign on the incident-pressure term. The displayed corrected equation follows directly from both boundary traces. The given right side cannot be derived with these definitions. Using $a(k_I)=-2\beta/\gamma_I$, an especially useful equivalent form is

$$
K P^-+\eta^+=\frac{TA}{a}-\frac i\kappa-\frac{i\beta K}{\kappa\gamma_I}.
$$

The correction is necessary for the reconstructed [pressure](../../../thermodynamics.md#pressure) to satisfy the original physical boundary conditions.

For [Wiener-Hopf factorization](../../../differential-equation.md#wiener-hopf-factorization), take $K=K^+K^-$ with the plus factor analytic and nonzero in the upper half-plane and the minus factor analytic and nonzero in the lower half-plane. Singularities listed next refer to continuation out of each factor's own analytic half-plane. Let $b=\omega\sqrt{m/T}$, so $a=-T(k-b)(k+b)$ and $b$ lies below the real axis. Generically $K^+$ inherits the [pole](../../../isolated-singularity.md#pole) at $b$ and the square-root [branch point](../../../complex-analysis.md#branch-point) at $k_0$, while $K^-$ inherits the [pole](../../../isolated-singularity.md#pole) at $-b$ and the [branch point](../../../complex-analysis.md#branch-point) at $-k_0$. The kernel is finite but nonanalytic at the acoustic branch points: its local behavior is a constant plus a square-root term, not an inverse-square-root divergence. Coincident branch points and poles require a limiting treatment.

Zeros of $K$ are the fluid-loaded [dispersion relation](../../../wave-equation.md#dispersion-relation) roots. Lower-half-plane roots, including the incoming guided root $k_I$, belong to the continued $K^+$; upper-half-plane roots, including the reflected root $-k_I$ for the even kernel, belong to the continued $K^-$. The roots represent membrane-guided modes; the branch cuts represent radiated acoustic waves. Only roots on the selected outgoing sheet are included, not spurious roots created by squaring the dispersion relation. No explicit factorization is required.

Here is an explicit solution in terms of those factors. Define

$$
B(k)=\frac{T}{a(k)K^+(k)},\qquad C=\frac{1}{2bK^+(-b)},\qquad B^-(k)=\frac C{k+b},\qquad B^+(k)=B(k)-\frac C{k+b}.
$$

The [pole](../../../isolated-singularity.md#pole) of $B$ at $-b$ has residue $C$; the [pole](../../../isolated-singularity.md#pole) at $b$ is canceled by the [pole](../../../isolated-singularity.md#pole) of $K^+$. Thus $B^\pm$ have the required respective analyticity. Divide the corrected [Wiener-Hopf equation](../../../differential-equation.md#wiener-hopf-equation) by $K^+$ and split its right side as $F^++F^-$, where

$$
\begin{aligned}
F^-&=A\frac C{k+b}-\frac{i\beta}{\gamma_I}\frac{K^-(k)-K^-(k_I)}{k-k_I},\\
F^+&=AB^+(k)-\frac{i}{(k-k_I)K^+(k)}-\frac{i\beta K^-(k_I)}{(k-k_I)\gamma_I}.
\end{aligned}
$$

The difference quotient in $F^-$ is removable at $k_I$ and is analytic below. Moving the plus and minus terms to opposite sides yields the common [entire function](../../../complex-analysis.md#entire-function). With the assumed **$E(k)=0$**, the solution is

$$
\boxed{P^-=\frac{F^-}{K^-},\qquad\eta^+=K^+F^+.}
$$

Combining $P^-$ with the known $P^+$ gives the full scattered [pressure](../../../thermodynamics.md#pressure) transform

$$
P^-+P^+=\frac1{K^-(k)}\left[\frac{AC}{k+b}+\frac{i\beta K^-(k_I)}{(k-k_I)\gamma_I}\right].
$$

The requested [pressure](../../../thermodynamics.md#pressure) integral, for $y\ne0$, is consequently

$$
\boxed{p(x,y)=p_I(x,y)+\frac{\operatorname{sgn}(y)}{2\pi}\int_{\mathcal C}e^{-ikx-\gamma(k)|y|}\frac1{K^-(k)}\left[\frac{AC}{k+b}+\frac{i\beta K^-(k_I)}{(k-k_I)\gamma_I}\right]dk.}
$$

The real contour $\mathcal C$ uses the causal continuation $\operatorname{Im}\omega<0$; its undamped limit retains the induced [pole](../../../isolated-singularity.md#pole) and branch-cut prescriptions. The [residue theorem](../../../analysis.md#residue-theorem) shows that upper-half-plane zeros of $K^-$ yield left-going scattered [elastic membrane](../../../continuum-mechanics.md#elastic-membrane) modes. On the right, the lower incident-pole residue of the scattered integral cancels $p_I$ at the open line, as required.

Finally reconstruct the left scattered displacement:

$$
\boxed{\eta^-=\frac{2P^- -TA-iT(k+k_I)}{a(k)}.}
$$

For a generic unspecified $A$, this has a lower-half-plane [pole](../../../isolated-singularity.md#pole) at the bare [elastic membrane](../../../continuum-mechanics.md#elastic-membrane) wavenumber $b$. Such a [pole](../../../isolated-singularity.md#pole) is incompatible with analyticity of an outgoing left-supported scattered displacement: it would represent an additional right-going incoming [elastic membrane](../../../continuum-mechanics.md#elastic-membrane) contribution. It must be removed. Its residue is $-[2P^-(b)-TA-iT(b+k_I)]/(2Tb)$, so the [incoming-pole cancellation at a pinned membrane edge](../../../linear-acoustics.md#incoming-pole-cancellation-at-a-pinned-membrane-edge) condition is

$$
\boxed{2P^-(b)-TA-iT(b+k_I)=0.}
$$

Since $P^-$ is linear in $A$, this fixes the endpoint slope generically. Explicitly it is

$$
A\left[T-\frac{C}{bK^-(b)}\right]=\frac{2i\beta K^-(k_I)}{(b-k_I)\gamma_I K^-(b)}.
$$

The physical lower incident [pole](../../../isolated-singularity.md#pole) of the total displacement is already prescribed by $\eta_I$; it must not be confused with this removable spurious [pole](../../../isolated-singularity.md#pole) of the scattered field.

## 3

↑ **Parent:** [Paper 77](paper-77.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Inviscid Burgers equation](../../../partial-differential-equation.md#inviscid-burgers-equation) here has the negative quadratic flux $F(f)=-f^2/2$. By the [method of characteristics](../../../partial-differential-equation.md#method-of-characteristics), $df/dZ=0$ and $d\theta/dZ=-f$, so a characteristic beginning at $\theta_0$ satisfies

$$
\boxed{\theta=\theta_0-f_0(\theta_0)Z,\qquad f(Z,\theta)=f_0(\theta_0).}
$$

This is a classical solution until [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) intersect. Across a [shock wave](../../../partial-differential-equation.md#shock-wave), the [Rankine-Hugoniot condition](../../../partial-differential-equation.md#rankine-hugoniot-conditions) gives

$$
\boxed{\theta_s'=\frac{F(f_R)-F(f_L)}{f_R-f_L}=-\frac{f_R+f_L}{2}.}
$$

It uses the one-sided limiting values and agrees with the weak-shock expression.

For $U>0$, the right-state [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) travel left with speed $-U$ while the left-state [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) have speed zero. They converge into a compressive [shock wave](../../../partial-differential-equation.md#shock-wave) with speed $-U/2$. The [entropy solution](../../../partial-differential-equation.md#entropy-solution) is

$$
\boxed{f(Z,\theta)=\begin{cases}0,&\theta<-UZ/2,\\U,&\theta>-UZ/2.\end{cases}\quad(U>0).}
$$

The characteristic speeds satisfy $0>-U/2>-U$, so both sides enter the shock.

For $U<0$, right-state [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) travel right with speed $-U>0$, leaving a gap. A steep continuous transition fills that gap with a [rarefaction wave](../../../partial-differential-equation.md#rarefaction-wave). The [entropy solution](../../../partial-differential-equation.md#entropy-solution) is

$$
\boxed{f(Z,\theta)=\begin{cases}0,&\theta<0,\\-\theta/Z,&0<\theta<-UZ,\\U,&\theta>-UZ.\end{cases}\quad(U<0).}
$$

The middle value is fixed by $\theta/Z=F'(f)=-f$. A discontinuity joining the two states would satisfy the jump equation but violate entropy admissibility. If $U=0$, the solution is identically zero.

<a id="3/a/image-characteristics-forming-a-compressive-shock-and-a-rarefaction-fan-for-the-negative-flux-burgers-equation"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-77-burgers-characteristics.png)

**[Figure 1](#3/a/image-characteristics-forming-a-compressive-shock-and-a-rarefaction-fan-for-the-negative-flux-burgers-equation). Characteristics forming a compressive shock and a rarefaction fan for the negative-flux Burgers equation**.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $h=\log\psi$ and $f=2\alpha h_\theta$. Direct substitution into the [viscous Burgers equation](../../../partial-differential-equation.md#viscous-burgers-equation) gives

$$
f_Z-ff_\theta-\alpha f_{\theta\theta}=2\alpha\partial_\theta\left(h_Z-\alpha h_{\theta\theta}-\alpha h_\theta^2\right).
$$

If $\psi_Z=\alpha\psi_{\theta\theta}$, then $h_Z=\alpha(h_{\theta\theta}+h_\theta^2)$, proving the [Cole-Hopf transformation](../../../partial-differential-equation.md#cole-hopf-transformation). A function of $Z$ inside the parentheses can be removed by rescaling $\psi$ by a time-dependent factor, which leaves $f$ unchanged.

For the forward [heat equation](../../../diffusion-equation.md#heat-equation) and the displayed Gaussian kernel we require **$\alpha>0$ and $Z>0$**. The algebraic transformation works for nonzero $\alpha$, but the printed convolution is not a forward solution for negative $\alpha$: its Gaussian then grows and the step-data integral diverges.

Integrating the initial logarithmic derivative fixes a convenient positive initial heat datum,

$$
\psi(0,\phi)=\begin{cases}1,&\phi<0,\\e^{U\phi/(2\alpha)},&\phi>0.\end{cases}
$$

Split the [heat kernel](../../../diffusion-equation.md#heat-kernel) convolution at zero and complete the square in the positive half. With $h_*=U(2\theta+UZ)/(4\alpha)$, put

$$
A_0=\int_\theta^\infty e^{-y^2/(4\alpha Z)}dy,\qquad C_0=\int_{-(\theta+UZ)}^\infty e^{-y^2/(4\alpha Z)}dy.
$$

Then $\psi=(A_0+e^{h_*}C_0)/\sqrt{4\pi\alpha Z}$. On differentiation, the moving-limit terms cancel because $e^{h_*}e^{-(\theta+UZ)^2/(4\alpha Z)}=e^{-\theta^2/(4\alpha Z)}$. Hence

$$
\boxed{f(Z,\theta)=\frac{Ue^{h_*}C_0}{A_0+e^{h_*}C_0}=\frac{U}{1+J e^{-U(2\theta+UZ)/(4\alpha)}},\qquad J=\frac{A_0}{C_0}.}
$$

This is the [viscous Burgers step solution with negative flux](../../../partial-differential-equation.md#viscous-burgers-step-solution-with-negative-flux). Both integrals can be written as $\sqrt{\pi\alpha Z}$ times a [complementary error function](../../../calculus.md#complementary-error-function).

For fixed $Z>0$, the Gaussian-tail asymptotics give **$f\to U$ as $\theta\to+\infty$** and **$f\to0$ as $\theta\to-\infty$**. For example $Je^{-h_*}$ tends to zero on the right with a Gaussian factor $e^{-(\theta+UZ)^2/(4\alpha Z)}$, while on the left it diverges with a Gaussian factor $e^{\theta^2/(4\alpha Z)}$. This holds for either sign of $U$; for $U=0$ the solution is already zero.

The Gaussian tail is strictly decreasing in its lower limit, so $J=1$ occurs exactly at $\theta=-UZ/2$. There $h_*=0$, and **$f=U/2$**. For $U>0$, the two lower limits are both far into the negative tail in the mature shock region, so $J\simeq1$ throughout its thin transition. The solution is then approximately the traveling viscous front

$$
f\simeq\frac U2\left[1+\tanh\frac{U(\theta+UZ/2)}{4\alpha}\right],
$$

centred at the inviscid shock position, with thickness of order $\alpha/U$.

In the [vanishing-viscosity limit](../../../viscous-fluid-flow.md#vanishing-viscosity-limit), for $U>0$ the solution tends to the compressive [entropy solution](../../../partial-differential-equation.md#entropy-solution) of part (a), away from its shock. For $U<0$, it tends instead to the [rarefaction wave](../../../partial-differential-equation.md#rarefaction-wave). To see the latter explicitly inside $0<\theta<-UZ$, both tails have positive lower limits, and their leading asymptotics give $Je^{-h_*}\to(-\theta-UZ)/\theta$. Thus $f\to-\theta/Z$ in the fan, with the constant states outside. Although $J=1$ still marks the fan midpoint, it is not approximately one throughout the expanding fan; replacing it by one there would create an inadmissible compressive-front approximation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
