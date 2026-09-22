# Paper 71

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper71.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper71.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [differential form](../../../differential-form.md) of degree $k$ is integrated over an oriented $k$-dimensional [smooth manifold](../../../differential-geometry.md#smooth-manifold) by integrating its coefficient in orientation-preserving coordinates. For an oriented parametrization $F:U\to M$, this means integrating the [pullback](../../../category.md#pullback-category-theory) $F^*\alpha$ over $U$; a [partition of unity](../../../differential-geometry.md#partition-of-unity) combines charts. The [change of variables formula](../../../calculus.md#change-of-variables-formula) makes the result independent of the charts. Reversing the [orientation of a smooth manifold](../../../differential-geometry.md#orientation-of-a-smooth-manifold) reverses the integral. The [Generalized Stokes theorem](../../../differential-form.md#generalized-stokes-theorem) says, for a compact oriented $k$-dimensional [smooth manifold](../../../differential-geometry.md#smooth-manifold) with boundary and a smooth $(k-1)$-form $\beta$,

$$
\int_M d\beta=\int_{\partial M}\beta,
$$

where the right-hand side includes the boundary [pullback](../../../category.md#pullback-category-theory), and the boundary has the [outward-normal-first boundary orientation](../../../differential-geometry.md#outward-normal-first-boundary-orientation). Compact support suffices on a noncompact manifold. This unifies the fundamental theorem of calculus, circulation and flux identities.

For example, take the unit disk $D$ oriented by $dx\wedge dy$ and the [differential one-form](../../../differential-form.md#one-form) $\beta=\tfrac12(x\,dy-y\,dx)$. Its [exterior derivative](../../../differential-form.md#exterior-derivative) is $d\beta=dx\wedge dy$, so the area integral is $\pi$. Parametrizing the positively oriented circle by $(x,y)=(\cos t,\sin t)$ gives the [pullback](../../../category.md#pullback-category-theory) $\beta=\tfrac12dt$ and the boundary integral $\int_0^{2\pi}\tfrac12dt=\pi$, directly illustrating [Generalized Stokes theorem](../../../differential-form.md#generalized-stokes-theorem).

For the distance calculation, write $u=|\mathbf r_1|$, $v=|\mathbf r_2|$, $x=u+v$ and $y=u-v$; these are scalar radii, not position vectors. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) and its reverse give $r\leq u+v=x$ and $|y|=|u-v|\leq r$. Also,

$$
x+|y|=2\max(u,v)\leq2R.
$$

Thus **$r\leq x\leq2R-|y|$ and $|y|\leq r$**. These conditions, with $u,v\geq0$, are also sufficient for a triangle with side lengths $u,v,r$. Endpoints correspond to collinear configurations.

Assume the two positions are [independent random variables](../../../random-variable.md#independent-random-variables), each having constant volume [probability density](../../../quantum-mechanics.md#probability-density) inside the radius-$R$ [ball](../../../topological-analysis.md#ball-mathematics). Independence is needed: uniform marginal distributions alone do not determine the distance distribution. Put $C=3/(4\pi R^3)$ and $\mathbf s=\mathbf r_2-\mathbf r_1$. The [change of variables](../../../calculus.md#change-of-variables-formula) $(\mathbf r_1,\mathbf r_2)\mapsto(\mathbf r_1,\mathbf s)$ has unit [Jacobian determinant](../../../calculus.md#jacobian-determinant), so the joint probability volume [differential form](../../../differential-form.md) is the product of the two normalized volume forms. In spherical coordinates for $\mathbf r_1$ and for $\mathbf s$ relative to its axis, it is

$$
C^2u^2\sin\theta_1\,du\wedge d\theta_1\wedge d\phi_1\wedge r^2\sin\theta\,dr\wedge d\theta\wedge d\chi.
$$

The polar coordinates fail on axes and at zero radii, which are sets of zero volume and do not affect the [probability](../../../probability-theory.md#probability). Here $\theta$ is the angle from $\mathbf r_1$ to $\mathbf s$. The [law of cosines](../../../geometry-and-topology.md#law-of-cosines) becomes

$$
v^2=u^2+r^2+2ur\cos\theta.
$$

Differentiating and taking the [wedge product](../../../linear-algebra.md#exterior-product) with $du\wedge dr$ eliminates the terms involving $du$ and $dr$:

$$
du\wedge dr\wedge(v\,dv)=-ur\sin\theta\,du\wedge dr\wedge d\theta.
$$

Consequently the positive integration density transforms by $|\sin\theta\,d\theta|=v\,dv/(ur)$ at fixed $u,r$. The minus sign is accounted for by reversal of limits: $v$ decreases as $\theta$ increases. The radial variable retained is $r$, while the polar angle is replaced by $v$; equivalently one can start with the angle between the two position vectors and replace that angle by $r$. The wording of the printed hint conflates these two coordinate choices, but its volume form gives the stated transformation directly.

Integrating $\sin\theta_1\,d\theta_1\,d\phi_1$ over the first orientation gives $4\pi$, and integrating $d\chi$ gives $2\pi$. The [probability density function](../../../continuous-probability-distribution.md#probability-density-function) of $r$ is therefore

$$
f_R(r)=8\pi^2C^2r\iint_{D_r}uv\,du\,dv=\frac{9r}{2R^6}\iint_{D_r}uv\,du\,dv,
$$

where $D_r$ has $0\leq u,v\leq R$ and $|u-v|\leq r\leq u+v$. There are no such configurations for $r>2R$.

To evaluate this integral explicitly, the [Jacobian determinant](../../../calculus.md#jacobian-determinant) of $(u,v)=((x+y)/2,(x-y)/2)$ has absolute value $1/2$. Hence $uv\,du\,dv=(x^2-y^2)\,dx\,dy/8$ as a positive density. For $0\leq r\leq2R$, set $a=\min(r,2R-r)$. The domain is $-a\leq y\leq a$, $r\leq x\leq2R-|y|$, and evenness in $y$ gives

$$
I(r)=\iint_{D_r}uv\,du\,dv=\frac14\int_0^a\left[\frac{(2R-y)^3-r^3}{3}-y^2(2R-y-r)\right]dy.
$$

An antiderivative, zero at $y=0$, yields

$$
I(r)=\frac1{12}\left[(8R^3-r^3)a-6R^2a^2+ra^3+\frac{a^4}{2}\right].
$$

Substituting $a=r$ for $r\leq R$ and $a=2R-r$ for $r\geq R$ gives the same polynomial in both intervals:

$$
I(r)=\frac{2R^3r}{3}-\frac{R^2r^2}{2}+\frac{r^4}{24}.
$$

Thus the [distance between two uniform points in a three-dimensional ball](../../../continuous-probability-distribution.md#distance-between-two-uniform-points-in-a-three-dimensional-ball) has the final density

$$
\boxed{dP=\left(\frac{3r^2}{R^3}-\frac{9r^3}{4R^4}+\frac{3r^5}{16R^6}\right)dr,\qquad 0\leq r\leq2R.}
$$

It is zero outside this interval. Its nonnegativity also follows from $f_R(r)=3r^2(4R+r)(2R-r)^2/(16R^6)$, and direct integration gives $\int_0^{2R}f_R(r)dr=1$. The derivation uses the full six-dimensional probability volume [differential form](../../../differential-form.md), rather than treating the three scalar distances as independent.

## 2

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The displayed matrices describe the orientation-preserving component $SE(2)$ of the full [Euclidean group](../../../geometry-and-topology.md#euclidean-group) $E(2)=O(2)\ltimes\mathbb R^2$. Both have the same [Lie algebra](../../../lie-algebra.md), so this naming convention does not affect the calculation. Choose the translation generators $P_1,P_2$ and rotation generator $J$ in the [Lie algebra](../../../lie-algebra.md) of this [Matrix Lie group](../../../lie-theory.md#matrix-lie-group) as

$$
P_1=\begin{pmatrix}0&0&1\\0&0&0\\0&0&0\end{pmatrix},\qquad P_2=\begin{pmatrix}0&0&0\\0&0&1\\0&0&0\end{pmatrix},\qquad J=\begin{pmatrix}0&-1&0\\1&0&0\\0&0&0\end{pmatrix}.
$$

Taking matrix [commutators](../../../lie-algebra.md#commutator) gives

$$
\boxed{[P_1,P_2]=0,\qquad[J,P_1]=P_2,\qquad[J,P_2]=-P_1.}
$$

All remaining brackets follow from antisymmetry. The corresponding [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field) in coordinates $(x,y,\psi)$ are

$$
L_1=\cos\psi\,\partial_x+\sin\psi\,\partial_y,\qquad L_2=-\sin\psi\,\partial_x+\cos\psi\,\partial_y,\qquad L_3=\partial_\psi.
$$

Their [Lie brackets of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) obey the same relations. This also fixes which sign of the rotation generator is being used.

There is an important qualification to the printed connection prescription. For an arbitrary [vector field](../../../calculus.md#vector-field) $Z$ and smooth function $f$, its literal right-hand side obeys

$$
\lambda[L_i,fZ]=\lambda L_i(f)Z+\lambda f[L_i,Z].
$$

An [affine connection](../../../fiber-bundle.md#affine-connection) instead requires $\nabla_{L_i}(fZ)=L_i(f)Z+f\nabla_{L_i}Z$. Thus **the formula for arbitrary $Z$ defines a connection only when $\lambda=1$**. For example, at $\psi=0$, take $i=1$, $f=x$ and $Z=L_1$: the erroneous formula gives $\lambda L_1$, whereas the [Leibniz rule](../../../calculus.md#leibniz-rule) requires $L_1$.

The intended one-parameter family is the [bracket connection on a Lie group](../../../fiber-bundle.md#bracket-connection-on-a-lie-group): prescribe the rule for left-invariant $Z$, then extend it by the [Leibniz rule](../../../calculus.md#leibniz-rule). If $[L_i,L_j]=c_{ij}{}^kL_k$, this means

$$
\nabla_{L_i}L_j=\lambda c_{ij}{}^kL_k,\qquad \nabla_{L_i}(z^jL_j)=L_i(z^j)L_j+\lambda z^j c_{ij}{}^kL_k.
$$

Extend linearly over functions in the first slot. This is a well-defined [affine connection](../../../fiber-bundle.md#affine-connection) for every real $\lambda$. The following [Ricci tensor](../../../general-relativity.md#ricci-tensor) calculation applies to this intended family; under the literal arbitrary-$Z$ reading only its $\lambda=1$ member exists.

Use the curvature convention

$$
R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z,\qquad \operatorname{Ric}(X,Y)=\operatorname{tr}\bigl(Z\mapsto R(Z,X)Y\bigr).
$$

For [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field) the [structure constants of a Lie algebra](../../../lie-algebra.md#structure-constant-of-a-lie-algebra) are constant. The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) gives

$$
\begin{aligned}
R(X,Y)Z&=\lambda^2\bigl([X,[Y,Z]]-[Y,[X,Z]]\bigr)-\lambda[[X,Y],Z]\\
&=\lambda(\lambda-1)[[X,Y],Z].
\end{aligned}
$$

Writing $A=\lambda(\lambda-1)$, the only nonzero curvature actions, apart from antisymmetry in the first two slots, are

$$
R(L_3,L_1)L_3=A L_1,\qquad R(L_3,L_2)L_3=A L_2.
$$

For instance, $[[J,P_1],J]=[P_2,J]=P_1$. Contracting the first and output slots gives $\operatorname{Ric}(L_3,L_3)=-2A$, while every other component vanishes. Equivalently, $[[Z,X],Y]=\operatorname{ad}_Y\operatorname{ad}_X Z$, so

$$
\operatorname{Ric}(X,Y)=A\,B(X,Y),\qquad B(X,Y)=\operatorname{tr}(\operatorname{ad}_X\operatorname{ad}_Y).
$$

This is the [Killing form](../../../lie-algebra.md#killing-form). Here $\operatorname{ad}_J$ rotates the two-dimensional translation space and vanishes on $J$, so $B(J,J)=-2$; translation generators give all other components zero. Therefore

$$
\boxed{(\operatorname{Ric}_{ij})_{i,j=1}^3=\begin{pmatrix}0&0&0\\0&0&0\\0&0&2\lambda(1-\lambda)\end{pmatrix}.}
$$

Since the coframe component dual to $L_3$ is $d\psi$, the same [Ricci tensor](../../../general-relativity.md#ricci-tensor) is $2\lambda(1-\lambda)d\psi\otimes d\psi$ in these coordinates. Reversing the curvature convention reverses this sign.

At both $\lambda=0$ and $\lambda=1$, the full curvature vanishes. At $\lambda=0$, the [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field) form a global [parallel frame](../../../fiber-bundle.md#parallel-frame-along-a-curve). At $\lambda=1$, every [right-invariant vector field](../../../lie-theory.md#right-invariant-vector-field) is parallel because left- and right-invariant [vector fields](../../../calculus.md#vector-field) commute; the connection is flat in that global [parallel frame](../../../fiber-bundle.md#parallel-frame-along-a-curve). Flatness does not imply zero torsion: for left-invariant arguments the [torsion tensor](../../../fiber-bundle.md#torsion-tensor) is

$$
T(X,Y)=\nabla_XY-\nabla_YX-[X,Y]=(2\lambda-1)[X,Y].
$$

Thus **the two endpoint connections are flat, with opposite nonzero torsion**. For comparison, $\lambda=1/2$ is torsion-free but has nonzero curvature, with $\operatorname{Ric}_{33}=1/2$. No metric has been specified, so these connections should not automatically be identified with a [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection).

## 3

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [symplectic manifold](../../../symplectic-geometry.md#symplectic-manifold) is a smooth even-dimensional [manifold](../../../topology.md#topological-manifold) $M$ with a [differential two-form](../../../differential-form.md#2-form) $\omega$ that is closed, $d\omega=0$, and nondegenerate at every point. Nondegeneracy identifies [vector fields](../../../calculus.md#vector-field) with [differential one-forms](../../../differential-form.md#one-form) by the [interior product](../../../differential-form.md#interior-product) $X\mapsto\iota_X\omega$. In this solution use the explicit [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) convention

$$
\iota_{X_f}\omega=df,\qquad \{f,g\}=\omega(X_f,X_g).
$$

This contraction sign differs from the negative-sign convention sometimes used for [Hamiltonian vector fields](../../../symplectic-geometry.md#hamiltonian-vector-field); all subsequent signs are fixed by the displayed choice. In [Darboux coordinates](../../../symplectic-geometry.md#darboux-chart) with $\omega=\sum_a dx_a\wedge dy_a$ it gives

$$
X_f=\sum_a\left(f_{y_a}\partial_{x_a}-f_{x_a}\partial_{y_a}\right),\qquad \{f,g\}=\sum_a\left(f_{x_a}g_{y_a}-f_{y_a}g_{x_a}\right),\qquad X_f(g)=-\{f,g\}.
$$

The [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) is bilinear and antisymmetric, and the ordinary product rule gives $\{f,gh\}=\{f,g\}h+g\{f,h\}$. Thus it remains to check the [Jacobi identity for the Poisson bracket](../../../classical-mechanics.md#jacobi-identity-for-the-poisson-bracket).

The [Cartan formula for the Lie derivative](../../../differential-form.md#cartan-s-magic-formula) and closedness of the [symplectic form](../../../symplectic-geometry.md#symplectic-form) give $\mathcal L_{X_f}\omega=d(\iota_{X_f}\omega)+\iota_{X_f}d\omega=d^2f=0$. Hence

$$
\begin{aligned}
\iota_{[X_f,X_g]}\omega&=\mathcal L_{X_f}(\iota_{X_g}\omega)-\iota_{X_g}(\mathcal L_{X_f}\omega)\\
&=\mathcal L_{X_f}(dg)=d(X_f g)=-d\{f,g\},
\end{aligned}
$$

and nondegeneracy gives

$$
\boxed{[X_f,X_g]=-X_{\{f,g\}}.}
$$

Applying both sides to an arbitrary smooth function $h$ gives $\{f,\{g,h\}\}-\{g,\{f,h\}\}=\{\{f,g\},h\}$, which is exactly the [Jacobi identity for the Poisson bracket](../../../classical-mechanics.md#jacobi-identity-for-the-poisson-bracket). Consequently the smooth functions, with their pointwise product and this [Poisson bracket](../../../classical-mechanics.md#poisson-bracket), form a [Poisson algebra](../../../algebra.md#poisson-algebra). Constants have zero [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field). If $f,g$ are components of [moment maps](../../../symplectic-geometry.md#moment-map), the same displayed relation relates the brackets of their [Hamiltonian vector fields](../../../symplectic-geometry.md#hamiltonian-vector-field) to the [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) of those components. In the opposite contraction convention the corresponding relation is the [Hamiltonian Lie algebra homomorphism](../../../symplectic-geometry.md#hamiltonian-lie-algebra-homomorphism) with the compatible bracket sign.

For the [point vortices](../../../fluid-mechanics.md#line-vortex), remove the collision diagonals from $(\mathbb R^2)^N$, since the logarithmic [Hamiltonian function](../../../symplectic-geometry.md#hamiltonian-function) is singular there. Set $s_{ab}=(x_a-x_b)^2+(y_a-y_b)^2>0$ for $a\ne b$. Differentiating each pair contribution gives

$$
H_{x_a}=-2\sum_{b\ne a}\frac{x_a-x_b}{s_{ab}},\qquad H_{y_a}=-2\sum_{b\ne a}\frac{y_a-y_b}{s_{ab}}.
$$

The [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) therefore gives the equations of motion

$$
\boxed{\dot x_a=-2\sum_{b\ne a}\frac{y_a-y_b}{s_{ab}},\qquad\dot y_a=2\sum_{b\ne a}\frac{x_a-x_b}{s_{ab}}.}
$$

Each contribution is perpendicular to the displacement from vortex $b$ to vortex $a$ and has magnitude $2/|\mathbf r_a-\mathbf r_b|$. This is the velocity induced by a [point vortex](../../../fluid-mechanics.md#line-vortex) of positive [circulation](../../../fluid-mechanics.md#circulation-physics), with the normalization $\Gamma/(2\pi)=2$. Each vortex is advected by the velocity of the others, without a self-induced singular velocity. Pairwise contributions cancel in the total velocity, so $\sum_a x_a$ and $\sum_a y_a$ are conserved. For two vortices the separation is constant and they rotate counterclockwise about their midpoint, as expected for identical positive [point vortices](../../../fluid-mechanics.md#line-vortex).

For $L=\tfrac12\sum_a(x_a^2+y_a^2)$, compute its [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) with $H$ directly:

$$
\{L,H\}=\sum_a(x_aH_{y_a}-y_aH_{x_a})=-2\sum_a\sum_{b\ne a}\frac{y_ax_b-x_ay_b}{s_{ab}}=0.
$$

The last sum vanishes by pairing $(a,b)$ with $(b,a)$, since their numerators are opposite and denominators equal. Thus **$L$ Poisson commutes with $H$ and is conserved**. Equivalently, the [Hamiltonian function](../../../symplectic-geometry.md#hamiltonian-function) depends only on pairwise distances and is invariant under simultaneous rotations.

The standard positive generator of the simultaneous [circle group](../../../lie-theory.md#circle-group) $SO(2)$ action is

$$
Y=\sum_a\left(-y_a\partial_{x_a}+x_a\partial_{y_a}\right).
$$

Its [interior product](../../../differential-form.md#interior-product) with the [symplectic form](../../../symplectic-geometry.md#symplectic-form) is

$$
\iota_Y\omega=-\sum_a(y_a\,dy_a+x_a\,dx_a)=-dL.
$$

Use the [moment map](../../../symplectic-geometry.md#moment-map) convention $d\langle\mu,\xi\rangle=-\iota_{Y_\xi}\omega$ for the usual positive rotation generator. Identifying $\mathfrak{so}(2)^*$ with $\mathbb R$, this proves **$L$ is the moment map for the standard rotation action**. It is invariant under the action, hence equivariant because [circle group](../../../lie-theory.md#circle-group) $SO(2)$ is abelian. Additive constants are possible; the natural normalization is $L=0$ at the origin of the ambient space. On the collision-free space this polynomial is its restriction. With the solution's positive contraction convention, the rotation generator is $Y=-X_L$. Confusing these two signs would reverse the final augmented Hamiltonian.

Let $\mathcal R_\varphi$ denote simultaneous counterclockwise rotation through $\varphi$, and introduce the co-rotating coordinates by $\mathbf r(t)=\mathcal R_{\Omega t}\mathbf r'(t)$. Both the [symplectic form](../../../symplectic-geometry.md#symplectic-form) and $H$ are rotation-invariant, so pulling back the inertial [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) leaves $X_H$ unchanged. Differentiating the rotation gives the co-rotating equation

$$
\dot{\mathbf r}'=X_H(\mathbf r')-\Omega Y(\mathbf r')=X_H(\mathbf r')+\Omega X_L(\mathbf r')=X_{H+\Omega L}(\mathbf r').
$$

The co-rotating positions are constant precisely when this [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) vanishes. By nondegeneracy of the [symplectic form](../../../symplectic-geometry.md#symplectic-form), that is equivalent to

$$
\boxed{d(H+\Omega L)(\mathbf r')=0.}
$$

Conversely a collision-free [critical point](../../../analysis.md#critical-point) of this augmented [Hamiltonian function](../../../symplectic-geometry.md#hamiltonian-function) produces a rigidly rotating solution. This is a [rotating point-vortex relative equilibrium](../../../dynamical-systems.md#rotating-point-vortex-relative-equilibrium).

As a sign and scaling check, scaling every position by $s>0$ changes $H$ by $-N(N-1)\log s$. Therefore $\sum_a\mathbf r_a\cdot\nabla_aH=-N(N-1)$. At a [rotating point-vortex relative equilibrium](../../../dynamical-systems.md#rotating-point-vortex-relative-equilibrium), $\nabla_aH+\Omega\mathbf r_a=0$, so $2\Omega L=N(N-1)$. For $N\geq2$ the [angular velocity](../../../classical-mechanics.md#angular-velocity) is positive in this circulation convention. An equilateral three-vortex configuration of circumradius $\rho$ has $L=3\rho^2/2$ and $\Omega=2/\rho^2$, agreeing directly with the equations of motion.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
