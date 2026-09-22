# Paper 70

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper70.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper70.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a real matrix $A$ with positive [determinant](../../../linear-algebra.md#determinant), the [polar decomposition of an invertible real matrix](../../../linear-algebra.md#polar-decomposition-of-an-invertible-real-matrix) gives unique factorizations

$$
\boxed{A=RU=VR,\qquad R\in SO(3),\quad U=U^T>0,\quad V=V^T>0,}
$$

where $U$ and $V$ are the [right stretch tensor](../../../continuum-mechanics.md#right-stretch-tensor) and [left stretch tensor](../../../continuum-mechanics.md#left-stretch-tensor), respectively. Positivity here means positive definiteness, not merely nonnegative entries.

To prove existence, $C=A^TA$ is symmetric and $v^TCv=|Av|^2>0$ for every nonzero $v$, because $A$ is invertible. The [spectral theorem for real symmetric matrices](../../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) supplies an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) $Q$ and positive [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $c_j$ such that $C=Q\operatorname{diag}(c_1,c_2,c_3)Q^T$. Define $U$ using the [principal square root of a positive semidefinite matrix](../../../linear-algebra.md#principal-square-root-of-a-positive-semidefinite-matrix) construction:

$$
U=Q\operatorname{diag}(\sqrt{c_1},\sqrt{c_2},\sqrt{c_3})Q^T,
\qquad R=AU^{-1}.
$$

Then $R^TR=U^{-1}A^TAU^{-1}=I$, so $R$ is orthogonal. Also $\det R=\det A/\det U>0$; an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) has [determinant](../../../linear-algebra.md#determinant) plus or minus one, hence $\det R=1$. Set $V=RUR^T$. It is symmetric positive definite, $V^2=AA^T$, and $VR=RU=A$.

For uniqueness, any second factorization $A=R_1U_1$ with the same properties gives $U_1^2=A^TA=C$. Since $U_1$ commutes with its square, it preserves every [eigenspace](../../../linear-operator-theory.md#eigenspace) of $C$. On a $c$-eigenspace its own positive [eigenvalues](../../../linear-operator-theory.md#eigenvalue) must square to $c$, so it equals $\sqrt c$ times the identity there. Thus $U_1=U$, then $R_1=AU^{-1}=R$, and finally $V$ is fixed too. This proves both uniqueness and the [polar decomposition in continuum mechanics](../../../continuum-mechanics.md#polar-decomposition-in-continuum-mechanics), with the same proper rotation in its left and right forms.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A material fibre segment of reference length $L$ and unit direction $l$ has reference [vector](../../../vector-space.md#vector) $Ll$. The uniform [deformation gradient](../../../continuum-mechanics.md#deformation-gradient) maps it to $LAl$, whose current length is

$$
L|Al|=L\sqrt{l^TA^TAl}.
$$

Therefore its length is preserved if and only if

$$
\boxed{l^TA^TAl=1.}
$$

This is the [inextensible fibre constraint](../../../continuum-mechanics.md#inextensible-fibre-constraint). The [quadratic form](../../../linear-algebra.md#quadratic-form) uses the [right Cauchy-Green deformation tensor](../../../continuum-mechanics.md#right-cauchy-green-deformation-tensor); a subsequent rigid rotation does not change it, consistently with the polar factorization $A=RU$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For two distinct symmetric fibre families use reference directions $l_\pm=(\cos\theta,\pm\sin\theta,0)^T$, with $0<\theta<\pi/2$. The second sign is needed for the orthogonality conclusion: the PDF prints only one direction. If both families literally had that same direction, their images under an invertible deformation would remain parallel, so part (ii) would be false. The following derivation states the intended two-family geometry explicitly.

Write $c=\cos\theta$, $s=\sin\theta$ and take positive $\lambda,\alpha$, as required for a positive [stretch tensor](../../../continuum-mechanics.md#stretch-tensor). Applying the [inextensible fibre constraint](../../../continuum-mechanics.md#inextensible-fibre-constraint) to either family gives

$$
\frac{\alpha^2c^2+\alpha^{-2}s^2}{\lambda}=1.
$$

With $b=\alpha^2$, multiplication by $b$ yields $c^2b^2-\lambda b+s^2=0$. Its discriminant is $\lambda^2-4c^2s^2=\lambda^2-\sin^22\theta$, so the [two-family inextensible-fibre pure stretch](../../../continuum-mechanics.md#two-family-inextensible-fibre-pure-stretch) has

$$
\boxed{\alpha^2=\frac{\lambda\pm\sqrt{\lambda^2-\sin^22\theta}}{2\cos^2\theta}.}
$$

This also shows why the angle endpoints need separate treatment: at $\theta=0$ the admissible root is $\alpha^2=\lambda$, and at $\theta=\pi/2$ it is $\alpha^2=1/\lambda$. The nominal two families then represent the same unoriented fibre direction, and the two-branch/orthogonality assertions do not apply.

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

For $0<\theta<\pi/2$ and $\lambda>\sin2\theta$, the discriminant is strictly positive. The two roots have positive sum $\lambda/c^2$ and positive product $s^2/c^2$, so both roots are positive and distinct. Each gives exactly one positive $\alpha$ and hence a different [right stretch tensor](../../../continuum-mechanics.md#right-stretch-tensor). If $\lambda\ne1$, neither tensor is the undeformed identity because its third diagonal entry is $\lambda$. Thus **two distinct deformed configurations are possible**. Excluding $\lambda=1$ removes the case in which one of the two configurations is the undeformed body; it is not needed just for positivity of the roots.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

The smallest admissible axial stretch is $\lambda_{\min}=\sin2\theta$, where the two branches merge and $\alpha^2=\tan\theta=s/c$. The current unit fibre [vectors](../../../vector-space.md#vector) are $m_\pm=Ul_\pm$. Their [dot product](../../../linear-algebra.md#dot-product) is

$$
m_+\cdot m_-=
\frac1\lambda\left(\alpha^2c^2-\alpha^{-2}s^2\right).
$$

At the minimum, both terms in parentheses equal $cs$, so

$$
\boxed{m_+\cdot m_-=0.}
$$

Hence the two families are orthogonal at the maximum possible contraction. There is also a geometric proof of the bound: their reference parallelogram area is $\sin2\theta$, and its current area is $\sin2\theta/\lambda$, because the in-plane area stretch is $1/\lambda$. Two unit [vectors](../../../vector-space.md#vector) span area at most one, with equality precisely when perpendicular. This gives $\lambda\ge\sin2\theta$ and the same equality condition without solving the quadratic. At $\theta=\pi/4$ the minimum is one, so no axial contraction is possible and the fibres are already orthogonal.

## 2

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use the material-first [nominal stress tensor](../../../continuum-mechanics.md#nominal-stress-tensor) convention $N_{\alpha i}$, whose reference-volume power is $N_{\alpha i}\dot A_{i\alpha}$. At a regular constraint point, $F_{,A}\ne0$, all admissible deformation rates satisfy $F_{,A_{i\alpha}}\dot A_{i\alpha}=0$. Equality of mechanical power and the derivative of the [strain energy density](../../../continuum-mechanics.md#strain-energy-density) gives

$$
\left(N_{\alpha i}-W_{,A_{i\alpha}}\right)\dot A_{i\alpha}=0
$$

for every [vector](../../../vector-space.md#vector) in this eight-dimensional tangent hyperplane. Its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) is the span of $F_{,A}$. Consequently the [constraint reaction in hyperelastic stress](../../../continuum-mechanics.md#constraint-reaction-in-hyperelastic-stress) is

$$
\boxed{N_{\alpha i}=W_{,A_{i\alpha}}+qF_{,A_{i\alpha}}.}
$$

The scalar [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) $q$ is not determined by the work identity: its contribution vanishes on every allowed rate. Regularity matters. For example, replacing a regular [incompressibility](../../../fluid-mechanics.md#incompressible-flow) constraint by $(\det A-1)^2=0$ would give zero gradient on the same admissible set and could not represent an arbitrary pressure reaction through that gradient.

For [incompressibility](../../../fluid-mechanics.md#incompressible-flow) use the regular function $F=J-1$, with $J=\det A$. Differentiating the alternating-tensor expression for $J$ gives

$$
\frac{\partial J}{\partial A_{i\alpha}}
=\frac12\epsilon_{ijk}\epsilon_{\alpha\beta\gamma}A_{j\beta}A_{k\gamma}
=J(A^{-1})_{\alpha i}.
$$

The first expression is the cofactor entry; contracting it with $A_{j\alpha}$ gives $J\delta_{ij}$, proving the inverse formula. On $J=1$ this yields

$$
\boxed{N_{\alpha i}=W_{,A_{i\alpha}}+q(A^{-1})_{\alpha i}.}
$$

With this plus-sign convention $q$ is the negative of the usual pressure multiplier.

For an equibiaxially stretched sheet, [incompressibility](../../../fluid-mechanics.md#incompressible-flow) requires the principal stretches $(\lambda,\lambda,\lambda^{-2})$. The printed sheet expression's $\lambda^{-1/2}$ is inconsistent with this constraint and must be $\lambda^{-2}$; the balloon expression later on the same PDF page has the correct exponent. Let $W_j$ denote the derivative with respect to [principal stretch](../../../continuum-mechanics.md#principal-stretch) $\lambda_j$, evaluated on this constrained path. With no applied thickness-direction [traction](../../../continuum-mechanics.md#traction),

$$
0=N_{33}=W_3+q\lambda^2,
\qquad q=-\lambda^{-2}W_3.
$$

Isotropy gives $W_1=W_2$ at equal in-plane stretches. Hence

$$
N_{11}=N_{22}=W_1-\lambda^{-3}W_3,
\qquad
\frac d{d\lambda}W(\lambda,\lambda,\lambda^{-2})
=W_1+W_2-2\lambda^{-3}W_3.
$$

The [equibiaxial nominal tension of an incompressible sheet](../../../continuum-mechanics.md#equibiaxial-nominal-tension-of-an-incompressible-sheet) is therefore

$$
\boxed{N_{11}=N_{22}=\frac12\frac d{d\lambda}W(\lambda,\lambda,\lambda^{-2}).}
$$

The two equal in-plane nominal tensions do work $2N_{11}\,d\lambda$ per reference volume; the thickness-direction [nominal stress](../../../continuum-mechanics.md#nominal-stress-tensor) does no work because it is zero. That is exactly the constrained energy differential, explaining energy conservation. As a check that the printed exponent is a genuine error, a [neo-Hookean solid](../../../continuum-mechanics.md#neo-hookean-solid) gives $N=\mu(\lambda-\lambda^{-5})$, zero at the undeformed state. The derivative with the erroneous exponent would instead give $3\mu/4$ at that state.

For the thin spherical balloon, use the leading reference shell volume $4\pi a_0^2h_0$. Its two tangential stretches are $\lambda=a/a_0$, while its thickness stretch is $\lambda^{-2}$ and its current thickness is $h=h_0\lambda^{-2}$. Define $\widehat W(\lambda)=W(\lambda,\lambda,\lambda^{-2})$. Its total [elastic energy](../../../continuum-mechanics.md#elastic-energy) at leading thin-shell order is

$$
E=4\pi a_0^2h_0\widehat W(\lambda).
$$

During a quasistatic increment $da$, the enclosed volume changes by $d\mathcal V=4\pi a^2da$, and $d\lambda=da/a_0$. Equating energy change to work of the internal excess pressure gives

$$
p\,4\pi a^2da
=4\pi a_0h_0\widehat W'(\lambda)da,
\qquad
\boxed{p(a)=\frac{h_0}{a_0\lambda^2}\widehat W'(\lambda).}
$$

This is the [inflation pressure of a thin incompressible elastic balloon](../../../continuum-mechanics.md#inflation-pressure-of-a-thin-incompressible-elastic-balloon). The approximation neglects through-thickness variation and curvature corrections beyond leading order, and requires $h/a\ll1$. It also agrees with membrane [force](../../../classical-mechanics.md#force) balance: $p=2h\sigma_t/a$, $\sigma_t=\lambda N$, and $N=\widehat W'/2$. Here pressure is [force](../../../classical-mechanics.md#force) per current area, while $N$ is [force](../../../classical-mechanics.md#force) per reference area; confusing them would lose a factor of $\lambda$.

## 3

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $c=\cos(\alpha\xi_3)$, $s=\sin(\alpha\xi_3)$ and $r^2=x_1^2+x_2^2=(\xi_1^2+\xi_2^2)/\lambda$. Differentiating the deformation gives

$$
A=\begin{pmatrix}
\lambda^{-1/2}c&-\lambda^{-1/2}s&-\alpha x_2\\
\lambda^{-1/2}s&\lambda^{-1/2}c&\alpha x_1\\
0&0&\lambda
\end{pmatrix},
\qquad \det A=1.
$$

For the [neo-Hookean solid](../../../continuum-mechanics.md#neo-hookean-solid), $W_{,A_{i\alpha}}=\mu A_{i\alpha}$. The constrained [nominal stress tensor](../../../continuum-mechanics.md#nominal-stress-tensor) is therefore $N_{\alpha i}=\mu A_{i\alpha}+q(A^{-1})_{\alpha i}$. The multiplier cannot be set arbitrarily to a constant; equilibrium and the traction-free curved surface determine it.

Push the [nominal stress](../../../continuum-mechanics.md#nominal-stress-tensor) to the [Cauchy stress tensor](../../../continuum-mechanics.md#cauchy-stress-tensor): since $J=1$, $\sigma=AN=\mu AA^T+qI$. In the current cylindrical orthonormal basis, the [left Cauchy-Green deformation tensor](../../../continuum-mechanics.md#left-cauchy-green-deformation-tensor) has entries

$$
AA^T=\begin{pmatrix}
\lambda^{-1}&0&0\\
0&\lambda^{-1}+\alpha^2r^2&\alpha\lambda r\\
0&\alpha\lambda r&\lambda^2
\end{pmatrix}.
$$

Thus $\sigma_{rr}=\mu/\lambda+q$, $\sigma_{\vartheta\vartheta}=\mu/\lambda+\mu\alpha^2r^2+q$, and $\sigma_{\vartheta3}=\mu\alpha\lambda r$. Static radial equilibrium without [body force](../../../fluid-mechanics.md#body-force) gives

$$
\frac{d\sigma_{rr}}{dr}+\frac{\sigma_{rr}-\sigma_{\vartheta\vartheta}}r=0,
\qquad q'(r)=\mu\alpha^2r.
$$

The current outer radius is $a=R/\sqrt\lambda$. Setting $\sigma_{rr}(a)=0$ integrates the reaction field:

$$
\boxed{q(r)=-\frac\mu\lambda+\frac{\mu\alpha^2}{2}(r^2-a^2).}
$$

The other curved-surface [traction](../../../continuum-mechanics.md#traction) components vanish because $\sigma_{r\vartheta}=\sigma_{r3}=0$.

On the reference end $\xi_3=H$, the outward reference normal is $e_3$, and the nominal [traction](../../../continuum-mechanics.md#traction) has components $t_i=N_{3i}$. The third row of $A^{-1}$ is $(0,0,\lambda^{-1})$. Hence the [nominal end traction of a twisted neo-Hookean cylinder](../../../continuum-mechanics.md#nominal-end-traction-of-a-twisted-neo-hookean-cylinder) is

$$
\boxed{\begin{aligned}
t_1&=-\mu\alpha x_2,\\
t_2&=\mu\alpha x_1,\\
t_3&=\mu(\lambda-\lambda^{-2})
+\frac{\mu\alpha^2}{2\lambda^2}(\xi_1^2+\xi_2^2-R^2).
\end{aligned}}
$$

The current $x_1,x_2$ here are evaluated at $\xi_3=H$. These components are per unit reference area, not per unit current area.

For the moment, use current lever arms and reference-area [traction](../../../continuum-mechanics.md#traction). Its axial component is

$$
\begin{aligned}
M_3&=\int_{\xi_1^2+\xi_2^2<R^2}(x_1t_2-x_2t_1)\,d\xi_1d\xi_2\\
&=\frac{\mu\alpha}{\lambda}\int_0^{2\pi}\int_0^R s^2s\,ds\,d\vartheta
=\boxed{\frac{\mu\pi R^4\alpha}{2\lambda}.}
\end{aligned}
$$

The axial [traction](../../../continuum-mechanics.md#traction) gives no axial moment. This [torque](../../../classical-mechanics.md#torque) also agrees with the reference-energy derivative at fixed axial stretch: the twist-dependent energy per reference length is $\mu\alpha^2\pi R^4/(4\lambda)$. It is important that $\alpha$ is twist per reference length, not twist per current length.

## 4

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For [antiplane shear](../../../continuum-mechanics.md#antiplane-shear), the only nonzero infinitesimal [strains](../../../continuum-mechanics.md#strain) are $e_{13}=e_{31}=w_{,1}/2$ and $e_{23}=e_{32}=w_{,2}/2$. Their trace is zero. The isotropic constitutive law $\sigma_{ij}=\lambda_L e_{kk}\delta_{ij}+2\mu e_{ij}$ consequently gives

$$
\boxed{\sigma_{13}=\sigma_{31}=\mu w_{,1},\qquad
\sigma_{23}=\sigma_{32}=\mu w_{,2},}
$$

with every other component zero. The first two equations of motion vanish because the fields are independent of $x_3$. The third is $\rho w_{,tt}=\sigma_{31,1}+\sigma_{32,2}$, hence

$$
\boxed{\nabla^2w-\frac1{c^2}w_{,tt}=0,\qquad c^2=\mu/\rho.}
$$

The PDF omits the final equals-zero; this is the equation supplied by momentum balance.

For a steadily moving field put $x=x_1-Vt$ and $\beta=\sqrt{1-V^2/c^2}$. In the subsonic case $|V|<c$, the equation becomes $\beta^2w_{xx}+w_{x_2x_2}=0$. With $y=\beta x_2$ it reduces to $w_{xx}+w_{yy}=0$. Thus $w$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) and, on a simply connected region, has a [harmonic conjugate](../../../partial-differential-equation.md#harmonic-conjugate); there is a [holomorphic function](../../../complex-analysis.md#holomorphic-function) $H(z)$ such that

$$
\boxed{w=\operatorname{Re}H(z),\qquad z=x+iy.}
$$

This is [steadily moving antiplane shear](../../../continuum-mechanics.md#steadily-moving-antiplane-shear). The representation is local on more general domains unless the conjugate's periods vanish. The subsonic condition is essential: at or above the shear-wave speed the coordinate rescaling is degenerate or the equation is hyperbolic rather than this elliptic harmonic problem.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Retain $\beta=\sqrt{1-V^2/c^2}>0$, but normalize the complex potential as $F=\beta H$, so that $w=\operatorname{Re}F/\beta$. The [Cauchy-Riemann equations](../../../analysis.md#cauchy-riemann-equations) give $w_x=\operatorname{Re}F'/\beta$ and $w_y=-\operatorname{Im}F'/\beta$. Since $\partial_{x_2}=\beta\partial_y$, the two stresses satisfy

$$
\boxed{\beta\sigma_{13}-i\sigma_{23}=\mu F'(z).}
$$

Using the same unscaled $H$ from part (a) would instead put an additional $\beta$ on its derivative; the potential normalization matters.

Take the principal branch of $\sqrt z$, with its [branch cut](../../../analysis.md#branch-cut) along the negative real axis and positive $\sqrt x$ for $x>0$. Write $Q=F'$. For the antisymmetric crack-opening response, reflection gives $Q^-(s)=-\overline{Q^+(s)}$ on the faces. The prescribed equal face [stress](../../../continuum-mechanics.md#stress) gives $\operatorname{Im}Q^\pm(s)=f(s)/\mu$. Multiplication by the square-root factor converts this face condition to an additive jump. In fact, with $G=\sqrt zQ$ and $r=\sqrt{-s}$,

$$
G^+=irQ^+,\qquad G^-=-irQ^-=ir\overline{Q^+},
\qquad
G^+-G^-=-\frac{2}{\mu}\sqrt{-s}\,f(s).
$$

The [Sokhotski–Plemelj theorem](../../../complex-analysis.md#sokhotski-plemelj-theorem) applied to this jump gives

$$
G(z)=-\frac1{\pi i\mu}\int_{-\infty}^0\frac{\sqrt{-s}\,f(s)}{s-z}\,ds+P(z),
$$

where $P$ is entire after imposing the usual finite-energy crack-tip regularity. This is the [Hilbert problem for an antiplane crack](../../../continuum-mechanics.md#hilbert-problem-for-an-antiplane-crack), with the stress-potential phase chosen explicitly above.

For localized face loading with no additional remote loading, the far [displacement](../../../classical-mechanics.md#displacement) is bounded and the weighted Cauchy transform decays. In particular, for compactly supported loading, $G\to0$ at infinity and [Liouville theorem](../../../complex-analysis.md#liouville-theorem) sets $P=0$. The resulting [Cauchy solution for a steadily moving semi-infinite antiplane crack](../../../continuum-mechanics.md#cauchy-solution-for-a-steadily-moving-semi-infinite-antiplane-crack) is

$$
\boxed{F'(z)=-\frac{i}{\pi\mu\sqrt z}
\int_{-\infty}^0\frac{\sqrt{-s}\,f(s)}{z-s}\,ds.}
$$

Integrals and boundary values are understood for loadings with the corresponding convergence and regularity, or as limits of localized loading. The reflection used above is the pure antiplane opening response: reflection with a sign change of [displacement](../../../classical-mechanics.md#displacement) leaves both prescribed face stresses unchanged, and the usual no-extra-load uniqueness condition eliminates an unforced symmetric addition.

One can check the face stresses directly. Put $I_{\mathrm{pv}}(s)=\operatorname{PV}\int_{-\infty}^0\sqrt{-t}f(t)/(s-t)\,dt$. The Cauchy boundary limits give

$$
Q^+(s)=-\frac{I_{\mathrm{pv}}(s)}{\pi\mu\sqrt{-s}}+\frac{i}{\mu}f(s),
\qquad
Q^-(s)=\frac{I_{\mathrm{pv}}(s)}{\pi\mu\sqrt{-s}}+\frac{i}{\mu}f(s).
$$

Both have $-\mu\operatorname{Im}Q^\pm=-f(s)$, verifying the prescribed [traction](../../../continuum-mechanics.md#traction) and its sign on both faces. The opposite real parts also give the required reflection. Ahead of the tip, the integral is real and $Q$ is purely imaginary, so the bonded line has zero tangential [displacement](../../../classical-mechanics.md#displacement) gradient and the two halves match.

For $x=x_1-Vt>0$, take $z=x$ in the boxed analytic solution. The ahead-of-tip [stress](../../../continuum-mechanics.md#stress) is

$$
\boxed{\sigma_{23}(x_1,0,t)=\frac1{\pi\sqrt x}
\int_{-\infty}^0\frac{\sqrt{-s}\,f(s)}{x-s}\,ds.}
$$

No $\beta$ appears: **at fixed co-moving position and the specified co-moving face loading, this [stress](../../../continuum-mechanics.md#stress) is independent of the speed**. The [displacement](../../../classical-mechanics.md#displacement), however, still scales with $1/\beta$, so speed independence does not apply to the whole elastic field. If $\int_{-\infty}^0|f(s)|/\sqrt{-s}\,ds$ is finite, the near-tip [stress](../../../continuum-mechanics.md#stress) is inverse-square-root with coefficient $\pi^{-1}\int f(s)/\sqrt{-s}\,ds$.

The far-field condition is a genuine uniqueness requirement. A [homogeneous stress-intensity field of a semi-infinite antiplane crack](../../../continuum-mechanics.md#homogeneous-stress-intensity-field-of-a-semi-infinite-antiplane-crack) has $Q_h=iC/\sqrt z$, for real $C$. It adds no face [traction](../../../continuum-mechanics.md#traction) but changes the [stress](../../../continuum-mechanics.md#stress) ahead by $-\mu C/\sqrt x$. Although its [stress](../../../continuum-mechanics.md#stress) tends to zero at infinity, its primitive is $2iC\sqrt z$, which gives unbounded remote [displacement](../../../classical-mechanics.md#displacement) and infinite total [elastic energy](../../../continuum-mechanics.md#elastic-energy). Thus only asking for [stress](../../../continuum-mechanics.md#stress) to vanish at infinity would leave the homogeneous constant undetermined; excluding that added remote stress-intensity loading selects the displayed face-loaded solution. The ordinary inverse-square-root tip singularity itself has finite energy in a bounded neighbourhood and is not being excluded.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
