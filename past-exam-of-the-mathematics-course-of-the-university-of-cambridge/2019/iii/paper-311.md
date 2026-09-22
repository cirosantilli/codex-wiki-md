# Paper 311

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_311.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_311.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
    - [iv](#1/b/iv)
      - [Solution](#1/b/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

An isolated collapse emits transient matter and [gravitational waves](../../../general-relativity.md#gravitational-wave). The exterior is expected to settle to an asymptotically flat [stationary spacetime](../../../general-relativity.md#stationary-spacetime). Because the star is uncharged, the [black-hole uniqueness theorem](../../../general-relativity.md#black-hole-uniqueness-theorem) identifies the regular final state with a [Kerr black hole](../../../general-relativity.md#kerr-black-hole). Its higher [multipole moments](../../../physics.md#multipole-moment) are fixed by its conserved charges: the [black-hole no-hair theorem](../../../general-relativity.md#black-hole-no-hair-theorem) leaves only the total [mass](../../../classical-mechanics.md#mass) $M$ and [angular momentum](../../../classical-mechanics.md#angular-momentum) $J$. Thus **the late-time spacetime is characterized by $M$ and $J$**.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Factor

$$
f(r)=\left(1-\frac{r_+^2}{r^2}\right)\left(1-\frac{r_-^2}{r^2}\right),
\qquad r_\pm^2=M\pm\sqrt{M^2-Q^2}.
$$

Introduce $v=t+r_*$ with $dr_*/dr=f^{-1}$. Since $dt=dv-dr/f$,

$$
\boxed{ds^2=-f(r)\,dv^2+2\,dv\,dr+r^2d\Omega_3^2},
\qquad d\Omega_3^2=d\theta^2+\sin^2\theta\,d\phi^2+\cos^2\theta\,d\psi^2.
$$

These are the charged analogue of [Ingoing Eddington-Finkelstein coordinates](../../../general-relativity.md#ingoing-eddington-finkelstein-coordinates). The $(v,r)$ block has determinant $-1$, so the metric and its inverse are nonsingular at $r=r_+$. For $M\geq Q$, $r_+$ is real and the metric extends analytically through it. The original potential becomes $A=-Q\,dv/r^2+Q\,dr/(r^2f)$; the radial term is locally exact, and a [gauge transformation](../../../electromagnetism.md#gauge-transformation) gives the horizon-regular potential $A=-Q\,dv/r^2$.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The stationary [Killing vector field](../../../general-relativity.md#killing-vector-field) is $k=\partial_t=\partial_v$, with $k^2=-f$. The normal to $r=\text{constant}$ has squared norm $g^{rr}=f$, so $r=r_+$ is a [null hypersurface](../../../general-relativity.md#null-hypersurface); there $k$ is both tangent and normal. It is therefore a [Killing horizon](../../../general-relativity.md#killing-horizon).

For a static metric of this form, the [surface gravity](../../../general-relativity.md#surface-gravity) is $\kappa=f'(r_+)/2$. Since $r_+^2r_-^2=Q^2$ and $r_+^2+r_-^2=2M$,

$$
\boxed{\kappa=\frac{r_+^2-r_-^2}{r_+^3}=\frac{2\sqrt{M^2-Q^2}}{r_+^3}}.
$$

For the [extremal black hole](../../../general-relativity.md#extremal-black-hole) $M=Q$, the horizons coincide and **$\kappa=0$**.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The zeros of $f$ give three causal structures.

- If $M>Q$, there are two simple horizons $r_+>r_->0$. The maximally extended [Penrose diagram](../../../general-relativity.md#penrose-diagram) is the repeating subextremal charged-black-hole diagram: $r=r_+$ is an [event horizon](../../../general-relativity.md#event-horizon), $r=r_-$ is a [Cauchy horizon](../../../general-relativity.md#cauchy-horizon), and $r=0$ is a timelike singularity.
- If $M=Q$, the roots coincide. The extremal diagram has one degenerate horizon, no bifurcation surface, and an infinite throat between the exterior and interior.
- If $M<Q$, $f$ has no real zero. The timelike $r=0$ singularity is visible from infinity, so there is a [naked singularity](../../../general-relativity.md#naked-singularity) and no black-hole region.

Thus **the cases are subextremal, extremal, and overextremal according as $M>Q$, $M=Q$, and $M<Q$**.

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

For this [charged scalar field](../../../quantum-field-theory.md#charged-scalar-field), $\sqrt{-g}=r^3\sin\theta\cos\theta$. On $e^{-i\omega t}$, the [gauge-covariant derivative of a charged scalar field](../../../quantum-field-theory.md#gauge-covariant-derivative-of-a-charged-scalar-field) supplies the shifted frequency

$$
\omega+qA_t=\omega-\frac{qQ}{r^2}.
$$

The wave equation becomes

$$
\frac1{r^3}\frac{d}{dr}\left(r^3f\frac{dR}{dr}\right)+\frac{(\omega-qQ/r^2)^2}{f}R
+\frac{R}{r^2\Theta\sin\theta\cos\theta}\frac{d}{d\theta}\left(\sin\theta\cos\theta\frac{d\Theta}{d\theta}\right)=0.
$$

[Separation of variables](../../../partial-differential-equation.md#separation-of-variables) with constant $\lambda$ gives

$$
\boxed{\frac1{\sin\theta\cos\theta}\frac{d}{d\theta}\left(\sin\theta\cos\theta\frac{d\Theta}{d\theta}\right)+\lambda\Theta=0}
$$

and

$$
\boxed{\frac1{r^3}\frac{d}{dr}\left(r^3f\frac{dR}{dr}\right)+\left[\frac{(\omega-qQ/r^2)^2}{f}-\frac{\lambda}{r^2}\right]R=0}.
$$

The angular equation is the axisymmetric [spherical harmonic](../../../analysis.md#spherical-harmonic) equation on the [three-sphere](../../../geometry-and-topology.md#three-sphere); regular solutions have $\lambda=\ell(\ell+2)$ with $\ell=0,2,4,\ldots$, the even values selected by the absence of $\phi$ and $\psi$ dependence.

## 2

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Take $n^an_a=-1$. The [first fundamental form](../../../differential-geometry.md#first-fundamental-form), or [induced metric](../../../riemannian-geometry.md#induced-metric), is the [spatial projection tensor](../../../numerical-relativity.md#spatial-projection-tensor)

$$
\boxed{h_{ab}=g_{ab}+n_an_b},\qquad h_a{}^b=\delta_a{}^b+n_an^b.
$$

With the convention used in the question, define the [second fundamental form](../../../second-fundamental-form.md) by

$$
\boxed{K_{ab}=-h_a{}^ch_b{}^d\nabla_cn_d}.
$$

Locally $n_a$ is proportional to the gradient of a defining function for the [hypersurface](../../../differential-geometry.md#hypersurface), so $h_a{}^ch_b{}^d\nabla_{[c}n_{d]}=0$ and $K_{ab}=K_{ba}$. Both derivative indices are projected tangentially. If two extensions of $n$ agree on $\Sigma$, their difference vanishes there, as does its tangential derivative, so $K_{ab}$ is independent of the extension.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let $D$ be the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) of $h$. Apply $(D_cD_d-D_dD_c)$ to a tangent vector, replace each $D$ by the tangential projection of $\nabla$, and decompose $\nabla n$ using $K_{ab}$. Comparison with the intrinsic [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) gives the [Gauss equation](../../../second-fundamental-form.md#gauss-equation)

$$
\boxed{{}^{(3)}R_{abcd}=h_a{}^eh_b{}^fh_c{}^gh_d{}^h\,{}^{(4)}R_{efgh}-K_{ac}K_{bd}+K_{ad}K_{bc}}.
$$

Changing the sign convention for $K_{ab}$ does not alter these quadratic terms.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Contract the [Gauss equation](../../../second-fundamental-form.md#gauss-equation) with $h^{ac}h^{bd}$. Since $h^{ab}=g^{ab}+n^an^b$ and the antisymmetries of the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) eliminate the term containing four normals,

$$
h^{ac}h^{bd}R_{abcd}=R+2R_{ab}n^an^b.
$$

The extrinsic terms contract to $K^2$ and $K_{ab}K^{ab}$. Hence the intrinsic [Ricci scalar](../../../general-relativity.md#ricci-scalar) is

$$
\boxed{{}^{(3)}R=R+2R_{ab}n^an^b-K^2+K_{ab}K^{ab}}.
$$

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Contract the [Einstein field equations](../../../general-relativity.md#einstein-field-equations) $G_{ab}=8\pi T_{ab}$ twice with $n^a$. Since $n^an_a=-1$ and $\rho=T_{ab}n^an^b$,

$$
R+2R_{ab}n^an^b=16\pi\rho.
$$

If $K_{ab}$ is proportional to $h_{ab}$ in three dimensions, tracing gives $K_{ab}=(K/3)h_{ab}$ and $K_{ab}K^{ab}=K^2/3$. The [Scalar Gauss equation](../../../numerical-relativity.md#scalar-gauss-equation) gives the [Hamiltonian constraint](../../../numerical-relativity.md#hamiltonian-constraint)

$$
{}^{(3)}R=16\pi\rho-\frac23K^2=\frac23(24\pi\rho-K^2).
$$

Therefore

$$
\boxed{24\pi\rho-K^2\geq0\quad\Longrightarrow\quad{}^{(3)}R\geq0}.
$$

## 3

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For any nonzero $g$-causal vector $v^a$,

$$
\widetilde g_{ab}v^av^b=g_{ab}v^av^b-(t_av^a)^2.
$$

For timelike $v$, the first term is negative. For null $v$, a nonzero null vector cannot be orthogonal to a timelike vector, so $(t\mathbin\cdot v)^2>0$. Thus

$$
\boxed{\widetilde g(v,v)<0}
$$

in both cases. Every $g$-causal direction is strictly timelike for $\widetilde g$, so its [light cone](../../../special-relativity.md#light-cone) is strictly wider.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Let $t^a$ exhibit the [stable causality](../../../general-relativity.md#stable-causality) of $g$, so $g-t_at_b$ has no [closed timelike curves](../../../general-relativity.md#closed-timelike-curve). Set

$$
r^a=\frac{t^a}{\sqrt2},\qquad g'_{ab}=g_{ab}-r_ar_b=g_{ab}-\frac12t_at_b.
$$

The vector $r^a$ remains timelike for $g'$. Widening the cones of $g'$ once more using $r$ gives

$$
g'_{ab}-r_ar_b=g_{ab}-t_at_b,
$$

which is causal by assumption. Hence

$$
\boxed{g-r r\ \text{is itself stably causal}}.
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The relevant implications in the [causal hierarchy](../../../general-relativity.md#causal-hierarchy) are

$$
\text{stable causality}\Longrightarrow\text{strong causality}\Longrightarrow\text{future-distinguishing spacetime}.
$$

The first follows from strict cone widening: failure of [strong causality](../../../general-relativity.md#strong-causality) would give causal curves leaving and re-entering arbitrarily small neighborhoods, and the wider metric turns the limiting recurrence into a [closed timelike curve](../../../general-relativity.md#closed-timelike-curve). For the second, if distinct $p,q$ had $I^+(p)=I^+(q)$, arbitrarily short timelike segments near either point and this equality would produce a causal curve leaving and re-entering a sufficiently small causally convex neighborhood. Therefore

$$
\boxed{I^+(p)=I^+(q)\quad\Longrightarrow\quad p=q}.
$$

The stated [null geodesic completeness](../../../general-relativity.md#null-geodesic-completeness) is stronger than needed: stable causality already gives the conclusion.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Write $I^+(U)=U=I^-(U)$. Since every [chronological future](../../../general-relativity.md#chronological-future) and [chronological past](../../../general-relativity.md#chronological-past) is open, $U$ is an [open set](../../../topology.md#open-set). We show its complement is also open.

Take $p\notin U$ and choose $p_-\ll p\ll p_+$ in a convex normal neighborhood. The diamond $V=I^+(p_-)\cap I^-(p_+)$ is a neighborhood of $p$. If $x\in V\cap U$, then $p_-\ll x$ and $U=I^-(U)$ imply $p_-\in U$; then $p_-\ll p$ and $U=I^+(U)$ imply $p\in U$, a contradiction. Thus $V$ lies in the complement of $U$.

Hence $U$ is nonempty, open, and closed. Since $\mathcal M$ is a [connected space](../../../geometry-and-topology.md#connected-space),

$$
\boxed{U=\mathcal M}.
$$

## 4

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For a real free [scalar field](../../../quantum-field-theory.md#scalar-field) on a [globally hyperbolic spacetime](../../../general-relativity.md#globally-hyperbolic-spacetime), take

$$
S=-\frac12\int d^4x\sqrt{-g}\left(\nabla_a\phi\nabla^a\phi+(m^2+\xi R)\phi^2\right).
$$

The [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation) has a well-posed initial-value problem on every [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface). Its complex solution space carries the conserved [Klein-Gordon inner product](../../../quantum-field-theory.md#klein-gordon-inner-product). Choose modes with

$$
(u_i,u_j)_{KG}=\delta_{ij},\qquad (u_i^*,u_j^*)_{KG}=-\delta_{ij},\qquad (u_i,u_j^*)_{KG}=0,
$$

and expand

$$
\widehat\phi=\sum_i(a_i u_i+a_i^\dagger u_i^*),\qquad [a_i,a_j^\dagger]=\delta_{ij}.
$$

The [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation) produce the [bosonic Fock space](../../../quantum-field-theory.md#bosonic-fock-space), and $a_i|0\rangle=0$ defines the chosen vacuum.

The choice of [positive-frequency solutions](../../../quantum-field-theory.md#positive-frequency-solution) is extra structure. In a time-dependent geometry there is no preferred time translation, so different choices mix $u_i$ with $u_i^*$ and give the [vacuum ambiguity in a nonstationary spacetime](../../../quantum-field-theory.md#vacuum-ambiguity-in-a-nonstationary-spacetime). In a [stationary spacetime](../../../general-relativity.md#stationary-spacetime), a timelike [Killing vector field](../../../general-relativity.md#killing-vector-field) defines positive frequency by $i\mathcal L_Ku_i=\omega_i u_i$, $\omega_i>0$, and hence the preferred [vacuum state in a stationary spacetime](../../../quantum-field-theory.md#vacuum-state-in-a-stationary-spacetime).

If the spacetime is stationary in the remote past and future, define normalized in- and out-modes there. Their [Bogoliubov transformation](../../../quantum-field-theory.md#bogoliubov-transformation) is

$$
u_i^{\rm out}=\sum_j(\alpha_{ij}u_j^{\rm in}+\beta_{ij}u_j^{{\rm in}*}).
$$

The expected out-particle number in the in-vacuum is

$$
\boxed{\langle0_{\rm in}|N_i^{\rm out}|0_{\rm in}\rangle=\sum_j|\beta_{ij}|^2}.
$$

Thus nonzero beta coefficients measure particle creation by the intervening time dependence.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Classically, the [laws of black-hole mechanics](../../../general-relativity.md#laws-of-black-hole-mechanics) have the same form as the laws of [thermodynamics](../../../thermodynamics.md), but this could have been only a formal analogy. [Hawking radiation](../../../general-relativity.md#hawking-radiation) makes it physical: a stationary black hole emits approximately [thermal radiation](../../../electromagnetism.md#thermal-radiation) with

$$
\boxed{T_H=\frac{\hbar\kappa}{2\pi k_Bc}},
$$

so [surface gravity](../../../general-relativity.md#surface-gravity) is proportional to genuine [temperature](../../../thermodynamics.md#temperature).

The correspondence is:


- constancy of $\kappa$ on a stationary horizon becomes constancy of equilibrium temperature;
- the [First law of black-hole mechanics](../../../general-relativity.md#first-law-of-black-hole-mechanics)


$$
dM=\frac{\kappa}{8\pi G}\,dA+\Omega_H\,dJ+\Phi_H\,dQ
$$

matches the [first law of thermodynamics](../../../thermodynamics.md#first-law-of-thermodynamics) and fixes the [Bekenstein-Hawking entropy](../../../general-relativity.md#bekenstein-hawking-entropy)

$$
\boxed{S_{BH}=\frac{k_Bc^3A}{4G\hbar}};
$$


- [Hawking's area theorem](../../../general-relativity.md#hawking-s-area-theorem) becomes a second law, replaced in the quantum theory by the [generalized second law](../../../general-relativity.md#generalized-second-law) for $S_{BH}+S_{\rm outside}$;
- the impossibility of reaching $\kappa=0$ by a finite process parallels the unattainability of absolute zero.

A real Hawking temperature therefore identifies horizon area as thermodynamic entropy and turns the geometric laws into thermodynamic laws.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
