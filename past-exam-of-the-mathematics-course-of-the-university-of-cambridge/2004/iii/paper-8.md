# Paper 8

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper8.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper8.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
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
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)

## 1

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

A [Poisson structure](../../../symplectic-geometry.md#poisson-structure) is a real bilinear operation on [smooth functions](../../../analysis.md#smooth-function) on $M$,

$$
\{\cdot,\cdot\}:C^\infty(M)\times C^\infty(M)\longrightarrow C^\infty(M),
$$

which is antisymmetric, obeys the [Jacobi identity](../../../lie-algebra.md#jacobi-identity), and is a [derivation](../../../associative-algebra.md#derivation-of-an-algebra) in each argument. Explicitly,

$$
\{f,g\}=-\{g,f\},\qquad
\{f,\{g,h\}\}+\{g,\{h,f\}\}+\{h,\{f,g\}\}=0,\qquad
\{f,gh\}=\{f,g\}h+g\{f,h\}.
$$

Antisymmetry supplies the corresponding [Leibniz rule](../../../calculus.md#leibniz-rule) in the first argument. Equivalently it is a smooth [Poisson bivector](../../../symplectic-geometry.md#poisson-bivector) $\Pi$ with $\{f,g\}=\Pi(df,dg)$ and $[\Pi,\Pi]=0$ for the [Schouten-Nijenhuis bracket](../../../linear-algebra.md#schouten-nijenhuis-bracket). In local coordinates,

$$
\{f,g\}=\sum_{i,j}\Pi^{ij}(x)\partial_i f\partial_j g,\qquad
\Pi^{ij}=-\Pi^{ji},\qquad
\sum_l\left(\Pi^{il}\partial_l\Pi^{jk}+\Pi^{jl}\partial_l\Pi^{ki}+\Pi^{kl}\partial_l\Pi^{ij}\right)=0.
$$

The last equation is the coordinate [Jacobi identity](../../../lie-algebra.md#jacobi-identity). Nondegeneracy is not part of the definition: a [Poisson structure](../../../symplectic-geometry.md#poisson-structure) may have [Casimir functions](../../../symplectic-geometry.md#casimir-function-of-a-poisson-manifold) and [symplectic leaves](../../../symplectic-geometry.md#symplectic-leaf) of different dimensions.

A [Hamiltonian system](../../../classical-mechanics.md#hamiltonian-system) consists of such a [Poisson manifold](../../../symplectic-geometry.md#poisson-manifold), a [Hamiltonian](../../../classical-mechanics.md#hamiltonian) $H\in C^\infty(M)$, and the flow of its [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field). Choose the convention

$$
\boxed{X_H(f)=\{f,H\},\qquad \dot x^i=\sum_j\Pi^{ij}\partial_jH.}
$$

For an observable with no explicit time dependence, $df/dt=\{f,H\}$. In particular $H$ is conserved because $\{H,H\}=0$. For the canonical [Poisson bracket](../../../classical-mechanics.md#poisson-bracket), this convention gives $\dot q_i=\partial H/\partial p_i$ and $\dot p_i=-\partial H/\partial q_i$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

For the [Arnold-Liouville theorem](../../../classical-mechanics.md#liouville-arnold-theorem), work on a [symplectic manifold](../../../symplectic-geometry.md#symplectic-manifold) of dimension $2d$. Let $F_1=H,F_2,\ldots,F_d$ be [smooth functions](../../../analysis.md#smooth-function) with pairwise vanishing [Poisson brackets](../../../classical-mechanics.md#poisson-bracket), and suppose

$$
dF_1\wedge\cdots\wedge dF_d\ne0
$$

on a connected component $N$ of a common level. If $N$ is compact, then **$N$ is a $d$-dimensional [torus](../../../topology.md#torus)**. Its commuting [Hamiltonian vector fields](../../../symplectic-geometry.md#hamiltonian-vector-field) generate translations, and the [Hamiltonian](../../../classical-mechanics.md#hamiltonian) motion on it is linear in angular coordinates. Compactness ensures completeness of these restricted [vector fields](../../../calculus.md#vector-field).

Moreover a neighbourhood of $N$ admits [action-angle variables](../../../classical-mechanics.md#action-angle-variables) $(I_1,\ldots,I_d,\theta_1,\ldots,\theta_d)$, with each angle defined modulo $2\pi$, for which

$$
\{\theta_i,I_j\}=\delta_{ij},\qquad
\{I_i,I_j\}=\{\theta_i,\theta_j\}=0,\qquad
F_j=F_j(I_1,\ldots,I_d).
$$

One compatible [symplectic form](../../../symplectic-geometry.md#symplectic-form) convention is $\omega=\sum_i d\theta_i\wedge dI_i$. The equations become

$$
\boxed{\dot I_i=0,\qquad \dot\theta_i=\frac{\partial H}{\partial I_i},\qquad
\theta_i(t)=\theta_i(0)+t\frac{\partial H}{\partial I_i}(I(0)).}
$$

The resulting motion is periodic when the frequencies are commensurable and otherwise quasiperiodic on a subtorus. This is [Liouville integrability](../../../classical-mechanics.md#integrable-hamiltonian-system) with $d$ independent [first integrals in involution](../../../classical-mechanics.md#first-integrals-in-involution). Compactness and regularity cannot be discarded from the [torus](../../../topology.md#torus) conclusion. On a general [Poisson manifold](../../../symplectic-geometry.md#poisson-manifold), apply this theorem on a regular [symplectic leaf](../../../symplectic-geometry.md#symplectic-leaf) of dimension $2d$; the ambient dimension alone does not specify the required number of integrals.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

A field $u(x,t)$ has infinitely many degrees of freedom: its initial state is a [function](../../../function.md) rather than a finite list of coordinates. For a [Hamiltonian](../../../classical-mechanics.md#hamiltonian) evolution, the analogue of the finite-dimensional construction seeks an infinite sequence of independent conserved [functionals](../../../calculus-of-variations.md#functional) $H_j[u]$ whose [Poisson brackets](../../../classical-mechanics.md#poisson-bracket) vanish. Their [Hamiltonian vector fields](../../../symplectic-geometry.md#hamiltonian-vector-field) then define commuting time evolutions. For example, a [Poisson operator](../../../symplectic-geometry.md#poisson-operator) $J$ produces the field equation $u_t=J\,\delta H/\delta u$, where $\delta H/\delta u$ is the [variational derivative](../../../classical-mechanics.md#variational-derivative).

A [Lax equation](../../../integrable-systems.md#isospectral-lax-equation) packages many conservation laws into one operator identity. If $L_t=[A,L]$, cyclicity of an appropriate trace gives

$$
\frac{d}{dt}\operatorname{Tr}(L^r)
=r\operatorname{Tr}(L^{r-1}[A,L])
=r\operatorname{Tr}([A,L^r])=0.
$$

For a [formal pseudodifferential operator](../../../analysis.md#formal-pseudodifferential-operator) the relevant trace is the [Adler trace](../../../analysis.md#adler-trace); suitable fractional powers of a monic [differential operator](../../../analysis.md#differential-operator) produce further conserved [functionals](../../../calculus-of-variations.md#functional). A [Lenard-Magri recursion](../../../symplectic-geometry.md#lenard-magri-recursion) can prove that such [functionals](../../../calculus-of-variations.md#functional) are [Poisson-commuting functions](../../../classical-mechanics.md#poisson-commuting-functions), rather than merely [conserved quantities](../../../classical-mechanics.md#conserved-quantity). A [Lax equation](../../../integrable-systems.md#isospectral-lax-equation) by itself does not establish all the independence and completeness properties needed for integrability.

The [Korteweg-De Vries equation](../../../integrable-systems.md#korteweg-de-vries-equation) illustrates the mechanism. In one time normalization take $L=\partial^2+u$ and $A=\partial^3+\tfrac32u\partial+\tfrac34u_x$. Direct composition gives

$$
L_t=[A,L]\quad\Longleftrightarrow\quad
u_t=\frac14u_{xxx}+\frac32u u_x.
$$

Its spectral problem, together with the [inverse scattering transform](../../../integrable-systems.md#inverse-scattering-transform) for decaying data or suitable spectral coordinates for periodic data, turns nonlinear evolution into simple evolution of spectral data. Solitary waves arise from discrete spectral data, while continuous data describe dispersive radiation.

Thus [infinite-dimensional Hamiltonian integrability](../../../integrable-systems.md#infinite-dimensional-hamiltonian-integrability) is more than an infinite list of formulas: one wants sufficiently complete commuting invariants and a reconstruction mechanism that solves the evolution. [Boundary conditions](../../../differential-equation.md#boundary-condition) and the [function](../../../function.md) space are essential. A formal hierarchy need not converge, and an infinite family of [conserved quantities](../../../classical-mechanics.md#conserved-quantity) does not automatically give a compact infinite-dimensional [torus](../../../topology.md#torus) or an unrestricted analogue of the [Arnold-Liouville theorem](../../../classical-mechanics.md#liouville-arnold-theorem).

## 2

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

First let $n\geq0$. The ordinary [Leibniz rule](../../../calculus.md#leibniz-rule), applied to a test [function](../../../function.md) $h$, gives

$$
\partial^n(fh)=\sum_{r=0}^n\binom nr f^{(r)}h^{(n-r)}.
$$

Equivalently, the composition of [differential operators](../../../analysis.md#differential-operator) is

$$
\boxed{\partial^n m_f=\sum_{r=0}^n\binom nr m_{f^{(r)}}\partial^{n-r}.}
$$

For completeness, this formula follows by [induction](../../../foundations-of-mathematics.md#mathematical-induction): applying $\partial$ differentiates either the [coefficient](../../../vector-space.md#coefficient) or the remaining [derivative](../../../calculus.md#derivative) of $h$, and the two contributions combine by $\binom nr+\binom n{r-1}=\binom{n+1}r$. The initial case is multiplication by $f$.

For all [integers](../../../number-theory.md#integer) $n$, define $\binom n0=1$ and $\binom nr=n(n-1)\cdots(n-r+1)/r!$. The [formal pseudodifferential composition rule](../../../analysis.md#formal-pseudodifferential-composition-rule) is

$$
\boxed{\partial^n m_f=\sum_{r\geq0}\binom nr m_{f^{(r)}}\partial^{n-r},\qquad n\in\mathbb Z.}
$$

For $n=-s<0$, $\binom{-s}r=(-1)^r\binom{s+r-1}r$, so this is usually an infinite series. In particular

$$
\partial^{-1}m_f=m_f\partial^{-1}-m_{f'}\partial^{-2}+m_{f''}\partial^{-3}-\cdots.
$$

Applying $\partial$ on the left gives $m_f$: all later [coefficient](../../../vector-space.md#coefficient) [derivatives](../../../calculus.md#derivative) cancel in pairs. This uniquely determines the normal-ordered inverse expansion. Repeating the inverse construction, or using the same binomial recurrence downward in $n$, gives every negative power. More explicitly, applying $\partial$ to the proposed $n$-series yields [coefficient](../../../vector-space.md#coefficient) $\binom nr+\binom n{r-1}=\binom{n+1}r$ at $f^{(r)}\partial^{n+1-r}$, so it is consistent with the already determined $(n+1)$-series. Negative powers here are formal; differentiation on all of $C^\infty(\mathbb R)$ has a nontrivial kernel and has no genuine two-sided inverse there.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Use the [formal pseudodifferential composition rule](../../../analysis.md#formal-pseudodifferential-composition-rule) on each [coefficient](../../../vector-space.md#coefficient) $w_i(x)$ and then the exponential eigenfunction convention. For every [integer](../../../number-theory.md#integer) $n$,

$$
\partial^n\bigl(w_i(x)e^{kx}\bigr)
=e^{kx}\sum_{r\geq0}\binom nr w_i^{(r)}(x)k^{n-r}.
$$

Consequently

$$
Pw=k^\beta e^{kx}\sum_{j,i,r\geq0}
g_j\binom{\alpha-j}{r}w_i^{(r)}k^{\alpha-j-i-r}.
$$

Collecting all terms of a fixed power of the spectral parameter gives the useful answer

$$
\boxed{Pw=k^{\alpha+\beta}e^{kx}\sum_{s\geq0}\frac{v_s(x)}{k^s},\qquad
v_s=\sum_{i+j+r=s}g_j\binom{\alpha-j}{r}w_i^{(r)}.}
$$

The sum defining each $v_s$ is finite. For example,

$$
v_0=g_0w_0,\qquad
v_1=g_0w_1+g_1w_0+\alpha g_0w_0',
$$

and

$$
v_2=g_0w_2+g_1w_1+g_2w_0+\alpha g_0w_1'
+(\alpha-1)g_1w_0'+\binom\alpha2g_0w_0''.
$$

This is the action on a [formal pseudodifferential wave function](../../../analysis.md#formal-pseudodifferential-wave-function). It is a formal expansion near $k=\infty$, with $k^\beta$ carried as a formal prefactor. It does not assert convergence for finite $k$, and negative powers are not evaluated at $k=0$.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Write the two [formal pseudodifferential operators](../../../analysis.md#formal-pseudodifferential-operator) in normal order as

$$
P_1=a\partial^p+a_1\partial^{p-1}+\cdots,\qquad
P_2=b\partial^q+b_1\partial^{q-1}+\cdots,
$$

where $p=\alpha_1$ and $q=\alpha_2$. The [formal pseudodifferential composition rule](../../../analysis.md#formal-pseudodifferential-composition-rule) gives

$$
P_1P_2=ab\partial^{p+q}
+\bigl(pa b'+ab_1+a_1b\bigr)\partial^{p+q-1}+\cdots.
$$

Thus $\boxed{\operatorname{ord}(P_1P_2)=p+q}$ whenever $ab$ is not identically zero, in particular when both leading [coefficients](../../../vector-space.md#coefficient) are nowhere zero. In general the rigorous statement over the specified [coefficient](../../../vector-space.md#coefficient) algebra is $\operatorname{ord}(P_1P_2)\leq p+q$.

The leading scalar [coefficients](../../../vector-space.md#coefficient) commute. Subtracting the reversed composition also cancels the terms involving $a_1,b_1$, leaving

$$
[P_1,P_2]=(pa b'-qb a')\partial^{p+q-1}+\cdots.
$$

Therefore the [order filtration of formal pseudodifferential operators](../../../analysis.md#order-filtration-of-formal-pseudodifferential-operators) gives

$$
\boxed{\operatorname{ord}[P_1,P_2]\leq p+q-1,}
$$

with equality precisely when the displayed [coefficient](../../../vector-space.md#coefficient) is not identically zero. The bound can be strict: constant-coefficient powers of $\partial$ commute, giving the zero operator, whose order can be assigned $-\infty$.

There is also a genuine qualification to product-order addition in $C^\infty(\mathbb R)$. Choose nonzero [smooth functions](../../../analysis.md#smooth-function) $a,b$ with disjoint [compact supports](../../../function.md#compact-support) and take $P_1=m_a,P_2=m_b$. Each has order zero, but their product is zero. Nonzero [coefficients](../../../vector-space.md#coefficient) as elements of this algebra need not have a nonzero product. Thus an unqualified assertion of exact product order requires an additional leading-symbol hypothesis.

## 3

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Put every [formal pseudodifferential operator](../../../analysis.md#formal-pseudodifferential-operator) in normal order, with all [coefficient](../../../vector-space.md#coefficient) [functions](../../../function.md) on the left. Its [formal pseudodifferential residue](../../../analysis.md#formal-pseudodifferential-residue) is the [coefficient](../../../vector-space.md#coefficient) of $\partial^{-1}$. The [Adler trace](../../../analysis.md#adler-trace) is

$$
\boxed{\operatorname{Tr}P=\int\operatorname{res}P\,dx.}
$$

Here and below, use periodic [coefficients](../../../vector-space.md#coefficient) and integrate over a period, or impose convergence and vanishing boundary terms on the real line. Equivalently, the algebraic integration [functional](../../../calculus-of-variations.md#functional) must annihilate total [derivatives](../../../calculus.md#derivative). This convention is needed for the requested trace property; arbitrary elements of $C^\infty(\mathbb R)$ do not supply it automatically.

It suffices to compute with monomials $A=a\partial^p$, $B=b\partial^q$. Write $r=p+q+1$. If $r<0$, no term in either product has power $\partial^{-1}$, so both residues are zero. If $r\geq0$, the [formal pseudodifferential composition rule](../../../analysis.md#formal-pseudodifferential-composition-rule) gives

$$
\operatorname{res}(AB)=\binom pr a b^{(r)},\qquad
\operatorname{res}(BA)=\binom qr b a^{(r)}.
$$

Since $q=r-1-p$, reversal of the factors in the numerator proves

$$
\binom qr=\frac{(r-1-p)\cdots(-p)}{r!}=(-1)^r\binom pr.
$$

After $r$ integrations by parts, $\int ab^{(r)}dx=(-1)^r\int ba^{(r)}dx$. Hence the two product traces agree. More explicitly, for $r\geq1$ their residue difference is the total [derivative](../../../calculus.md#derivative)

$$
\operatorname{res}[A,B]
=\binom pr\frac{d}{dx}\left(\sum_{j=0}^{r-1}(-1)^j a^{(j)}b^{(r-1-j)}\right).
$$

For $r=0$ the residue difference is $ab-ba=0$. In products of operators bounded above in order, only finitely many monomial pairs can contribute to a residue: the required $r$ is nonnegative, so the two downward [coefficient](../../../vector-space.md#coefficient) indices have a bounded sum. Summing the monomial result therefore proves

$$
\boxed{\operatorname{Tr}[P_1,P_2]=0,\qquad
\operatorname{Tr}(P_1P_2)=\operatorname{Tr}(P_2P_1).}
$$

The boundary convention is substantive. Without it, take $A=\partial^2$, $B=(\tanh x)\partial^{-2}$. Both individual residues vanish, but $\operatorname{res}[A,B]=2(\tanh x)'=2\operatorname{sech}^2x$ and its integral over $\mathbb R$ is $4$, not zero. The primitive has unequal limits at the two ends. Also a generic smooth residue need not have a convergent integral at all. Thus the proof supplies the intended cyclic trace under its necessary analytic or formal integration convention.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Write $P=\sum_{j\leq\alpha}p_j(x)\partial^j$, setting unused [coefficients](../../../vector-space.md#coefficient) to zero. Split the [Adler trace](../../../analysis.md#adler-trace) into its fixed leading part and variable parts:

$$
l_P(L)=\operatorname{Tr}(P\partial^m)
+\sum_{l=0}^{m-1}\operatorname{Tr}(P u_l\partial^l).
$$

Cyclicity from part (i) gives

$$
\operatorname{Tr}(P u_l\partial^l)
=\operatorname{Tr}(u_l\partial^lP)
=\int u_l\operatorname{res}(\partial^lP)\,dx.
$$

Thus this [Hamiltonian trace functional on monic differential operators](../../../analysis.md#hamiltonian-trace-functional-on-monic-differential-operators) has the required form

$$
\boxed{l_P(L)=c+\sum_{l=0}^{m-1}\int a_l(x)u_l(x)\,dx,\qquad
c=\int p_{-m-1}(x)\,dx,\quad a_l=\operatorname{res}(\partial^lP).}
$$

To make each [coefficient](../../../vector-space.md#coefficient) explicit, expand $\partial^lp_j$ by the [Leibniz rule](../../../calculus.md#leibniz-rule). A term with $k$ [derivatives](../../../calculus.md#derivative) of $p_j$ contributes to the residue exactly when $l-k+j=-1$. Consequently,

$$
\boxed{a_l(x)=\sum_{k=0}^l\binom lk p_{k-l-1}^{(k)}(x).}
$$

These are [smooth functions](../../../analysis.md#smooth-function) depending on $P$, not on the variable [coefficients](../../../vector-space.md#coefficient) of $L$. In particular $a_0=p_{-1}$ and $a_1=p_{-2}+p_{-1}'$. The [coefficient](../../../vector-space.md#coefficient) $a_0$ must be included: it appears in the displayed sum even though the printed [coefficient](../../../vector-space.md#coefficient) list starts at $a_1$.

The monic operators form an [affine space](../../../geometry-and-topology.md#affine-space), not a vector space. Accordingly $l_P$ is affine in the coordinates $u_l$, with constant $c$, and its differential is linear in variations. Its [variational derivatives](../../../classical-mechanics.md#variational-derivative) are $\delta l_P/\delta u_l=a_l$. It is the restriction of a linear trace pairing on the full operator space, which explains the terminology without discarding the constant term.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Use the canonical representatives of [functionals](../../../calculus-of-variations.md#functional) of $u$: $P_f=f\partial^{-1}$, $P_g=g\partial^{-1}$. The [formal pseudodifferential composition rule](../../../analysis.md#formal-pseudodifferential-composition-rule) gives

$$
P_fP_g=fg\partial^{-2}-fg'\partial^{-3}+fg''\partial^{-4}+\cdots,
$$

and the reversed product has $f,g$ exchanged. Therefore

$$
[P_f,P_g]=(gf'-fg')\partial^{-3}+(fg''-gf'')\partial^{-4}+\cdots.
$$

Multiplying by $L=\partial^2+u$ on the left, only the leading displayed [commutator](../../../lie-algebra.md#commutator) term can produce a residue. Differentiation of its [coefficient](../../../vector-space.md#coefficient) produces powers at most $\partial^{-2}$, and multiplication by $u$ produces powers at most $\partial^{-3}$. Thus

$$
\operatorname{res}\bigl(L[P_f,P_g]\bigr)=gf'-fg',
$$

and, with the trace convention of part (i),

$$
\boxed{\{l_{P_f},l_{P_g}\}(L)=\int(gf'-fg')\,dx=-2\int fg'\,dx.}
$$

There is no $u$ dependence in this bracket.

Moreover $\operatorname{res}(P_fL)=fu$, so $l_{P_f}=\int fu\,dx$ and $\delta l_{P_f}/\delta u=f$. If $K(x,y)=\{u(x),u(y)\}$ is the distributional field bracket, it is characterized by

$$
\iint f(x)g(y)K(x,y)\,dx\,dy=-2\int f(x)g'(x)\,dx.
$$

Since $\int\partial_x\delta(x-y)g(y)\,dy=g'(x)$, the answer is

$$
\boxed{\{u(x),u(y)\}=-2\partial_x\delta(x-y)=2\partial_y\delta(x-y).}
$$

The [Dirac delta](../../../distribution-theory.md#dirac-delta-function) is periodic in the periodic setting, or the ordinary [Dirac delta](../../../distribution-theory.md#dirac-delta-function) on the real line with admissible test [functions](../../../function.md). This is the [first Hamiltonian structure of the KdV equation](../../../integrable-systems.md#first-hamiltonian-structure-of-the-kdv-equation), with [Poisson operator](../../../symplectic-geometry.md#poisson-operator) $-2\partial_x$. Its skewness follows by [integration by parts](../../../calculus.md#integration-by-parts); its [coefficients](../../../vector-space.md#coefficient) are constant, so the [functional](../../../calculus-of-variations.md#functional) [Jacobi identity](../../../lie-algebra.md#jacobi-identity) has no coefficient-variation terms.

A qualification is needed if the displayed trace formula is interpreted as a bracket on the reduced space for arbitrary operator representatives. Multiplication by a [function](../../../function.md) $h$ gives $l_{m_h}(\partial^2+u)=0$, yet direct expansion gives

$$
\operatorname{res}\bigl(L[m_h,g\partial^{-1}]\bigr)
=2(gh')'-gh'',\qquad
\operatorname{Tr}\bigl(L[m_h,g\partial^{-1}]\bigr)=-\int gh''\,dx.
$$

With $h=g=\cos x$ on a period $[0,2\pi]$, the latter is $\pi$. Hence the formula does not descend through every possible representative of a [functional](../../../calculus-of-variations.md#functional) on this reduced [affine space](../../../geometry-and-topology.md#affine-space). The requested $f\partial^{-1},g\partial^{-1}$ representatives, used consistently for variational gradients, give the well-defined constant field bracket just computed; a general restriction from the ambient operator algebra needs an appropriate reduction.

## 4

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The [coefficients](../../../vector-space.md#coefficient) of the formal series must be [smooth functions](../../../analysis.md#smooth-function) $H_n\in C^\infty(M)$, rather than points of $M$. Interpret complex parameter values in the complexified [function](../../../function.md) algebra. The [Casimir function](../../../symplectic-geometry.md#casimir-function-of-a-poisson-manifold) condition for the [Poisson pencil](../../../symplectic-geometry.md#poisson-pencil) is a coefficientwise formal identity:

$$
0=\{H,f\}_\lambda
=\{H_0,f\}_1+\sum_{n\geq1}\lambda^n
\left(\{H_n,f\}_1+\{H_{n-1},f\}_2\right).
$$

Equality of the formal [coefficients](../../../vector-space.md#coefficient) proves

$$
\boxed{\{H_0,f\}_1=0,\qquad
\{H_n,f\}_1=-\{H_{n-1},f\}_2\quad(n\geq1).}
$$

These are the [Lenard-Magri recursion](../../../symplectic-geometry.md#lenard-magri-recursion) relations, valid for every [smooth function](../../../analysis.md#smooth-function) $f$.

For $i\geq1$ and $j\geq0$, use the recursion in the first argument, then antisymmetry and the recursion in the second:

$$
\{H_i,H_j\}_1=-\{H_{i-1},H_j\}_2
=\{H_{i-1},H_{j+1}\}_1.
$$

Each step lowers the first index while raising the second. Iterating $i$ times gives

$$
\{H_i,H_j\}_1=\{H_0,H_{i+j}\}_1=0,
$$

because $H_0$ is a [Casimir function](../../../symplectic-geometry.md#casimir-function-of-a-poisson-manifold) of the first [Poisson structure](../../../symplectic-geometry.md#poisson-structure). This includes $i=0$ directly. The recursion one step higher then gives

$$
\{H_i,H_j\}_2=-\{H_{i+1},H_j\}_1=0.
$$

Thus the [commuting coefficients of a Poisson pencil Casimir](../../../symplectic-geometry.md#commuting-coefficients-of-a-poisson-pencil-casimir) satisfy

$$
\boxed{\{H_i,H_j\}_1=\{H_i,H_j\}_2=0\qquad(i,j\geq0).}
$$

They are therefore [Poisson-commuting functions](../../../classical-mechanics.md#poisson-commuting-functions) for every member of the [Poisson pencil](../../../symplectic-geometry.md#poisson-pencil). The argument proves involution, not [functional independence](../../../calculus.md#functionally-independent-functions); an infinite sequence can contain repetitions or zero [coefficients](../../../vector-space.md#coefficient).

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The intended construction is to solve the [Lenard-Magri recursion](../../../symplectic-geometry.md#lenard-magri-recursion) one step at a time. With $H_0$ a [Casimir function](../../../symplectic-geometry.md#casimir-function-of-a-poisson-manifold) of the first [Poisson structure](../../../symplectic-geometry.md#poisson-structure), seek $H_n$ satisfying

$$
\boxed{X^{(1)}_{H_n}=-X^{(2)}_{H_{n-1}},\quad\text{equivalently}\quad
\Pi_1dH_n=-\Pi_2dH_{n-1}.}
$$

Here $X_H^{(a)}f=\{f,H\}_a$, consistently with part 1(i). If every step can be solved by a globally defined [smooth function](../../../analysis.md#smooth-function), the formal series $\sum_{n\geq0}H_n\lambda^n$ is a [Casimir function](../../../symplectic-geometry.md#casimir-function-of-a-poisson-manifold) for the [Poisson pencil](../../../symplectic-geometry.md#poisson-pencil), and part (i) proves that all the $H_n$ are [Poisson-commuting functions](../../../classical-mechanics.md#poisson-commuting-functions) for every parameter value after complexification.

The recursive step is a concrete potential problem. Put $Y=-X^{(2)}_{H_{n-1}}$. It must first be tangent to the [symplectic leaves](../../../symplectic-geometry.md#symplectic-leaf) of $\Pi_1$. On a regular leaf use [canonical coordinates](../../../classical-mechanics.md#canonical-variables) $(q_i,p_i)$. The required equations are

$$
\frac{\partial H_n}{\partial p_i}=Y^{q_i},\qquad
\frac{\partial H_n}{\partial q_i}=-Y^{p_i}.
$$

Thus the leaf one-form

$$
\alpha_Y=\sum_i\left(-Y^{p_i}\,dq_i+Y^{q_i}\,dp_i\right)
$$

must be exact. Where it is closed on a contractible coordinate domain, define $H_n$ by integrating $\alpha_Y$ from a base point; path independence follows from closedness. A [function](../../../function.md) of the leaf labels can be added, corresponding to a [Casimir function](../../../symplectic-geometry.md#casimir-function-of-a-poisson-manifold) of the first [Poisson structure](../../../symplectic-geometry.md#poisson-structure). Global solvability also requires vanishing periods and smooth matching between leaves. This describes how to perform each solvable step without pretending that a degenerate [Poisson structure](../../../symplectic-geometry.md#poisson-structure) can simply be inverted.

Compatibility alone does not ensure these solvability conditions. There is an immediate [obstruction to a Lenard-Magri recursion](../../../symplectic-geometry.md#obstruction-to-a-lenard-magri-recursion) even in two dimensions. On $M=\mathbb R^2$ take

$$
\{f,g\}_1=0,\qquad
\{f,g\}_2=f_xg_y-f_yg_x,\qquad H_0=x.
$$

Both are [Poisson structures](../../../symplectic-geometry.md#poisson-structure), and their linear combination is a scalar multiple of the canonical [Poisson bracket](../../../classical-mechanics.md#poisson-bracket), so they are compatible. Every [function](../../../function.md), including $H_0$, is a [Casimir function](../../../symplectic-geometry.md#casimir-function-of-a-poisson-manifold) for the first bracket. But the first recursion, evaluated at $f=y$, would require

$$
0=\{H_1,y\}_1=-\{x,y\}_2=-1,
$$

a contradiction. **An arbitrary initial Casimir need not extend even to $H_1$.** Consequently the unconditional existence assertion requires an additional hypothesis: the indicated [vector field](../../../calculus.md#vector-field) must be [Hamiltonian](../../../classical-mechanics.md#hamiltonian) for $\Pi_1$ at every step. Under that hypothesis the recursive construction and involution proof above complete the intended result; without it the counterexample rules out the requested infinite extension.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
