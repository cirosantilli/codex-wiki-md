# Paper 331

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_331.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_331.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
    - [iv](#1/b/iv)
      - [Solution](#1/b/iv/solution)
    - [v](#1/b/v)
      - [Solution](#1/b/v/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
    - [iv](#3/b/iv)
      - [Solution](#3/b/iv/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Separate the uniform stream and an arbitrary time-dependent gauge from each [velocity potential](../../../fluid-mechanics.md#velocity-potential): $\phi_j=U_jx+f_j(t)+\phi'_j$. Only [gradients](../../../calculus.md#gradient) of the [velocity potential](../../../fluid-mechanics.md#velocity-potential) determine the [velocity field](../../../fluid-mechanics.md#velocity-field). The remote fluid must remain in its unperturbed uniform stream, so

$$
\boxed{\nabla\phi_1\to(U_1,0)\quad(z\to+\infty),\qquad
\nabla\phi_2\to(U_2,0)\quad(z\to-\infty).}
$$

After fixing the harmless gauge, the nonzero-[wavenumber](../../../wave-equation.md#wavenumber) perturbation [velocity potentials](../../../fluid-mechanics.md#velocity-potential) themselves vanish at the corresponding infinities. [Incompressible flow](../../../fluid-mechanics.md#incompressible-flow) and [irrotational flow](../../../fluid-mechanics.md#irrotational-flow) give the [Laplace equation](../../../partial-differential-equation.md#laplace-equation) for each perturbation. For a [normal mode](../../../wave-equation.md#normal-mode) with $k>0$, the vertical amplitude solves $\Phi_j''-k^2\Phi_j=0$, hence

$$
\phi'_1=A_1e^{-kz}e^{ik(x-ct)},\qquad
\phi'_2=A_2e^{kz}e^{ik(x-ct)}.
$$

The opposite exponentials are excluded because they make the perturbation grow at infinity. It is the perturbation, rather than the total potential $U_jx+f_j(t)$, that decays.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Let $F(x,z,t)=z-\eta(x,t)$. The interface is a material surface for both fluids: its [material derivative](../../../continuum-mechanics.md#material-derivative) vanishes on $F=0$. With $u_j=\partial_x\phi_j$ and $w_j=\partial_z\phi_j$, this gives

$$
0=\frac{D_jF}{Dt}=w_j-\partial_t\eta-u_j\partial_x\eta,
\qquad
w_j=\partial_t\eta+u_j\partial_x\eta.
$$

Thus the [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition) says that particles stay on the moving interface. The tangential [velocities](../../../classical-mechanics.md#velocity) can differ; each side has its own [material derivative](../../../continuum-mechanics.md#material-derivative). Replacing both [derivatives](../../../calculus.md#derivative) by one background speed would be incorrect.

The [dynamic boundary condition for an inviscid interface](../../../fluid-mechanics.md#dynamic-boundary-condition-for-an-inviscid-interface) is [pressure continuity](../../../fluid-mechanics.md#pressure-continuity), because the fluids have no viscous normal stress and there is no [surface tension](../../../fluid-mechanics.md#surface-tension). The unsteady [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) in each layer of [irrotational flow](../../../fluid-mechanics.md#irrotational-flow) reads

$$
p_j=\rho_j\left[C_j(t)-\partial_t\phi_j-\frac12|\nabla\phi_j|^2-gz\right].
$$

Equating these pressures at $z=\eta$ gives the required [dynamic boundary condition for an inviscid interface](../../../fluid-mechanics.md#dynamic-boundary-condition-for-an-inviscid-interface). Choose the potential gauges so that $\rho_1C_1=\rho_2C_2$, or set both constants to zero relative to a common reference [pressure](../../../thermodynamics.md#pressure). For example, $\phi_j=U_jx-\tfrac12U_j^2t+\phi'_j$ removes the distinct uniform-stream Bernoulli constants without changing either [velocity](../../../classical-mechanics.md#velocity). **Material-interface kinematics and [pressure continuity](../../../fluid-mechanics.md#pressure-continuity) supply the two matching conditions**, with the Bernoulli gauge understood.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

Use $\phi_j=U_jx-\tfrac12U_j^2t+\phi'_j$ and retain terms linear in the displacement and perturbation potentials. Evaluation at $z=\eta$ may then be replaced by evaluation at $z=0$: the correction to a perturbation is second order. The [kinematic boundary conditions](../../../fluid-mechanics.md#kinematic-boundary-condition) become

$$
\partial_z\phi'_j=(\partial_t+U_j\partial_x)\eta\quad(z=0).
$$

The linearized [pressure continuity](../../../fluid-mechanics.md#pressure-continuity) is

$$
\rho_1(\partial_t+U_1\partial_x)\phi'_1
-\rho_2(\partial_t+U_2\partial_x)\phi'_2
+g(\rho_1-\rho_2)\eta=0.
$$

The decaying [normal modes](../../../wave-equation.md#normal-mode) give $-kA_1=ik(U_1-c)B$ and $kA_2=ik(U_2-c)B$. Thus $A_1=-i(U_1-c)B$, $A_2=i(U_2-c)B$. Substitution into the dynamic condition yields the [Kelvin-Helmholtz dispersion relation with gravity](../../../fluid-mechanics.md#kelvin-helmholtz-dispersion-relation-with-gravity),

$$
\rho_1(U_1-c)^2+\rho_2(U_2-c)^2=\frac{g(\rho_2-\rho_1)}k.
$$

Put $\rho=\rho_1+\rho_2$ and $\overline U=(\rho_1U_1+\rho_2U_2)/\rho$. [Completing the square](../../../polynomial.md#completing-the-square) gives

$$
c=\overline U\pm\sqrt{\frac{g(\rho_2-\rho_1)}{\rho k}
-\frac{\rho_1\rho_2(U_1-U_2)^2}{\rho^2}}.
$$

For $k>0$, the [temporal growth rate](../../../wave-equation.md#growth-rate) is $kc_i$. A growing [complex conjugate](../../../complex-analysis.md#complex-conjugate) branch therefore exists precisely when the radicand of the [square root](../../../algebra.md#square-root) is negative:

$$
\boxed{k>\frac{g(\rho_2^2-\rho_1^2)}{\rho_1\rho_2(U_1-U_2)^2}.}
$$

At equality the two [phase velocities](../../../wave-equation.md#phase-velocity) coincide and there is no exponential growth. Below it the roots describe real [internal gravity waves](../../../gravity-wave.md#internal-wave). The denser lower fluid gives stable [density stratification](../../../gravity-wave.md#density-stratification), but the tangential shear can overcome it. The assumption $U_1\ne U_2$ is needed for the displayed threshold; equal streams have no such shear instability.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Write $\phi'=\Phi(z)e^{ik(x-ct)}$ and let $B_\pm$ be the displacement amplitudes at $z=\pm L$. Use subscripts $I$ for the jet interior and $O$ for the adjoining exterior. Each interface is a material [vortex sheet](../../../fluid-mechanics.md#vortex-sheet), so its linearized [kinematic boundary conditions](../../../fluid-mechanics.md#kinematic-boundary-condition) are

$$
\Phi'_I(\pm L)=ik(V-c)B_\pm,\qquad
\Phi'_O(\pm L)=-ikcB_\pm.
$$

The equal [mass densities](../../../fluid-mechanics.md#density) make the hydrostatic displacement terms cancel. The [dynamic boundary condition for an inviscid interface](../../../fluid-mechanics.md#dynamic-boundary-condition-for-an-inviscid-interface) therefore gives

$$
\boxed{(V-c)\Phi_I(\pm L)=-c\Phi_O(\pm L),\qquad
\frac{\Phi'_I(\pm L)}{V-c}=\frac{\Phi'_O(\pm L)}{-c}=ikB_\pm.}
$$

The division form assumes $c\ne0,V$; the preceding undivided equations remain the proper conditions in those exceptional cases. Potentials themselves need not be continuous, and their vertical [derivatives](../../../calculus.md#derivative) need not be equal: the same material displacement is advected by different tangential base [velocities](../../../classical-mechanics.md#velocity). At infinity the exterior potentials decay. These displacement and [pressure](../../../thermodynamics.md#pressure) conditions, rather than continuity of $\Phi$ and $\Phi'$, determine the [equal-density top-hat planar-jet dispersion relation](../../../fluid-mechanics.md#equal-density-top-hat-planar-jet-dispersion-relation).

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

For an odd [velocity potential](../../../fluid-mechanics.md#velocity-potential), choose

$$
\Phi_I=C\sinh(kz),\qquad
\Phi_O(z)=\begin{cases}Ae^{-k(z-L)},&z>L,\\-Ae^{k(z+L)},&z<-L.\end{cases}
$$

At $z=L$ the two kinematic conditions give $A=icB_+$ and $C\cosh(kL)=i(V-c)B_+$. The dynamic condition is $-cA=(V-c)C\sinh(kL)$. Eliminating $A,C,B_+$ gives, with $s=\tanh(kL)$,

$$
\boxed{c^2=-s(V-c)^2,\qquad
c=\frac{Vs}{1+s}\pm i\frac{|V|\sqrt s}{1+s}.}
$$

The lower interface gives the same equation by odd parity of the [velocity potential](../../../fluid-mechanics.md#velocity-potential). The interior vertical [velocity](../../../classical-mechanics.md#velocity) is even, so $B_-=B_+$: the displacement is a [sinuous mode of a planar jet](../../../fluid-mechanics.md#sinuous-mode-of-a-planar-jet) even though the potential is odd.

For $L>0$, $V\ne0$ and $k>0$, $0<s<1$ and one root has $c_i>0$. Thus **every nonzero [wavenumber](../../../wave-equation.md#wavenumber) is unstable** in this ideal [top-hat planar jet](../../../fluid-mechanics.md#top-hat-planar-jet). The phrase “all choices” is understood with these assumptions: $k=0$ has no exponential wave growth, and $V=0$ has no shear.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

For an even [velocity potential](../../../fluid-mechanics.md#velocity-potential), take $\Phi_I=C\cosh(kz)$ and the decaying exterior amplitudes equal at the upper and lower interfaces. At $z=L$, kinematics gives $A=icB_+$ and $C\sinh(kL)=i(V-c)B_+$. The dynamic condition becomes $-cA=(V-c)C\cosh(kL)$. Therefore

$$
\boxed{c^2=-(V-c)^2\coth(kL).}
$$

Writing $s=\tanh(kL)$, its two roots are

$$
c=\frac{V}{1+s}\pm i\frac{|V|\sqrt s}{1+s}.
$$

The interior vertical [velocity](../../../classical-mechanics.md#velocity) is odd, so $B_-=-B_+$; this is a [varicose mode of a planar jet](../../../fluid-mechanics.md#varicose-mode-of-a-planar-jet). As with the odd potential, $k>0$, finite $L>0$ and $V\ne0$ give a growing root. The parity of the potential and the parity of the interface displacements are opposite because the vertical [velocity](../../../classical-mechanics.md#velocity) is its [derivative](../../../calculus.md#derivative).

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

The odd-potential branch uses $s=\tanh(kL)$, whereas the even-potential branch uses $1/s$. The [imaginary parts](../../../complex-analysis.md#imaginary-part) are identical because

$$
\frac{\sqrt{1/s}}{1+1/s}=\frac{\sqrt s}{1+s}.
$$

Consequently the [equality of top-hat jet parity growth rates](../../../fluid-mechanics.md#equality-of-top-hat-jet-parity-growth-rates) gives

$$
\boxed{\gamma_{\mathrm{odd}}=\gamma_{\mathrm{even}}
=\frac{k|V|\sqrt{\tanh(kL)}}{1+\tanh(kL)}
=\frac{k|V|}{2}\sqrt{1-e^{-4kL}}.}
$$

Here $\gamma=kc_i$ is the positive [temporal growth rate](../../../wave-equation.md#growth-rate). The real [phase velocities](../../../wave-equation.md#phase-velocity) differ: $c_{r,\mathrm{odd}}=\tfrac V2(1-e^{-2kL})$ and $c_{r,\mathrm{even}}=\tfrac V2(1+e^{-2kL})$. Thus equal amplification does not imply equal propagation. As $kL\to\infty$, both approach the isolated-[vortex sheet](../../../fluid-mechanics.md#vortex-sheet) [phase velocity](../../../wave-equation.md#phase-velocity) $V/2$ and [growth rate](../../../wave-equation.md#growth-rate) $k|V|/2$.

<h4 id="1/b/v">v</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/v/solution">Solution</h5>

↑ **Parent:** [V](#1/b/v)

For a single equal-density [vortex sheet](../../../fluid-mechanics.md#vortex-sheet) with stream speeds $0$ and $V$, the gravitational contribution vanishes. The [Kelvin-Helmholtz dispersion relation with gravity](../../../fluid-mechanics.md#kelvin-helmholtz-dispersion-relation-with-gravity) reduces to $c^2+(V-c)^2=0$, with roots $c=V/2\pm i|V|/2$. Its positive [temporal growth rate](../../../wave-equation.md#growth-rate) is $\gamma_{\mathrm{sheet}}=k|V|/2$.

Both jet parity branches have the common [growth rate](../../../wave-equation.md#growth-rate) derived above, hence

$$
\boxed{\frac{\gamma_{\mathrm{jet}}}{\gamma_{\mathrm{sheet}}}
=\sqrt{1-e^{-4kL}}<1\quad(0<kL<\infty,\ V\ne0).}
$$

Equivalently, $2\sqrt s\leq1+s$ follows from $(\sqrt s-1)^2\geq0$. Equality is approached when the two interfaces are separated by many disturbance decay lengths, $kL\to\infty$. The zero-shear case has both [growth rates](../../../wave-equation.md#growth-rate) zero. For small $kL$, the [growth rate](../../../wave-equation.md#growth-rate) ratio is approximately $2\sqrt{kL}$: interaction between the sheets suppresses amplification relative to an isolated sheet.

## 2

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $D=\overline U-c$ and $F=\widehat w/D^{1/2}$. For $c_i>0$, $D$ never vanishes, so an [analytic branch of a square root](../../../analysis.md#analytic-branch-of-a-square-root) exists along the real flow domain. Take real smooth [velocity](../../../classical-mechanics.md#velocity) and [buoyancy frequency](../../../gravity-wave.md#buoyancy-frequency) coefficients, nonzero $k$ (chosen positive for the growing-wave convention), a nontrivial regular [normal mode](../../../wave-equation.md#normal-mode), and boundary decay strong enough to remove the integration-by-parts term.

Substitution into the [Taylor–Goldstein equation](../../../gravity-wave.md#taylor-goldstein-equation) gives the half-power case of the [power-transformed Taylor–Goldstein energy identity](../../../gravity-wave.md#power-transformed-taylor-goldstein-energy-identity):

$$
(D F')'-k^2DF-\frac12\overline U''F
+\frac{S}{D}F=0,\qquad
S=N^2-\frac14(\overline U')^2.
$$

For completeness, differentiating $\widehat w=D^{1/2}F$ yields $\widehat w''=D^{1/2}F''+\overline U'D^{-1/2}F'+[\tfrac12\overline U''D^{-1/2}-\tfrac14(\overline U')^2D^{-3/2}]F$, which explains the coefficient $1/4$.

Multiply by $F^*$ and integrate over $z$. The boundary term $[F^*DF']$ is zero for the given homogeneous endpoint conditions, or for sufficiently decaying finite-energy modes at infinity. Therefore

$$
\int\left[D(|F'|^2+k^2|F|^2)+\frac12\overline U''|F|^2
-\frac{S}{D}|F|^2\right]dz=0.
$$

Since $\operatorname{Im}D=-c_i$, $\operatorname{Im}(1/D)=c_i/|D|^2$, and $S,\overline U''$ are real, taking the [imaginary part](../../../complex-analysis.md#imaginary-part) and dividing by $-c_i$ gives

$$
\int\left[|F'|^2+k^2|F|^2+\frac{S}{|D|^2}|F|^2\right]dz=0.
$$

The first two terms have strictly positive [integral](../../../calculus.md#integral) for a nonzero mode. Thus $S$ cannot be nonnegative everywhere:

$$
\boxed{N^2-\frac14(\overline U')^2<0\quad\text{somewhere}.}
$$

This proves the [Miles–Howard theorem](../../../gravity-wave.md#miles-howard-theorem) in contrapositive form. Where $\overline U'\ne0$, the corresponding [gradient Richardson number](../../../gravity-wave.md#gradient-richardson-number) must fall below $1/4$ somewhere. Failure of this sufficient-stability criterion does not prove instability. The derivation uses $c_i>0$; it cannot be applied unchanged to a neutral singular critical layer.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Set $y=\tanh z$ and $a=1-k$, so $dy/dz=1-y^2$ and $\widehat w=(1-y^2)^{k/2}y^a$. Away from $y=0$, the [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) gives

$$
\frac{\widehat w'}{\widehat w}=\frac ay-y,\qquad
\frac{\widehat w''}{\widehat w}=\frac{a(a-1)}{y^2}-a-1+2y^2.
$$

For $c=0$, $\overline U''/\overline U=-2(1-y^2)$ and $N^2/\overline U^2=J(1-y^2)/y^2$. The [Taylor–Goldstein equation](../../../gravity-wave.md#taylor-goldstein-equation) residual divided by $\widehat w$ consequently simplifies to

$$
[J-k(1-k)]\left(\frac1{y^2}-1\right).
$$

Thus the [neutral mode of the equal-width Hazel model](../../../hydrodynamic-stability.md#neutral-mode-of-the-equal-width-hazel-model) requires

$$
\boxed{J=k(1-k).}
$$

The qualifier “solution” needs care at the [critical level of an internal gravity wave](../../../gravity-wave.md#critical-level-of-an-internal-gravity-wave) $z=0$. For $0<k<1$, $\widehat w\sim z^{1-k}$ and $\widehat w'\sim(1-k)z^{-k}$: it is a solution separately on either side, not a classical smooth [eigenfunction](../../../linear-operator-theory.md#eigenfunction) across the [critical level of an internal gravity wave](../../../gravity-wave.md#critical-level-of-an-internal-gravity-wave). A branch for negative $\tanh z$ is also needed. For example, a limit from $c_i>0$ assigns $(\tanh z)^{1-k}=|\tanh z|^{1-k}e^{-i\pi(1-k)}$ on $z<0$.

The [critical-layer regularity of a neutral Hazel mode](../../../hydrodynamic-stability.md#critical-layer-regularity-of-a-neutral-hazel-mode) further gives local finite horizontal [kinetic energy](../../../classical-mechanics.md#kinetic-energy) only for $0<k<1/2$, since [incompressible flow](../../../fluid-mechanics.md#incompressible-flow) gives $\widehat u=i\widehat w'/k$ and $\int_0^\epsilon z^{-2k}dz$ then converges. At $k=1$, $J=0$ and $\widehat w=\operatorname{sech}z$ is smooth after the removable $\overline U''/\overline U$ quotient is continued. At $k=0$, $J=0$ and the formal $\tanh z$ profile does not decay at infinity, so it fails the remote endpoint condition. These qualifications prevent interpreting the whole closed parameter interval as a family of classical decaying modes.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

For the equal-width [Hazel model](../../../hydrodynamic-stability.md#hazel-model) with stable [density stratification](../../../gravity-wave.md#density-stratification) $J\geq0$,

$$
\mathrm{Ri}(z)=\frac{N^2}{(\overline U')^2}
=J\cosh^2z,\qquad \min_z\mathrm{Ri}(z)=J.
$$

The [Miles–Howard theorem](../../../gravity-wave.md#miles-howard-theorem) therefore excludes exponentially growing regular [normal modes](../../../wave-equation.md#normal-mode) for $J\geq1/4$. The candidate [neutral modes of the equal-width Hazel model](../../../hydrodynamic-stability.md#neutral-mode-of-the-equal-width-hazel-model) instead lie on

$$
\boxed{J=k(1-k)\leq\frac14,\qquad \max J=\frac14\text{ at }k=\frac12.}
$$

The parabola touches the sufficient-stability threshold at its maximum. There is no contradiction: neutrality has $c_i=0$, whereas the proof in part (a) assumes $c_i>0$. Moreover, the $k=1/2$ profile has a singular critical-layer [derivative](../../../calculus.md#derivative) and logarithmically divergent horizontal [kinetic energy](../../../classical-mechanics.md#kinetic-energy); it is not a regular growing mode satisfying the proof's hypotheses.

For $J<1/4$, the local [gradient Richardson number](../../../gravity-wave.md#gradient-richardson-number) condition permits instability but does not establish it. Substitution of a neutral ansatz alone also does not determine on which side of the curve unstable eigenvalues lie. It identifies the formal neutral curve; concluding a full stability boundary requires additional continuation analysis of the [eigenvalues](../../../linear-operator-theory.md#eigenvalue). The nondecaying $k=0$ endpoint and the smooth $k=1,J=0$ endpoint have the distinct qualifications described above.

## 3

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Take the physical coefficients $U,\mu,c_d$ real. Substitution of $e^{i(kx-\omega t)}$ into the [linear complex Ginzburg-Landau equation](../../../partial-differential-equation.md#linear-complex-ginzburg-landau-equation) gives $-i\omega+ikU-\mu+(1+ic_d)k^2=0$, hence

$$
\omega=Uk+(c_d-i)k^2+i\mu.
$$

Let $A=c_d-i$. [Completing the square](../../../polynomial.md#completing-the-square) yields $\omega=A(k+U/(2A))^2+i\mu-U^2/(4A)$. Therefore the [absolute wavenumber](../../../hydrodynamic-stability.md#absolute-wavenumber) and [absolute frequency](../../../hydrodynamic-stability.md#absolute-frequency) are

$$
\boxed{k_0=-\frac{U}{2(c_d-i)},\qquad
\omega_0=i\mu-\frac{U^2}{4(c_d-i)}.}
$$

Their explicitly separated parts are

$$
k_0=-\frac{U(c_d+i)}{2(1+c_d^2)},\qquad
\omega_0=-\frac{U^2c_d}{4(1+c_d^2)}
+i\left[\mu-\frac{U^2}{4(1+c_d^2)}\right].
$$

Thus $d\omega/dk=U+2(c_d-i)k$ vanishes at $k_0$. The complex saddle describes the localized [Green function](../../../analysis.md#green-s-function) response; it is different from selecting a real [wavenumber](../../../wave-equation.md#wavenumber) for a [Fourier mode](../../../fourier-analysis.md#fourier-mode) for temporal amplification.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

At the [absolute wavenumber](../../../hydrodynamic-stability.md#absolute-wavenumber), the [group velocity](../../../wave-equation.md#group-velocity) $d\omega/dk$ is zero. The corresponding accessible saddle therefore governs the disturbance seen at a fixed position. Its exponential [growth rate](../../../wave-equation.md#growth-rate) is

$$
\operatorname{Im}\omega_0=\mu-\frac{U^2}{4(1+c_d^2)}.
$$

Saddle accessibility can be checked directly here. With $D=1+ic_d$, whose [real part](../../../complex-analysis.md#real-part) is positive, [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) gives the [Green function of the linear complex Ginzburg-Landau equation](../../../partial-differential-equation.md#green-function-of-the-linear-complex-ginzburg-landau-equation),

$$
G(x,t)=\frac1{\sqrt{4\pi Dt}}
\exp\left[\mu t-\frac{(x-Ut)^2}{4Dt}\right],\qquad t>0.
$$

At fixed $x$ its exponential rate is $\operatorname{Im}\omega_0$, while along the packet centre $x=Ut$ it is $\mu$. For real [wavenumbers](../../../wave-equation.md#wavenumber) of [Fourier modes](../../../fourier-analysis.md#fourier-mode), the [temporal growth rate](../../../wave-equation.md#growth-rate) is $\operatorname{Im}\omega(k)=\mu-k^2$, so the flow is temporally unstable exactly when $\mu>0$.

Consequently the classifications for a localized disturbance in this laboratory frame are

$$
\boxed{\begin{aligned}
0<\mu<\frac{U^2}{4(1+c_d^2)}&:\ \text{convective instability},\\
\mu>\frac{U^2}{4(1+c_d^2)}&:\ \text{absolute instability}.
\end{aligned}}
$$

For [convective hydrodynamic instability](../../../hydrodynamic-stability.md#convective-hydrodynamic-instability), a travelling [wave packet](../../../wave-equation.md#wave-packet) amplifies but the response at each fixed position decays. For [absolute hydrodynamic instability](../../../hydrodynamic-stability.md#absolute-hydrodynamic-instability), that fixed-position response amplifies. The equality is the marginal absolute threshold: its exponential rate is zero and the impulse response has a $t^{-1/2}$ prefactor. For $\mu<0$ there is no temporal growth; $\mu=0$ is temporally marginal. When $U=0$ the convective window is empty. These conclusions use the infinite-line impulse problem; a general [dispersion relation](../../../wave-equation.md#dispersion-relation) requires its own spatial-branch or saddle selection.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

For this nonlinear ansatz, take $k$ real as well as $U,\mu$ real. Then $|e^{ik(x-Ut)}|=1$, and the advective time [derivative](../../../calculus.md#derivative) vanishes. Substitution into the [nonlinear Ginzburg-Landau equation](../../../partial-differential-equation.md#nonlinear-ginzburg-landau-equation) gives

$$
0=(\mu-k^2)Q-Q^3.
$$

The stipulated positive-amplitude [Ginzburg-Landau plane wave](../../../partial-differential-equation.md#ginzburg-landau-plane-wave) therefore has

$$
\boxed{Q=\sqrt{\mu-k^2}.}
$$

The strict inequality $\mu>k^2$ guarantees that this is real and positive. The zero solution of the [nonlinear Ginzburg-Landau equation](../../../partial-differential-equation.md#nonlinear-ginzburg-landau-equation) also exists but is not the required positive wave. Although complex $k$ is useful in the linear impulse analysis, it cannot generally be carried into this constant-amplitude nonlinear ansatz: its spatially varying modulus would make the cubic term carry a different spatial factor.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Put $a=\mu-k^2=Q^2>0$. The shared travelling phase again cancels [advection](../../../fluid-mechanics.md#advection) in the [nonlinear Ginzburg-Landau equation](../../../partial-differential-equation.md#nonlinear-ginzburg-landau-equation); the remaining amplitude [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) is

$$
R'=aR-R^3.
$$

For $R>0$, $Y=R^2$ obeys the [logistic differential equation](../../../differential-equation.md#logistic-differential-equation) $Y'=2Y(a-Y)$. Equivalently, $Z=1/Y$ solves $Z'=-2aZ+2$, whence $Z(t)=a^{-1}+(R_0^{-2}-a^{-1})e^{-2at}$. The nonconstant [cubic amplitude saturation](../../../partial-differential-equation.md#cubic-amplitude-saturation) solution is

$$
\boxed{R(t)=\frac{Q}{\sqrt{1+\left(Q^2/R_0^2-1\right)e^{-2Q^2t}}},\qquad t\geq0.}
$$

It takes the specified $R_0$ at $t=0$. The denominator of the [cubic amplitude saturation](../../../partial-differential-equation.md#cubic-amplitude-saturation) solution remains positive for all future time: if $R_0<Q$ its bracket exceeds one, and if $R_0>Q$ it lies between $Q^2/R_0^2$ and one. Thus the positive solution is global forward in time. $R_0=Q$ would give the excluded constant solution; $R_0=0$ would remain at zero rather than relax to the positive wave.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

The [cubic amplitude saturation](../../../partial-differential-equation.md#cubic-amplitude-saturation) equation $R'=R(Q^2-R^2)$ and the [Picard-Lindelöf theorem](../../../differential-equation.md#picard-lindelof-theorem) imply that positive solutions cannot cross the equilibrium $Q$. If $0<R_0<Q$, then $R$ stays below $Q$ and increases. If $R_0>Q$, then it stays above $Q$ and decreases. The explicit [cubic amplitude saturation](../../../partial-differential-equation.md#cubic-amplitude-saturation) solution tends to $Q$ in both cases, so

$$
\boxed{|\psi_R(x,t)-\psi_S(x,t)|=|R(t)-Q|\downarrow0.}
$$

The same relation makes the distance a decreasing [monotone function](../../../calculus.md#monotonic-function) in any spatial [norm](../../../functional-analysis.md#norm) for which the plane wave has finite norm, for example on a periodic domain. At large time, $R-Q\sim-\tfrac Q2(Q^2/R_0^2-1)e^{-2Q^2t}$.

The printed monotonicity wording must be interpreted as **monotone amplitude relaxation, or monotone decay of the distance between the waves**. [Complex numbers](../../../complex-analysis.md#complex-number) have no ordinary monotone ordering, and the [real part](../../../complex-analysis.md#real-part) at a fixed point can oscillate. For instance, $k=U=1$, $\mu=2$ and $R_0=1/2$ give $\operatorname{Re}\psi_R(0,t)=R(t)\cos t$, which is not monotone despite the monotone amplitude. This result concerns the common-phase single-mode family, not stability against arbitrary spatial perturbations.

<h4 id="3/b/iv">iv</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/b/iv)

When $R\ll Q$, the ratio of cubic damping to linear amplification is $R^2/Q^2\ll1$. The [cubic amplitude saturation](../../../partial-differential-equation.md#cubic-amplitude-saturation) equation therefore gives

$$
\frac{R'}R=Q^2-R^2\simeq Q^2=\mu-k^2,
\qquad
R(t)\simeq R(t_0)e^{(\mu-k^2)(t-t_0)}
$$

while the small-amplitude regime lasts. With $c_d=0$, the matching real-[wavenumber](../../../wave-equation.md#wavenumber) [normal mode](../../../wave-equation.md#normal-mode) of the [linear complex Ginzburg-Landau equation](../../../partial-differential-equation.md#linear-complex-ginzburg-landau-equation) has $\omega=Uk+i(\mu-k^2)$ and hence amplitude proportional to $e^{(\mu-k^2)t}$. Thus

$$
\boxed{\gamma_{\mathrm{small\ amplitude}}=\gamma_{\mathrm{linear\ Fourier\ mode}}=\mu-k^2.}
$$

This is the [temporal growth rate](../../../wave-equation.md#growth-rate) of the same Fourier component. It is not the fixed-position [absolute frequency](../../../hydrodynamic-stability.md#absolute-frequency) rate $\mu-U^2/4$ of a localized impulse. Nonlinear damping becomes important when $R$ is comparable with $Q$ and then arrests exponential amplification.

## 4

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use $\nu=Re^{-1}>0$, $\kappa=Pe^{-1}>0$, $\mathbf U=\overline{\mathbf u}+\mathbf u$, and $\Theta=\overline\theta+\theta$. Work along a sufficiently regular direct trajectory satisfying the given constraints. The zero spatial mean of the [scalar field](../../../quantum-field-theory.md#scalar-field) is conserved by [incompressible flow](../../../fluid-mechanics.md#incompressible-flow), impermeable walls and zero scalar flux, so minimizing $J=(\Theta(T),\Theta(T))$ is equivalent to minimizing [scalar variance](../../../fluid-mechanics.md#scalar-variance), up to the fixed domain volume.

The printed functional fixes the initial state to a candidate $\mathbf u_0$; it contains no term that enforces its [kinetic energy](../../../classical-mechanics.md#kinetic-energy). For the optimization over that candidate, add the real [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) constraint

$$
\mathcal L_E=\mathcal L-\lambda\left[\frac12(\mathbf u_0,\mathbf u_0)-E_0\right].
$$

Equivalently, one can restrict all control variations to the [sphere in a normed vector space](../../../functional-analysis.md#sphere-in-a-normed-vector-space) of fixed [kinetic energy](../../../classical-mechanics.md#kinetic-energy). This term changes the initial-control optimality condition, not the interior adjoint equations.

Let $\mathbf v=\delta\mathbf u$, $\sigma=\delta\theta$ and $\pi=\delta p$. [Linearization](../../../algebra.md#linearization) of the momentum and [scalar transport](../../../fluid-mechanics.md#scalar-transport) residuals gives

$$
\delta F_u=\partial_t\mathbf v+\mathbf U\cdot\nabla\mathbf v
+\mathbf v\cdot\nabla\mathbf U+Ri_B\sigma\hat{\mathbf y}
+\nabla\pi-\nu\Delta\mathbf v,
$$



$$
\delta F_\theta=\partial_t\sigma+\mathbf U\cdot\nabla\sigma
+\mathbf v\cdot\nabla\Theta-\kappa\Delta\sigma.
$$

Both appearances of the perturbation [velocity](../../../classical-mechanics.md#velocity) in the nonlinear momentum term have been differentiated. In particular, the coefficient is the [gradient](../../../calculus.md#gradient) of the total [velocity](../../../classical-mechanics.md#velocity), not just the base shear.

For the negative-constraint convention of the functional, [integration by parts](../../../calculus.md#integration-by-parts) gives the interior coefficients of $\mathbf v,\sigma,\pi$ as

$$
\begin{aligned}
A_u&=\partial_t\mathbf u^\dagger+\mathbf U\cdot\nabla\mathbf u^\dagger
-(\nabla\mathbf U)^T\mathbf u^\dagger+\nabla p^\dagger
+\nu\Delta\mathbf u^\dagger-\theta^\dagger\nabla\Theta,\\
A_\theta&=\partial_t\theta^\dagger+\mathbf U\cdot\nabla\theta^\dagger
+\kappa\Delta\theta^\dagger-Ri_Bu_y^\dagger,\\
A_p&=\nabla\cdot\mathbf u^\dagger.
\end{aligned}
$$

Thus the [adjoint equations for Boussinesq scalar mixing](../../../fluid-mechanics.md#adjoint-equations-for-boussinesq-scalar-mixing) are

$$
\boxed{A_u=0,\qquad A_\theta=0,\qquad \nabla\cdot\mathbf u^\dagger=0.}
$$

The transpose is essential: the $j$th component of $(\nabla\mathbf U)^T\mathbf u^\dagger$ is $\sum_i u_i^\dagger\partial_jU_i$. The coupling $-\theta^\dagger\nabla\Theta$ transposes advection of the scalar by a [velocity](../../../classical-mechanics.md#velocity) perturbation; $-Ri_Bu_y^\dagger$ transposes [buoyancy](../../../fluid-mechanics.md#buoyancy) feedback. Dropping the latter would give a [passive scalar](../../../fluid-mechanics.md#passive-scalar) adjoint, not the [active scalar](../../../fluid-mechanics.md#active-scalar) problem.

These equations are integrated backward, not forward. If $\tau=T-t$, they read

$$
\partial_\tau\mathbf u^\dagger=\mathbf U\cdot\nabla\mathbf u^\dagger
-(\nabla\mathbf U)^T\mathbf u^\dagger+\nabla p^\dagger
+\nu\Delta\mathbf u^\dagger-\theta^\dagger\nabla\Theta,
$$



$$
\partial_\tau\theta^\dagger=\mathbf U\cdot\nabla\theta^\dagger
+\kappa\Delta\theta^\dagger-Ri_Bu_y^\dagger,
$$

with direct coefficients evaluated at $t=T-\tau$. Both terms from the [diffusion equation](../../../diffusion-equation.md) now have the usual forward sign in $\tau$. A [direct-adjoint looping](../../../control-theory.md#direct-adjoint-looping) method stores or reconstructs the forward trajectory, solves these equations backward, and uses the initial adjoint as the control [gradient](../../../calculus.md#gradient). The endpoint and fixed-energy conditions below give necessary conditions for a local optimizer, not a global optimality theorem.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The temporal [integration by parts](../../../calculus.md#integration-by-parts) terms are

$$
-[\,(\mathbf u^\dagger,\delta\mathbf u)+(\theta^\dagger,\delta\theta)\,]_0^T
-(\mathbf u_0^\dagger,\delta\mathbf u(0)-\delta\mathbf u_0)
+2(\Theta(T),\delta\theta(T)).
$$

The terminal states are free and the objective has no explicit terminal-[velocity](../../../classical-mechanics.md#velocity) dependence. Therefore

$$
\boxed{\mathbf u^\dagger(T)=\mathbf0,\qquad
\theta^\dagger(T)=2\Theta(T).}
$$

The factor two follows from the displayed objective without a $1/2$ prefactor. The initial [scalar field](../../../quantum-field-theory.md#scalar-field) perturbation is fixed, so $\delta\theta(0)=0$ and there is no independently prescribed adjoint-scalar condition at $t=0$. Its value there is obtained by backward integration. Independent variation of the initial [velocity](../../../classical-mechanics.md#velocity) state gives $\mathbf u^\dagger(0)=\mathbf u_0^\dagger$.

Variation of the candidate $\mathbf u_0$ in the energy-augmented functional gives the [fixed-energy initial-condition optimality](../../../control-theory.md#fixed-energy-initial-condition-optimality) condition. For the usual divergence-free no-slip control space $H$, write $P_H$ for its [orthogonal projection](../../../hilbert-space.md#orthogonal-projection), the [Leray-Helmholtz projection](../../../viscous-fluid-flow.md#leray-helmholtz-projection) in the usual incompressible [velocity](../../../classical-mechanics.md#velocity) space. This is the standard formal control condition when [pressure](../../../thermodynamics.md#pressure) is determined by [incompressible flow](../../../fluid-mechanics.md#incompressible-flow) and normal momentum. If the independently imposed direct [pressure](../../../thermodynamics.md#pressure) flux is retained as an additional constraint, the admissible control variations must also satisfy its compatibility conditions along the trajectory; they need not fill the usual space $H$. The standard projection formula alone does not prove stationarity for that more restricted problem. Then

$$
\boxed{P_H\mathbf u^\dagger(0)=\lambda\mathbf u_0,\qquad
\frac12\|\mathbf u_0\|^2=E_0.}
$$

For the natural solenoidal adjoint space, $P_H\mathbf u^\dagger(0)=\mathbf u^\dagger(0)$. Equivalently, its component tangent to the [sphere in a normed vector space](../../../functional-analysis.md#sphere-in-a-normed-vector-space) of fixed [kinetic energy](../../../classical-mechanics.md#kinetic-energy) vanishes:

$$
g_{\mathrm{tan}}=P_H\mathbf u^\dagger(0)
-\frac{(P_H\mathbf u^\dagger(0),\mathbf u_0)}{2E_0}\mathbf u_0=0.
$$

Here $E_0>0$ is needed for the [sphere in a normed vector space](../../../functional-analysis.md#sphere-in-a-normed-vector-space) to be regular and for division by $2E_0$. The multiplier is real and can have either sign; normalizing the initial adjoint with a prescribed positive sign is not a general necessary condition for minimization. If $E_0=0$, the only feasible initial [velocity](../../../classical-mechanics.md#velocity) is zero and this tangent formula for the [sphere in a normed vector space](../../../functional-analysis.md#sphere-in-a-normed-vector-space) is inapplicable. First-order stationarity alone also allows maxima or saddles; a local minimum requires the appropriate nonnegative constrained second variation.

The spatial boundary terms vanish with periodic adjoints in $x,z$, homogeneous [no-slip boundary conditions](../../../viscous-fluid-flow.md#no-slip-boundary-condition) $\mathbf u^\dagger=0$ at $y=\pm1$, and $\partial_y\theta^\dagger=0$ there. To see this, [velocity](../../../classical-mechanics.md#velocity) variations vanish at the wall while their normal [derivatives](../../../calculus.md#derivative) need not, so the viscous boundary term forces the adjoint [velocity](../../../classical-mechanics.md#velocity) to vanish. Scalar variations have zero normal [derivative](../../../calculus.md#derivative) but free values, forcing the adjoint scalar's normal [derivative](../../../calculus.md#derivative) to vanish. Pressure variation gives adjoint [incompressible flow](../../../fluid-mechanics.md#incompressible-flow); no independent terminal or initial datum is assigned to $p^\dagger$. Its additive time-dependent constant may be fixed by a zero spatial mean.

In particular, a homogeneous Neumann condition for the direct [pressure](../../../thermodynamics.md#pressure) does not by variational transposition require $\partial_yp^\dagger=0$. For a smooth adjoint solution, the wall-normal adjoint momentum equation instead supplies

$$
\partial_yp^\dagger=-\nu\Delta u_y^\dagger
$$

at the flat walls, because the direct scalar normal [derivative](../../../calculus.md#derivative) is zero there. A zero adjoint-[pressure](../../../thermodynamics.md#pressure) [derivative](../../../calculus.md#derivative) would be an additional compatibility choice, valid only when this right-hand side vanishes.

There are also literal direct-data compatibility qualifications in the printed setup. The initial total [scalar field](../../../quantum-field-theory.md#scalar-field) is $\overline\theta=-\operatorname{erf}(30y)$, whose wall [derivative](../../../calculus.md#derivative) is $-60e^{-900}/\sqrt\pi\ne0$. It is extraordinarily small but mathematically not zero. Thus exact initial scalar data and exact zero wall flux are incompatible for a classical solution smooth at $t=0$. One may use a parabolic [mild solution of an abstract Cauchy problem](../../../functional-analysis.md#mild-solution-of-an-abstract-cauchy-problem) with the boundary condition enforced for $t>0$, or replace the initial profile by an exactly compatible smooth one; these are conventions, not an equality $e^{-900}=0$. The reference [scalar field](../../../quantum-field-theory.md#scalar-field) is also not a stationary profile of the [diffusion equation](../../../diffusion-equation.md) at finite $Pe$: the full $\Delta\Theta$ term must be retained.

The [pressure compatibility at a no-slip wall](../../../viscous-fluid-flow.md#pressure-compatibility-at-a-no-slip-wall) is similarly important. Direct normal momentum gives $\partial_yp=\nu\Delta u_y-Ri_B\theta$. The separately imposed zero [pressure](../../../thermodynamics.md#pressure) [derivative](../../../calculus.md#derivative) requires this right side to vanish. It is not automatic for arbitrary fixed-energy initial [velocities](../../../classical-mechanics.md#velocity). For example, the divergence-free no-slip field generated by the periodic [stream function](../../../fluid-mechanics.md#stream-function) $S=A(1-y^2)^2\sin(\alpha x)$ with $\alpha=\pi/L_x>0$ has $u_x=\partial_yS$, $u_y=-\partial_xS$ and $\Delta u_y|_{y=\pm1}=-8A\alpha\cos(\alpha x)\ne0$, while $\theta(0)=0$. With $A\ne0$ adjusted to any positive energy, no classical solution smooth up to the initial wall can satisfy that extra [pressure](../../../thermodynamics.md#pressure) condition. The displayed adjoints are the formal necessary equations along admissible smooth trajectories; a well-posed physical formulation normally determines [pressure](../../../thermodynamics.md#pressure) from [incompressible flow](../../../fluid-mechanics.md#incompressible-flow) and normal momentum, rather than imposing independent homogeneous [pressure](../../../thermodynamics.md#pressure) flux for every control.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
