# Paper 20

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_20.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_20.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [a](#1/ii/a)
      - [Solution](#1/ii/a/solution)
    - [b](#1/ii/b)
      - [Solution](#1/ii/b/solution)
    - [c](#1/ii/c)
      - [Solution](#1/ii/c/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)

## 1

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Use the [standard symplectic form](../../../symplectic-geometry.md#standard-symplectic-form) $\omega_0=\sum_{j=1}^n dq_j\wedge dp_j$. A [canonical transformation](../../../classical-mechanics.md#canonical-transformation) is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) $f$ preserving this [symplectic form](../../../symplectic-geometry.md#symplectic-form):

$$
\boxed{f^*\omega_0=\omega_0.}
$$

Thus, writing $f(q,p)=(Q,P)$, the defining identity is $\sum_jdQ_j\wedge dP_j=\sum_jdq_j\wedge dp_j$. For a local [canonical transformation](../../../classical-mechanics.md#canonical-transformation), require this on its open domain. In particular preservation of the [symplectic form](../../../symplectic-geometry.md#symplectic-form), rather than just of [phase-space volume](../../../symplectic-geometry.md#symplectic-volume-form), is the condition in dimensions greater than two.

Throughout these solutions choose the [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) convention $\iota_{X_F}\omega=dF$. It gives $\dot q=F_p$, $\dot p=-F_q$ and agrees with the positive coordinate [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) used below. The opposite convention for [Hamiltonian vector fields](../../../symplectic-geometry.md#hamiltonian-vector-field) changes signs in the [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) identity but none of the commuting or integrability conclusions.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/a">a</h4>

↑ **Parent:** [Ii](#1/ii)

<h5 id="1/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#1/ii/a)

The [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) in the original coordinates is

$$
\boxed{\{F,G\}_{q,p}=\sum_{j=1}^n(F_{q_j}G_{p_j}-F_{p_j}G_{q_j}).}
$$

For $z=(q,p)$, set

$$
J=\begin{pmatrix}0&I_n\\-I_n&0\end{pmatrix},\qquad A=Df(z).
$$

Then $\omega_0(u,v)=u^T Jv$ and $\{F,G\}=\nabla F^T J\nabla G$. The pullback definition of a [canonical transformation](../../../classical-mechanics.md#canonical-transformation) gives the pointwise [matrix](../../../vector-space.md#matrix) condition

$$
\boxed{A^TJA=J.}
$$

Since $A$ is invertible, this is equivalent to $AJA^T=J$. Indeed, invert $A^TJA=J$ and use $J^{-1}=-J$ to obtain $A^{-1}JA^{-T}=J$, then multiply by $A$ and $A^T$. Applying the same calculation to the inverse implication gives equivalence. These are the two equivalent [symplectic matrix](../../../symplectic-geometry.md#symplectic-matrix) identities that connect the [symplectic form](../../../symplectic-geometry.md#symplectic-form) with [Poisson brackets](../../../classical-mechanics.md#poisson-bracket).

<h4 id="1/ii/b">b</h4>

↑ **Parent:** [Ii](#1/ii)

<h5 id="1/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#1/ii/b)

The [chain rule](../../../calculus.md#chain-rule) yields

$$
\{F\circ f,G\circ f\}_{q,p}
=(\nabla F\circ f)^T AJA^T(\nabla G\circ f).
$$

If $f$ is a [canonical transformation](../../../classical-mechanics.md#canonical-transformation), the [symplectic matrix](../../../symplectic-geometry.md#symplectic-matrix) identity $AJA^T=J$ makes this expression $\{F,G\}_{Q,P}\circ f$. Thus preservation of the [symplectic form](../../../symplectic-geometry.md#symplectic-form) implies preservation of every [Poisson bracket](../../../classical-mechanics.md#poisson-bracket), for all $C^1$ functions.

Conversely, assume this [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) identity for every $F,G$. Take $F(Z)=u\cdot Z$ and $G(Z)=v\cdot Z$, for arbitrary constant [vectors](../../../vector-space.md#vector) $u,v\in\mathbb R^{2n}$. It gives $u^TAJA^Tv=u^TJv$. Since this holds for every $u,v$, $AJA^T=J$, hence $A^TJA=J$. Therefore **preservation of all [Poisson brackets](../../../classical-mechanics.md#poisson-bracket) is equivalent to canonicity**. Only first [derivatives](../../../calculus.md#derivative) of $f,F,G$ enter this argument.

<h4 id="1/ii/c">c</h4>

↑ **Parent:** [Ii](#1/ii)

<h5 id="1/ii/c/solution">Solution</h5>

↑ **Parent:** [C](#1/ii/c)

Apply preservation of [Poisson brackets](../../../classical-mechanics.md#poisson-bracket) to the coordinate functions. It gives

$$
\{Q_i,Q_j\}=0,\qquad\{P_i,P_j\}=0,\qquad\{Q_i,P_j\}=\delta_{ij}.
$$

Conversely, the entries of $AJA^T$ are exactly the [Poisson brackets](../../../classical-mechanics.md#poisson-bracket) between all transformed coordinate functions. The displayed relations therefore say $AJA^T=J$, which implies the [canonical transformation](../../../classical-mechanics.md#canonical-transformation) condition and, by the [chain rule](../../../calculus.md#chain-rule), preservation of every [Poisson bracket](../../../classical-mechanics.md#poisson-bracket). Thus **all three conditions are equivalent**:

$$
\boxed{f^*\omega_0=\omega_0\quad\Longleftrightarrow\quad
\text{all brackets are preserved}\quad\Longleftrightarrow\quad
\{Q_i,Q_j\}=\{P_i,P_j\}=0,\ \{Q_i,P_j\}=\delta_{ij}.}
$$

In particular the original coordinate bracket $\{q_i,p_j\}$ is $\delta_{ij}$ with the chosen [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) convention.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Under the given rank hypothesis, the necessary and sufficient local condition is

$$
\boxed{\{a_i,a_j\}=0\quad\text{for every }i,j\text{ on a neighbourhood of the point}.}
$$

Vanishing only at the single point would not suffice: an extension preserves the coordinate [Poisson brackets](../../../classical-mechanics.md#poisson-bracket) throughout its domain. Necessity follows from the coordinate criterion just proved.

For sufficiency, put $Q_i=a_i$ and $Y_i=X_{Q_i}$. Because the [symplectic form](../../../symplectic-geometry.md#symplectic-form) is a [nondegenerate bilinear form](../../../linear-algebra.md#nondegenerate-bilinear-form) at every point, the independent [differentials](../../../differential-geometry.md#differential-of-a-smooth-map) $dQ_i$ give independent fields $Y_1,\ldots,Y_n$. They commute, since

$$
[X_{Q_i},X_{Q_j}]=X_{\{Q_j,Q_i\}}=0.
$$

Moreover $dQ_j(Y_i)=\{Q_j,Q_i\}=0$, so they span the tangent spaces of the $n$-dimensional fibres of the [submersion](../../../differential-geometry.md#submersion) $Q$. Choose a local section $s(Q)$ transverse to those fibres. Its joint local flow defines coordinates $(Q,t)$ by

$$
\Psi(Q,t)=\varphi_{Y_1}^{t_1}\circ\cdots\circ\varphi_{Y_n}^{t_n}(s(Q)).
$$

The [inverse function theorem](../../../calculus.md#inverse-function-theorem) makes $\Psi$ a local [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism), and commuting flows give $\Psi_*\partial_{t_i}=Y_i$.

In these coordinates $\iota_{\partial_{t_i}}\Psi^*\omega_0=dQ_i$. Each flow preserves the [symplectic form](../../../symplectic-geometry.md#symplectic-form), by [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula). Thus its coefficients are independent of $t$, and

$$
\Psi^*\omega_0=\sum_i dt_i\wedge dQ_i+\beta(Q),
$$

where $\beta=s^*\omega_0$ is a closed [differential two-form](../../../differential-form.md#2-form) on the base. On a small ball, the [Poincaré lemma](../../../differential-form.md#poincare-lemma) gives $\beta=d\alpha$, with $\alpha=\sum_i\alpha_i(Q)dQ_i$. Define

$$
P_i=-t_i-\alpha_i(Q).
$$

Then

$$
\sum_i dQ_i\wedge dP_i
=\sum_i dt_i\wedge dQ_i+d\alpha
=\Psi^*\omega_0.
$$

Consequently the original coordinates are extended to the required [canonical transformation](../../../classical-mechanics.md#canonical-transformation) $(Q,P)$, with the prescribed first half $Q=a$. Its [Jacobian matrix](../../../calculus.md#jacobian-matrix) is invertible by construction. This is the [canonical completion of independent commuting functions](../../../classical-mechanics.md#canonical-completion-of-independent-commuting-functions). For the printed $C^2$ data, the flows and resulting [canonical transformation](../../../classical-mechanics.md#canonical-transformation) can be taken $C^1$, which is sufficient to preserve the [symplectic form](../../../symplectic-geometry.md#symplectic-form); smooth data give smooth coordinates.

## 2

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A function $F$ is an [integral of motion](../../../classical-mechanics.md#integral-of-motion) of $H$ when it is constant along every trajectory of the [Hamiltonian flow](../../../classical-mechanics.md#hamiltonian-flow). Infinitesimally,

$$
\boxed{X_HF=\{F,H\}=0.}
$$

The [antisymmetry of a Lie bracket](../../../lie-algebra.md#antisymmetry-of-a-lie-bracket) of the [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) gives $X_FH=\{H,F\}=0$. Hence **$H$ is also an [integral of motion](../../../classical-mechanics.md#integral-of-motion) of $F$**.

For the commuting assertion, $\mathcal L_{X_F}\omega=d(\iota_{X_F}\omega)=d^2F=0$, because $\omega$ is closed. The contraction identity for a [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) then gives

$$
\iota_{[X_F,X_H]}\omega
=\mathcal L_{X_F}(\iota_{X_H}\omega)-\iota_{X_H}(\mathcal L_{X_F}\omega)
=\mathcal L_{X_F}(dH)=d(X_FH)=d\{H,F\}=0.
$$

Since the [symplectic form](../../../symplectic-geometry.md#symplectic-form) is a [nondegenerate bilinear form](../../../linear-algebra.md#nondegenerate-bilinear-form) at every point, **the [Hamiltonian vector fields](../../../symplectic-geometry.md#hamiltonian-vector-field) commute**:

$$
\boxed{[X_F,X_H]=0.}
$$

With the chosen convention the general identity is $[X_F,X_H]=X_{\{H,F\}}$. Equivalently, it follows by applying the [Jacobi identity for the Poisson bracket](../../../classical-mechanics.md#jacobi-identity-for-the-poisson-bracket) to an arbitrary test function. Local flows commute whenever both compositions are defined; no global completeness assumption is needed.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Take the separate oscillator energies

$$
E_i=\frac12(y_i^2+\alpha_i^2x_i^2),\qquad i=1,2.
$$

They depend on disjoint canonical coordinate pairs, so

$$
\{E_1,E_2\}=0,\qquad\{E_i,H\}=0.
$$

Thus they are [first integrals in involution](../../../classical-mechanics.md#first-integrals-in-involution). Their [differentials](../../../differential-geometry.md#differential-of-a-smooth-map)

$$
dE_i=\alpha_i^2x_i\,dx_i+y_i\,dy_i
$$

are nonzero precisely when $(x_i,y_i)\ne(0,0)$ and have disjoint supports. Hence they are [functionally independent](../../../calculus.md#functionally-independent-functions) on the specified open set.

To understand all further global [integrals of motion](../../../classical-mechanics.md#integral-of-motion), use the actions

$$
R_i=E_i/\alpha_i>0,\qquad
x_i=\sqrt{2R_i/\alpha_i}\sin\theta_i,\quad
y_i=\sqrt{2\alpha_iR_i}\cos\theta_i.
$$

Direct differentiation gives $dx_i\wedge dy_i=d\theta_i\wedge dR_i$, so these are [action-angle variables](../../../classical-mechanics.md#action-angle-variables) with

$$
H=\alpha_1R_1+\alpha_2R_2,\qquad
\dot R_i=0,\quad\dot\theta_i=\alpha_i.
$$

When $\alpha_2/\alpha_1$ is irrational, every orbit is dense in its fixed-action two-dimensional [flat torus](../../../second-fundamental-form.md#flat-torus). One elementary proof samples the orbit at times $2\pi j/\alpha_1$: the first angle returns, and the second undergoes an [irrational rotation](../../../measure-theory.md#irrational-rotation). These samples are dense in the second circle. Allowing a fixed additional time supplies any desired first angle, proving density in the whole [flat torus](../../../second-fundamental-form.md#flat-torus).

A continuous, globally defined [integral of motion](../../../classical-mechanics.md#integral-of-motion) must have the same value on an orbit and its closure. Therefore it is constant on every fixed-action [flat torus](../../../second-fundamental-form.md#flat-torus). A $C^1$ such integral has the form $F=\phi(R_1,R_2)$, with $\phi$ $C^1$, by evaluating $F$ at a fixed choice of angles. Hence

$$
\boxed{dF=\phi_{R_1}\,dR_1+\phi_{R_2}\,dR_2.}
$$

It cannot be independent of $E_1,E_2$. This proves **there are at most two globally independent differentiable integrals**. If a third global integral were independent at a point on an excluded coordinate plane, independence would persist in a neighbourhood and hence at nearby points of the regular open set, again a contradiction.

The word global matters: on an angular chart, $\alpha_2\theta_1-\alpha_1\theta_2$ is a local [integral of motion](../../../classical-mechanics.md#integral-of-motion) independent of the actions. It is not single-valued on the [flat torus](../../../second-fundamental-form.md#flat-torus) when the frequency ratio is irrational. Thus the assertion would be false for arbitrary local, rather than global, integrals.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The [Hamiltonian perturbation preserving one regular level](../../../symplectic-geometry.md#hamiltonian-perturbation-preserving-one-regular-level) is explicit:

$$
\boxed{K=H+\frac12\sum_{j=1}^rG_j^2.}
$$

Linearity of the [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) in the [differential of a smooth map](../../../differential-geometry.md#differential-of-a-smooth-map) gives

$$
X_K-X_H=\sum_{j=1}^rG_jX_{G_j}.
$$

It vanishes on $\Sigma_0$. At a point of $\Sigma_c$, its contraction with the [symplectic form](../../../symplectic-geometry.md#symplectic-form) is

$$
\iota_{X_K-X_H}\omega=\sum_jc_j\,dG_j.
$$

Since the [differentials](../../../differential-geometry.md#differential-of-a-smooth-map) are independent there, this vanishes exactly when $c=0$. Thus on every nonempty nonzero regular fibre the two [Hamiltonian vector fields](../../../symplectic-geometry.md#hamiltonian-vector-field) differ at every point, not merely as functions somewhere:

$$
\boxed{c\ne0,\ z\in\Sigma_c\quad\Longrightarrow\quad X_K(z)\ne X_H(z).}
$$

Mutual [Poisson commutation](../../../classical-mechanics.md#poisson-commuting-functions) of the $G_j$ is unnecessary; the given first-integral property does not by itself make the perturbed flow preserve every common level, nor is that requested.

There is a genuine missing nonemptiness hypothesis in the literal statement. Independent [differentials](../../../differential-geometry.md#differential-of-a-smooth-map) on an empty set is a vacuous condition, and any two vector-field restrictions to an empty set are equal. For example, on $\mathbb R^2$ let $r=1$, $G_1=H=e^q$, and $\rho=1$. Every nonempty $\Sigma_c$, $0<c<1$, is regular, while $\Sigma_c=\varnothing$ for $-1<c\le0$. In particular, the restrictions at $c=-1/2$ can never be unequal for any $K$. Therefore the printed universal inequality requires either **all the compared fibres to be nonempty**, or the pointwise formulation displayed above. The explicit $K$ fully proves either intended qualification.

## 3

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

On a $2n$-dimensional [symplectic manifold](../../../symplectic-geometry.md#symplectic-manifold), a [completely integrable Hamiltonian system](../../../classical-mechanics.md#integrable-hamiltonian-system) has $n$ [first integrals in involution](../../../classical-mechanics.md#first-integrals-in-involution) $F_1=H,F_2,\ldots,F_n$ whose [differentials](../../../differential-geometry.md#differential-of-a-smooth-map) are independent almost everywhere, hence on a dense open regular set:

$$
\boxed{\{F_i,F_j\}=0,\qquad dF_1\wedge\cdots\wedge dF_n\ne0.}
$$

An equivalent formulation allows $H$ to be a function of the $n$ commuting independent integrals. The independence requirement is on the regular set, permitting exceptional critical points and singular fibres.

For example, on $\mathbb R^{2n}$ take $H=\sum_{j=1}^nE_j$ with $E_j=(p_j^2+\alpha_j^2q_j^2)/2$ and $\alpha_j>0$. The disjoint coordinate pairs make all [Poisson brackets](../../../classical-mechanics.md#poisson-bracket) $\{E_i,E_j\}$ zero, and the [differentials](../../../differential-geometry.md#differential-of-a-smooth-map) are independent whenever no pair $(q_j,p_j)$ vanishes. Replacing $E_1$ by $H$ is an invertible [linear map](../../../vector-space.md#linear-map) of this list. Thus $F_1=H,F_j=E_j$ for $j\ge2$ give the required example. Irrational frequency ratios affect orbit density, but not [complete integrability](../../../classical-mechanics.md#integrable-hamiltonian-system).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The [Arnold-Liouville theorem](../../../classical-mechanics.md#liouville-arnold-theorem) concerns a connected compact component $L$ of a regular common level of $n$ commuting independent smooth functions $F=(F_1,\ldots,F_n)$ on a $2n$-dimensional [symplectic manifold](../../../symplectic-geometry.md#symplectic-manifold). It states that $L$ is a [Lagrangian torus](../../../symplectic-geometry.md#lagrangian-torus), and that a neighbourhood of $L$ has [action-angle variables](../../../classical-mechanics.md#action-angle-variables)

$$
(\theta,I)\in\mathbb T^n\times U,\qquad
\omega=\sum_jd\theta_j\wedge dI_j,
$$

in which every $F_i$ depends only on $I$. If $H=F_1$ or, more generally, $H=h(F)$, its [Hamiltonian flow](../../../classical-mechanics.md#hamiltonian-flow) satisfies

$$
\boxed{\dot I=0,\qquad\dot\theta=\nabla_I H(I).}
$$

Angles have period $2\pi$ here. The theorem is local near this regular compact component; it does not assert globally defined [action-angle variables](../../../classical-mechanics.md#action-angle-variables) across singular levels or over an entire base with monodromy.

First, $L$ has [dimension of a manifold](../../../topology.md#dimension-of-a-manifold) $n$ by the [submersion theorem](../../../differential-geometry.md#submersion-theorem). The [Hamiltonian vector fields](../../../symplectic-geometry.md#hamiltonian-vector-field) $X_{F_i}$ are independent, tangent to $L$, and commute. They span $TL$. Moreover

$$
\omega(X_{F_i},X_{F_j})=dF_i(X_{F_j})=\{F_i,F_j\}=0,
$$

so $L$ is a [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold). Compactness makes these restricted [vector fields](../../../calculus.md#vector-field) complete. Their joint flow is an $\mathbb R^n$-action on $L$. Its orbits are open because the fields span $TL$, so connectedness gives one orbit. The stabilizer $\Lambda$ of a point is discrete by the [inverse function theorem](../../../calculus.md#inverse-function-theorem), and

$$
L\cong\mathbb R^n/\Lambda.
$$

Compactness forces $\Lambda$ to be a full-rank [Euclidean lattice](../../../fourier-analysis.md#euclidean-lattice): otherwise an unbounded linear coordinate transverse to its span would descend to the quotient. Thus **$L$ is an $n$-torus**.

Next choose a small ball of regular values near $F(L)$ and a neighbourhood $N$ of this component which is a product family of compact tori $L_c$. This local trivialization follows directly by choosing transverse [vector fields](../../../calculus.md#vector-field) $Z_j$ with $dF_i(Z_j)=\delta_{ij}$ and lifting short radial paths in the base; compactness of $L$ gives a uniform neighbourhood where their flows exist. Hence $N$ deformation retracts onto $L$. The commuting joint flows on nearby fibres have smoothly varying full-rank [Hamiltonian period lattices](../../../classical-mechanics.md#hamiltonian-period-lattice). A basis $t^{(j)}(c)\in\mathbb R^n$ of their periods can be chosen smoothly on this small ball: continue the return equations from a basis at the central fibre, using their nonsingular vertical flow derivatives and the [implicit function theorem](../../../calculus.md#implicit-function-theorem). No global choice of lattice basis is needed.

Because $\omega|_L=0$ and $N$ retracts onto $L$, its closed [symplectic form](../../../symplectic-geometry.md#symplectic-form) is exact on $N$. Choose a one-form $\lambda$ with $d\lambda=-\omega$. Let $\gamma_j(c)$ be the smoothly continued cycles represented by the period basis and define the [action integrals](../../../classical-mechanics.md#action-integral)

$$
I_j(c)=\frac1{2\pi}\int_{\gamma_j(c)}\lambda.
$$

For a transverse variation $v$ of the fibre, differentiating a cycle integral and using [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) eliminates the integral of the exact term. With the cycle parametrized by the joint-flow time $t^{(j)}$, this gives

$$
dI_j(v)=\frac1{2\pi}\int_{\gamma_j}(-\omega(v,\dot\gamma_j))
=\frac1{2\pi}\sum_i t_i^{(j)}(c)\,dF_i(v).
$$

Thus

$$
\boxed{dI_j=\frac1{2\pi}\sum_i t_i^{(j)}(c)\,dc_i.}
$$

The period matrix is nonsingular, so $I$ gives coordinates on the base. The corresponding [Hamiltonian vector fields](../../../symplectic-geometry.md#hamiltonian-vector-field) satisfy

$$
X_{I_j}=\frac1{2\pi}\sum_i t_i^{(j)}(c)X_{F_i}.
$$

Their time-$2\pi$ flows return along the basis cycles. They commute because each $I_j$ is a function of the commuting $F_i$. Consequently they give a free [torus action](../../../lie-theory.md#torus-action) on $N$.

Choose a section over the action-coordinate ball and use this [torus action](../../../lie-theory.md#torus-action) to define angles $\theta$. Since $X_{I_j}=\partial_{\theta_j}$, the [symplectic form](../../../symplectic-geometry.md#symplectic-form) takes the form

$$
\omega=\sum_jd\theta_j\wedge dI_j+\beta(I).
$$

The closed base two-form $\beta$ is exact on the ball: write $\beta=d\alpha$, $\alpha=\sum_j a_j(I)dI_j$, by the [Poincaré lemma](../../../differential-form.md#poincare-lemma). Changing the angular origins by $\theta'_j=\theta_j+a_j(I)$ removes this term, since $\sum_jd\theta'_j\wedge dI_j=\omega$. This completes the construction of [action-angle variables](../../../classical-mechanics.md#action-angle-variables). The functions $F_i$ are constant on the fibres, so are functions of $I$ alone, and [Hamilton's equations](../../../classical-mechanics.md#hamilton-s-equations) give the claimed straight-line motion. This proves both the topological and symplectic parts of the [Arnold-Liouville theorem](../../../classical-mechanics.md#liouville-arnold-theorem).

## 4

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Take $\mathbb T=\mathbb R/(2\pi\mathbb Z)$ and $|k|_1=\sum_j|k_j|$. A [Diophantine frequency vector](../../../number-theory.md#diophantine-frequency-vector) satisfies

$$
\boxed{|k\cdot\omega|\ge\gamma |k|_1^{-\tau}\quad
(k\in\mathbb Z^n\setminus\{0\}).}
$$

Changing the norm only changes the admissible $\gamma$. The bound excludes resonances and quantifies the [small divisors](../../../number-theory.md#small-divisor) in the inverse of $\mathcal D_\omega$.

A periodic solution necessarily has zero-mean right-hand side, because the integral of each angular derivative vanishes. Conversely, if $\langle g\rangle=0$, expand its [Fourier series](../../../fourier-series.md):

$$
g(x)=\sum_k g_ke^{ik\cdot x},\qquad
f(x)=f_0+\sum_{k\ne0}\frac{g_k}{i\,k\cdot\omega}e^{ik\cdot x}.
$$

The [Diophantine condition](../../../number-theory.md#diophantine-frequency-vector) makes every denominator nonzero. These are all differentiable periodic solutions: any difference satisfies $\mathcal D_\omega h=0$ and has no nonzero [Fourier coefficient](../../../fourier-series.md#fourier-coefficient). Thus **a solution exists exactly for zero-mean $g$, and is unique up to a constant**; setting $\langle f\rangle=0$ fixes it. The analytic conclusion is on every strictly smaller complex strip, not necessarily the original boundary strip.

Shifting each contour in the [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) integral toward the appropriate edge of the complex strip gives

$$
|g_k|\le |g|_\sigma e^{-\sigma|k|_1}.
$$

Hence for $0<\delta<\sigma$,

$$
|f-\langle f\rangle|_{\sigma-\delta}
\le\frac{|g|_\sigma}{\gamma}\sum_{k\ne0}|k|_1^\tau e^{-\delta|k|_1}.
$$

This converges normally, including differentiated series on any still smaller strip, and proves both holomorphic extension and $\mathcal D_\omega f=g$. Real-valuedness follows from $g_{-k}=\overline{g_k}$ and the corresponding identity for $f_k$.

An explicit bound is obtained by counting lattice shells. The number of $k$ with $|k|_1=m$ is at most

$$
2^n\binom{m+n-1}{n-1}\le A_n m^{n-1},\qquad
A_n=\frac{2^n n^{n-1}}{(n-1)!}.
$$

Put $s=n+\tau$ and $p=s-1\ge0$. For $p>0$, $m^p e^{-\delta m/2}\le(2p/(e\delta))^p$; for $p=0$ use the bound $1$. Since $\sum_{m\ge1}e^{-\delta m/2}=(e^{\delta/2}-1)^{-1}\le2/\delta$, this gives

$$
\boxed{|f-\langle f\rangle|_{\sigma-\delta}
\le \frac{C_{n,\tau}}{\gamma\,\delta^{n+\tau}}|g|_\sigma,\qquad
C_{n,\tau}=2A_n\left(\frac{2(n+\tau-1)}e\right)^{n+\tau-1}.}
$$

Use $0^0=1$ in this constant when $n=1,\tau=0$. The estimate is valid for every positive $\delta$; optimality of the exponent is not needed. For a unit-period [flat torus](../../../second-fundamental-form.md#flat-torus), insert the factors $2\pi$ in both the Fourier exponent and denominator and adjust the constant.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Fix a smaller angular strip and a momentum ball $B'\Subset B$; the [canonical transformation](../../../classical-mechanics.md#canonical-transformation) will be defined there and map into the original domain for small $\epsilon$. This domain restriction is natural for a near-identity change of coordinates with a nonzero momentum shift.

First solve the scalar [cohomological equation on a Diophantine torus](../../../fourier-series.md#cohomological-equation-on-a-diophantine-torus)

$$
\mathcal D_\omega u=\langle V\rangle-V,\qquad\langle u\rangle=0.
$$

The preceding result gives a real-analytic periodic $u$ on every smaller strip. We need a near-identity angular [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) $\chi$ and a constant vector $a$ such that

$$
D\chi(\theta)\,\omega
=\omega+\epsilon\nabla u(\chi(\theta))+a,
\qquad\chi=\mathrm{id}+O(\epsilon),\quad a=O(\epsilon^2).
$$

Here is a complete analytic construction of this [translated conjugacy of a Diophantine vector field](../../../fourier-series.md#translated-conjugacy-of-a-diophantine-vector-field).

Write $w=\epsilon\nabla u$ and, for a current approximation, put

$$
A=D\chi,\qquad e=\mathcal D_\omega\chi-\omega-w\circ\chi-a.
$$

Assume $A$ is close to the identity. For a correction $\Delta\chi=A v$, the linearized defect is

$$
\mathcal D_\omega(Av)-Dw(\chi)Av-\Delta a
=A\mathcal D_\omega v+(De)v-\Delta a.
$$

The identity follows by differentiating the definition of $e$, so the term $(De)v$ already contains the current error. Choose

$$
\Delta a=\langle A^{-1}\rangle^{-1}\langle A^{-1}e\rangle,
\qquad
\mathcal D_\omega v=A^{-1}(\Delta a-e),\qquad\langle v\rangle=0.
$$

The matrix average is invertible near the identity, and the right-hand side has zero mean. The preceding [torus small-divisor estimate](../../../fourier-series.md#analytic-estimate-for-the-torus-cohomological-equation) therefore solves this vector equation componentwise. Update $\chi_+=\chi+Av$, $a_+=a+\Delta a$. The exact new error is

$$
e_+=(De)v-\bigl[w(\chi+Av)-w(\chi)-Dw(\chi)Av\bigr].
$$

It is quadratic in the current defect.

For convergence, reserve a fixed outer strip on which $w$ is analytic and work on shrinking inner strips whose total loss is less than half the starting width. Let $s=n+\tau$ and choose loss parameters $\delta_j=d\,2^{-j}$ with $0<d<1$ small enough that the fixed multiples of these losses used at each stage fit in the reserved total width. The [torus small-divisor estimate](../../../fourier-series.md#analytic-estimate-for-the-torus-cohomological-equation) and [Cauchy estimates](../../../analysis.md#cauchy-estimate) give, with constants uniform while $A$ stays close to the identity and $\chi$ remains in the reserved strip,

$$
\|v_j\|\le C\delta_j^{-s}\|e_j\|,\qquad
\|\Delta\chi_j\|_{C^1}\le C\delta_j^{-(s+1)}\|e_j\|,
\qquad\|\Delta a_j\|\le C\|e_j\|,
$$

and

$$
\|e_{j+1}\|\le C\delta_j^{-\mu}\|e_j\|^2,
\qquad\mu=2s+2.
$$

Indeed, the first remainder is bounded using $\|De_j\|\le C\delta_j^{-1}\|e_j\|$, and the second using the uniformly bounded second derivatives of $w$ on the reserved strip. Taking a slightly larger exponent $\mu$ covers all these losses. Start with $\chi_0=\mathrm{id}$ and $a_0=0$, so $e_0=-w=O(\epsilon)$. If a small constant $K$ satisfies $C d^{-\mu}K2^{2\mu}\le1$ and $\|e_0\|\le K$, induction gives $\|e_j\|\le K2^{-2\mu j}$. The estimates on $\Delta\chi_j$ and $\Delta a_j$ are summable. Choosing $\epsilon$ still smaller keeps the derivatives close to the identity and the images inside the reserved strip, closing the induction. The real periodic analytic limits $\chi,a$ solve the conjugacy equation. Since $\langle w\rangle=0$, the very first constant correction is zero; the first new defect is $O(\epsilon^2)$, and the remaining summed constant corrections are $O(\epsilon^2)$. Also the summed change of $\chi$ is $O(\epsilon)$. This proves the claimed estimates as well as existence, without leaving an unsolved linear remainder.

Now set $\eta(x)=\epsilon\nabla u(x)+a$ and define the [symplectic cotangent lift with a closed momentum shift](../../../symplectic-geometry.md#symplectic-cotangent-lift-with-a-closed-momentum-shift)

$$
\boxed{x=\chi(x'),\qquad
 y=\eta(\chi(x'))+D\chi(x')^{-T}y'.}
$$

The [cotangent lift of a diffeomorphism](../../../symplectic-geometry.md#cotangent-lift-of-a-diffeomorphism) is symplectic. Translation by $\eta$ is also symplectic because the one-form $\eta\cdot dx=\epsilon\,du+a\cdot dx$ is closed. The constant term need not be exact on the [flat torus](../../../second-fundamental-form.md#flat-torus); closedness is sufficient. Thus their composition is the required near-identity [canonical transformation](../../../classical-mechanics.md#canonical-transformation).

Expanding the quadratic kinetic term gives a transformed linear coefficient $D\chi^{-1}(\omega+\eta\circ\chi)$, which is exactly $\omega$ by the conjugacy equation. The constant-in-$y'$ part is

$$
\omega\cdot\eta+\epsilon V+\frac12|\eta|^2
=\epsilon\langle V\rangle+\omega\cdot a+\frac12|\eta|^2,
$$

since $\mathcal D_\omega u=\langle V\rangle-V$. Consequently define

$$
E_\epsilon=\epsilon\langle V\rangle+\omega\cdot a,
\qquad Q_\epsilon(x',y')=
 y'^T D\chi(x')^{-1}D\chi(x')^{-T}y',
$$

and, for $\epsilon\ne0$,

$$
\widetilde V_\epsilon(x')=\frac12\left|\nabla u(\chi(x'))+\frac a\epsilon\right|^2.
$$

In the exact identities, squared Euclidean norms mean the real polynomial $\sum_j v_j^2$, continued bilinearly on complex strips, without complex conjugation. The latter is uniformly bounded and analytic on the retained strip because $a=O(\epsilon^2)$. At $\epsilon=0$ use the identity map, $E_0=0$, and $Q_0=|y'|^2$. We have the **exact requested normal form**

$$
\boxed{H\circ\Phi=E_\epsilon+\omega\cdot y'
+\frac12Q_\epsilon(x',y')+\epsilon^2\widetilde V_\epsilon(x').}
$$

Here $E_\epsilon=O(\epsilon)$, $Q_\epsilon$ is genuinely homogeneous quadratic in $y'$, and its coefficient matrix differs from the identity by $O(\epsilon)$. Thus $|Q_\epsilon-|y'|^2|\le C|\epsilon|\,|y'|^2$. The remainder depends only on the angular coordinate. If the printed final $\widetilde V(x)$ uses the old angle $x$, the same term is $\tfrac12|\nabla u(x)+a/\epsilon|^2$ evaluated at $x=\chi(x')$; this is just the corresponding coordinate convention.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
