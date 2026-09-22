# Paper 44

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_44.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_44.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a [unitary matrix](../../../linear-operator-theory.md#unitary-matrix), $UU^\dagger=1$, so $(U^\dagger MU)^r=U^\dagger M^rU$. Cyclicity of the [trace](../../../linear-algebra.md#matrix-trace) then gives $\operatorname{tr}(U^\dagger M^rU)=\operatorname{tr}(M^r)$ for both powers entering the action. Thus **the action is invariant under unitary conjugation**.

The [spectral theorem for normal operators](../../../hilbert-space.md#spectral-theorem-for-normal-operators) diagonalizes a finite-dimensional [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) by a [unitary matrix](../../../linear-operator-theory.md#unitary-matrix). Applying the invariance to that diagonal form gives

$$
\boxed{V(M)=\sum_{i=1}^N\left(\frac{\lambda_i^2}{2}+\frac g4\lambda_i^4\right).}
$$

Only the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) enter, not the choice of [eigenvectors](../../../linear-operator-theory.md#eigenvector).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Use the normalized Gaussian integral with action $\operatorname{tr}(M^2)/2$. Its [Wick contraction](../../../perturbative-quantum-field-theory.md#wick-contraction) is

$$
\langle M^i{}_j M^k{}_l\rangle_0=\delta^i{}_l\delta^k{}_j.
$$

There is no factor $1/N$ here: this part uses $V$, whereas the following part uses $NV$. Expanding the normalized [Hermitian matrix model](../../../perturbative-quantum-field-theory.md#hermitian-matrix-model) integral to first order gives

$$
\langle M^i{}_j M^k{}_l\rangle
=\langle M^i{}_j M^k{}_l\rangle_0-\frac g4\left[
\langle M^i{}_j M^k{}_l\operatorname{tr}(M^4)\rangle_0
-\langle M^i{}_j M^k{}_l\rangle_0\langle\operatorname{tr}(M^4)\rangle_0\right]+O(g^2).
$$

The subtracted term removes [Vacuum Feynman diagrams](../../../perturbative-quantum-field-theory.md#vacuum-feynman-diagram) disconnected from the external pair. Since the one-point function vanishes by $M\mapsto-M$, the resulting two-point function is a [connected correlation function](../../../critical-phenomenon.md#connected-correlation-function).

Write the vertex as $M^a{}_bM^b{}_cM^c{}_dM^d{}_a$. Each external field must contract with a different vertex field, leaving the other two to form a [tadpole diagram](../../../perturbative-quantum-field-theory.md#tadpole-diagram). Eight of the twelve connected pairings attach the external fields at adjacent cyclic positions. The remaining index loop gives $N\delta^i{}_l\delta^k{}_j$ in each case. The other four attach them at opposite positions and give $\delta^i{}_j\delta^k{}_l$, with no free index loop. Therefore

$$
\boxed{\langle M^i{}_j M^k{}_l\rangle_c
=(1-2gN)\delta^i{}_l\delta^k{}_j-g\delta^i{}_j\delta^k{}_l+O(g^2).}
$$

**Both index structures are required at finite $N$**. For $N=1$ the answer is $1-3g+O(g^2)$, agreeing with the ordinary zero-dimensional quartic integral. This is a formal [perturbative quantum field theory](../../../perturbative-quantum-field-theory.md) expansion; the real integral is convergent for $g\ge0$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The off-diagonal auxiliary integrations impose $M^i{}_j=0$ for $i\ne j$, by the Fourier representation of a [Dirac delta function](../../../distribution-theory.md#dirac-delta-function). After this constraint, $M=\operatorname{diag}(\lambda_1,\ldots,\lambda_N)$ and

$$
[M,C]^i{}_j=(\lambda_i-\lambda_j)C^i{}_j,\qquad
\operatorname{tr}(B[M,C])=\sum_{i\ne j}B^j{}_i(\lambda_i-\lambda_j)C^i{}_j.
$$

The [Grassmann Gaussian integral](../../../quantum-field-theory.md#grassmann-gaussian-integral) over each off-diagonal pair gives its coefficient. Consequently the ghost determinant is

$$
\det{}'\operatorname{ad}_M=\prod_{i\ne j}(\lambda_i-\lambda_j)
=(-1)^{N(N-1)/2}\prod_{i<j}(\lambda_i-\lambda_j)^2.
$$

The prime omits the diagonal directions, which were excluded from the outset. The constant sign depends on the [Berezin integral](../../../quantum-mechanics.md#berezin-integral) ordering and can be absorbed in normalization. Thus the [Vandermonde determinant](../../../galois-theory.md#vandermonde-determinant) squared is the eigenvalue measure factor in this [matrix diagonalization ghost determinant](../../../perturbative-quantum-field-theory.md#matrix-diagonalization-ghost-determinant).

Up to an eigenvalue-independent constant, the remaining integral is $\int\prod_i d\lambda_i\,e^{-S_{\rm eig}}$, where

$$
\boxed{S_{\rm eig}=N\sum_i\left(\frac{\lambda_i^2}{2}+\frac g4\lambda_i^4\right)
-2\sum_{i<j}\log|\lambda_i-\lambda_j|.}
$$

**The determinant supplies logarithmic eigenvalue repulsion**. An ordering restriction on the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) changes only a constant factorial; no remaining eigenvalue integral needs to be performed. The off-diagonal bosonic contours and the displayed normalization are understood in the usual Fourier-delta prescription.

## 2

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

In the [Wilsonian effective action](../../../perturbative-quantum-field-theory.md#wilsonian-effective-action) picture, integrate out field modes in a high-[momentum](../../../classical-mechanics.md#momentum) shell and encode their effects in the action for the retained modes. Rescale lengths and fields to compare the resulting theory at the original cutoff. The couplings then follow a [renormalization-group flow](../../../critical-phenomenon.md#renormalization-group-flow), while low-energy predictions are preserved. In general all local interactions allowed by the symmetries are generated, even if only a few appear in the initial action.

Near a [renormalization-group fixed point](../../../critical-phenomenon.md#renormalization-group-fixed-point), a perturbation $u\int d^dx\,\mathcal O(x)$ with scaling dimension $\Delta$ has linearized eigenvalue $y=d-\Delta$. Under coarse graining by $b>1$, its dimensionless coupling scales as $u'\simeq b^yu$. A [relevant operator](../../../critical-phenomenon.md#relevant-operator) has $y>0$, so its perturbation grows toward long distances; an [irrelevant operator](../../../critical-phenomenon.md#irrelevant-operator) has $y<0$ and decreases; a [marginal operator](../../../critical-phenomenon.md#marginal-operator) has $y=0$ and needs nonlinear flow to determine its behavior. **Marginality at linear order need not mean exact scale independence**. Interactions can be marginally relevant or [marginally irrelevant operators](../../../critical-phenomenon.md#marginally-irrelevant-operator).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Choose $\phi(x)=\int d^4p\,(2\pi)^{-4}e^{ip\cdot x}\widetilde\phi(p)$ in Euclidean signature. The inverse quadratic kernel is the [smooth-cutoff scalar propagator](../../../scalar-field-theory.md#smooth-cutoff-scalar-propagator)

$$
\boxed{\langle\widetilde\phi(p)\widetilde\phi(q)\rangle_0
=(2\pi)^4\delta^{(4)}(p+q)C_\Lambda(p),\qquad
C_\Lambda(p)=\frac1{f_\Lambda((p^2+m^2)/\Lambda^2)}.}
$$

The subscript records the explicit cutoff dependence implied by the condition $f_\Lambda(z)=\Lambda^2z$ at small $z$. For $p^2+m^2\le\Lambda^2$, this reduces to $1/(p^2+m^2)$, the usual Euclidean [scalar propagator](../../../scalar-field-theory.md#scalar-propagator). For $p^2+m^2\gg\Lambda^2$, the kernel $f_\Lambda$ grows rapidly and its inverse tends to zero.

**High-momentum modes are strongly suppressed**. For a finite smooth regulator they are not literally identically zero; that statement would require a sharp cutoff. The field variance carried by those [Fourier transform](../../../analysis.md#fourier-transform) modes is correspondingly negligible.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

It is useful to regulate the number of modes first, so the [functional integral](../../../quantum-field-theory.md#functional-measure) identities reduce to ordinary [integration by parts](../../../calculus.md#integration-by-parts). Let $C$ be the Gaussian covariance, $F=C^{-1}$, $W=e^{-S_1}$ and put a dot for $\Lambda\partial_\Lambda$. The matrix identity $\dot F=-F\dot C F$ gives

$$
\dot e^{-S_0}=\frac12(F\phi)^T\dot C(F\phi)e^{-S_0}.
$$

The second field derivative of the Gaussian is

$$
\partial_a\partial_b e^{-S_0}
=[(F\phi)_a(F\phi)_b-F_{ab}]e^{-S_0}.
$$

Hence, after two [integrations by parts](../../../calculus.md#integration-by-parts),

$$
\dot Z=\int d\phi\,e^{-S_0}\left[\dot W+\frac12\dot C_{ab}\partial_a\partial_bW\right]
+\frac12\operatorname{Tr}(F\dot C)Z.
$$

The imposed flow makes the bracket vanish. The remaining trace is independent of the fields and only changes the Gaussian normalization. Since the free Gaussian normalization is $\mathcal N=(\det(2\pi C))^{1/2}$, $\dot{\log\mathcal N}=\operatorname{Tr}(F\dot C)/2$. Therefore

$$
\boxed{\Lambda\partial_\Lambda(Z/\mathcal N)=0.}
$$

Equivalently, $Z$ is cutoff independent after discarding the stated overall rescaling. This is the [Gaussian covariance differentiation identity](../../../quantum-field-theory.md#gaussian-covariance-differentiation-identity) behind the [Polchinski equation](../../../perturbative-quantum-field-theory.md#polchinski-equation).

With the Fourier convention above and functional derivatives satisfying $\delta\widetilde\phi(p)/\delta\widetilde\phi(q)=\delta^{(4)}(p-q)$, contraction with $\dot C$ becomes $\int d^4p\,(2\pi)^4\dot C_\Lambda(p)\delta^2/[\delta\widetilde\phi(p)\delta\widetilde\phi(-p)]$. Thus **the numerator $(2\pi)^4$ in the printed flow is consistent with this derivative convention**; it must not be changed independently of the convention.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Using [functional derivatives](../../../calculus-of-variations.md#functional-derivative) of the interaction functional,

$$
\frac{\delta^2e^{-S_1}}{\delta\widetilde\phi(p)\delta\widetilde\phi(-p)}
=\left[\frac{\delta S_1}{\delta\widetilde\phi(p)}\frac{\delta S_1}{\delta\widetilde\phi(-p)}
-\frac{\delta^2S_1}{\delta\widetilde\phi(p)\delta\widetilde\phi(-p)}\right]e^{-S_1}.
$$

Dividing the flow by $e^{-S_1}$ therefore gives

$$
\boxed{\dot S_1=\frac12\int d^4p\,(2\pi)^4\dot C_\Lambda(p)
\left[\frac{\delta S_1}{\delta\widetilde\phi(p)}\frac{\delta S_1}{\delta\widetilde\phi(-p)}
-\frac{\delta^2S_1}{\delta\widetilde\phi(p)\delta\widetilde\phi(-p)}\right].}
$$

In the first term, remove one leg from each of two interaction vertices and join them with a line weighted by $\dot C_\Lambda(p)$. This produces the tree joining of two vertices. In the second, remove two legs from one vertex and contract them with that line, raising the [loop order](../../../perturbative-quantum-field-theory.md#loop-order) by one, with [tadpole diagrams](../../../perturbative-quantum-field-theory.md#tadpole-diagram) as the simplest example. The factor one half accounts for interchanging the contracted ends; the displayed signs are the signs in the interaction-action flow.

**The varying cutoff replaces an internal propagator by its cutoff derivative.** Repeated tree joins and loop closures express how eliminated high-momentum fluctuations generate the vertices of the [Wilsonian effective action](../../../perturbative-quantum-field-theory.md#wilsonian-effective-action). The action is not restricted to [one-particle-irreducible Feynman diagrams](../../../perturbative-quantum-field-theory.md#one-particle-irreducible-feynman-diagram): connected tree joins also occur. Field-independent vacuum contributions can again be absorbed into normalization.

## 3

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Fix the sign convention by taking the proper two-point insertion to be $i\Sigma(\not p)$. This convention matches the loop expression and mass conversion printed later. [Dyson resummation](../../../perturbative-quantum-field-theory.md#dyson-resummation) of successive [fermion self-energy](../../../perturbative-quantum-field-theory.md#fermion-self-energy) insertions gives

$$
iG=\frac{i}{\not p-m}+\frac{i}{\not p-m}(i\Sigma)\frac{i}{\not p-m}+\cdots
=\boxed{\frac{i}{\not p-m+\Sigma_R(\not p)}}.
$$

The subscript denotes the renormalized [self-energy](../../../perturbative-quantum-field-theory.md#self-energy). If the insertion is instead named $-i\Sigma_{\rm usual}$, then $\Sigma_{\rm usual}=-\Sigma_R$ and the denominator is written $\not p-m-\Sigma_{\rm usual}$. These are the same physical convention.

[Lorentz covariance](../../../special-relativity.md#lorentz-covariance) allows $\Sigma_R=\mathcal A(p^2)\not p+\mathcal B(p^2)m$. The physical mass-shell condition is

$$
\boxed{[1+\mathcal A(m_{\rm phys}^2)]m_{\rm phys}
-[1-\mathcal B(m_{\rm phys}^2)]m=0.}
$$

It locates the mass-shell singularity of the [Dirac propagator](../../../quantum-field-theory.md#dirac-propagator). In infrared-regulated perturbation theory this is the [pole mass](../../../perturbative-quantum-field-theory.md#pole-mass); near a simple pole the [quantum field theory propagator](../../../quantum-field-theory.md#propagator) has the form $iZ_{\rm pole}(\not p+m_{\rm phys})/(p^2-m_{\rm phys}^2+i0)$. The mass and pole residue are different quantities: the former fixes the singularity's location, the latter the field normalization. The calculation below uses this standard perturbative pole-mass definition.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

An [on-shell renormalization scheme](../../../perturbative-quantum-field-theory.md#on-shell-renormalization-scheme) fixes the mass parameter at the physical [pole mass](../../../perturbative-quantum-field-theory.md#pole-mass) and fixes the renormalized field by the chosen pole residue. Its [counterterms](../../../perturbative-quantum-field-theory.md#counterterm) include finite contributions needed to enforce those conditions. A coupling is likewise defined by a specified physical amplitude or mass-shell condition.

The [minimal subtraction scheme](../../../perturbative-quantum-field-theory.md#minimal-subtraction-scheme) removes only poles in the dimensional regulator. The [modified minimal subtraction scheme](../../../perturbative-quantum-field-theory.md#modified-minimal-subtraction-scheme), which is the overbarred scheme in the PDF, removes the accompanying universal combination $\log4\pi-\gamma_E$ as well. In $D=4-\epsilon$, the one-loop subtraction is proportional to

$$
\boxed{\Delta_{\overline{\rm MS}}=\frac2\epsilon-\gamma_E+\log4\pi.}
$$

**A subtraction-scheme mass is a running parameter and generally differs from the physical mass**. Finite redefinitions relate the schemes while leaving physical quantities unchanged. The overbar is essential for the stated finite formula in part (d).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The divergent part follows from the elementary integrals $\int_0^1x\,dx=1/2$ and $\int_0^1dx=1$:

$$
\Sigma_{\rm div}(\not p)=\boxed{\frac{e^2}{8\pi^2\epsilon}(\not p-4m).}
$$

Thus **a wave-function counterterm and a mass counterterm are required**. Write their contribution as

$$
\mathcal L_{\rm ct}=\delta Z_2\bar\psi i\not\partial\psi-\delta m_{\rm coeff}\bar\psi\psi.
$$

In the insertion convention of part (a), the inverse [Dirac propagator](../../../quantum-field-theory.md#dirac-propagator) receives $\delta Z_2\not p-\delta m_{\rm coeff}$. With $\kappa=e^2/(8\pi^2\epsilon)$, cancellation requires

$$
\boxed{\delta Z_2=-\kappa,\qquad\delta m_{\rm coeff}=-4\kappa m.}
$$

To distinguish the coefficient counterterm from the multiplicative mass renormalization, write $m_0=Z_m m$ and $\psi_0=Z_2^{1/2}\psi$. Then $\delta m_{\rm coeff}=m(\delta Z_2+\delta Z_m)$ at this order, giving $\delta Z_m=-3\kappa$. In [modified minimal subtraction](../../../perturbative-quantum-field-theory.md#modified-minimal-subtraction-scheme), replace $\kappa$ by $e^2\Delta_{\overline{\rm MS}}/(16\pi^2)$. No new derivative structure is needed for this two-point divergence; charge and photon [counterterms](../../../perturbative-quantum-field-theory.md#counterterm) are determined from other functions.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

After [modified minimal subtraction](../../../perturbative-quantum-field-theory.md#modified-minimal-subtraction-scheme), the surviving logarithm in the given [fermion self-energy](../../../perturbative-quantum-field-theory.md#fermion-self-energy) is $\log[\mu^2/((1-x)(m^2-p^2x))]$. For a one-loop mass shift, set $p^2=m^2$ and let $\not p$ act as $m$ on an on-shell spinor inside that correction; changing these arguments by the mass shift contributes only at order $e^4$. Thus

$$
\Sigma_R\big|_{\not p=m}
=\frac{e^2m}{8\pi^2}\int_0^1(x-2)\left[\log\frac{\mu^2}{m^2}-2\log(1-x)\right]dx.
$$

The needed integrals are

$$
\int_0^1(x-2)dx=-\frac32,\qquad
\int_0^1(x-2)\log(1-x)dx=\frac54.
$$

For the second, put $u=1-x$ and use $\int_0^1\log u\,du=-1$ and $\int_0^1u\log u\,du=-1/4$. Consequently

$$
\Sigma_R\big|_{\not p=m}=-\frac{e^2m}{16\pi^2}\left(5+3\log\frac{\mu^2}{m^2}\right).
$$

The [pole mass](../../../perturbative-quantum-field-theory.md#pole-mass) condition $m_{\rm phys}-m+\Sigma_R=0$ gives $m_{\rm phys}=m[1+e^2(5+3\log(\mu^2/m^2))/(16\pi^2)]+O(e^4)$. Invert this relation and replace $m$ by $m_{\rm phys}$ inside the already one-loop term to obtain

$$
\boxed{m=m_{\rm phys}\left[1-\frac{e^2}{16\pi^2}\left(5+3\log\frac{\mu^2}{m_{\rm phys}^2}\right)\right]+O(e^4).}
$$

**The negative sign in the running-mass conversion follows from the explicitly chosen self-energy convention.** Subtracting poles alone, instead of the overbarred combination, would leave additional $\log4\pi-\gamma_E$ terms.

## 4

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use Hermitian generators $T^a$ of the [special unitary group](../../../topological-group.md#special-unitary-group), with $[T^a,T^b]=if^{ab}{}_cT^c$. An adjoint field is the Lie-algebra-valued matrix $\psi=\psi^aT^a$, transforming as $\psi\mapsto U\psi U^{-1}$. The [adjoint covariant derivative](../../../relativistic-quantum-field.md#adjoint-covariant-derivative) is

$$
\boxed{D_\mu\psi=\partial_\mu\psi-ig[A_\mu,\psi].}
$$

In components, $(D_\mu\psi)^a=\partial_\mu\psi^a+gf^{abc}A_\mu^b\psi^c$. With $A_\mu\mapsto UA_\mu U^{-1}-(i/g)(\partial_\mu U)U^{-1}$, direct substitution gives $D_\mu\psi\mapsto U(D_\mu\psi)U^{-1}$. This is covariance in the [Adjoint representation of a Lie group](../../../lie-theory.md#adjoint-representation-of-a-lie-group). In the following [BRST symmetry](../../../relativistic-quantum-field.md#brst-symmetry) formulas, absorb the coupling into the connection, so $D_\mu=\partial_\mu-i[A_\mu,\cdot]$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Factor the odd parameter on the left, $\delta=\epsilon s$. The resulting [left-acting BRST differential](../../../relativistic-quantum-field.md#left-acting-brst-differential) obeys the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule)

$$
s(XY)=(sX)Y+(-1)^{|X|}X(sY).
$$

For the odd [Grassmann field](../../../quantum-field-theory.md#grassmann-field) $c$, the bracket in the transformation is a [graded commutator](../../../commutative-algebra.md#graded-commutator): $[c,c]_{\rm gr}=2c^2$, not the identically zero ordinary commutator of a matrix with itself. Thus $sc=ic^2$, while $sA_\mu=D_\mu c$, $s\bar c=h$ and $sh=0$.

On the ghost,

$$
s^2c=i[(sc)c-c(sc)]=i[ic^2c-ic c^2]=0.
$$

On the gauge field, variation of the connection and the [adjoint covariant derivative](../../../relativistic-quantum-field.md#adjoint-covariant-derivative) gives

$$
s^2A_\mu=D_\mu(sc)-i[sA_\mu,c]_{\rm gr}
=iD_\mu(c^2)-i[(D_\mu c)c+c(D_\mu c)]=0.
$$

Here $D_\mu$ is even and therefore obeys the ordinary product rule. Also $s^2\bar c=sh=0$ and $s^2h=0$, without using any field equation; this is off-shell nilpotence supplied by the [Nakanishi-Lautrup field](../../../relativistic-quantum-field.md#nakanishi-lautrup-field).

Applying the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule) twice cancels the two cross terms:

$$
s^2(XY)=(s^2X)Y+Xs^2Y.
$$

The square is consequently an even [graded derivation](../../../commutative-algebra.md#graded-derivation). Since it vanishes on every generator, it vanishes inductively on every polynomial in the fields. Hence **$s^2\mathcal O=0$ for every such operator**. This genuine result is stronger than the automatic vanishing obtained by merely setting $\epsilon^2=0$; two independent transformation parameters also give a vanishing commutator.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Use the [Minkowski metric](../../../special-relativity.md#minkowski-metric), path-integral weight $e^{iS}$ and the [Abelian gauge theory](../../../relativistic-quantum-field.md#abelian-gauge-theory) transformation $A_\mu\mapsto A_\mu+\partial_\mu\omega$. The gauge functional $F[A]=\partial\cdot A+A^2$ varies as

$$
\delta_\omega F=(\Box+2A^\mu\partial_\mu)\omega.
$$

Thus the [Faddeev-Popov operator](../../../relativistic-quantum-field.md#faddeev-popov-operator) is $\mathcal M_A=\Box+2A\cdot\partial$. It depends on the gauge field despite the gauge group being Abelian: **the ghosts interact because this gauge condition is nonlinear**.

Choose the [gauge-fixing fermion](../../../relativistic-quantum-field.md#gauge-fixing-fermion) $\Psi=\int d^4x\,\bar c(F[A]+\xi h/2)$. The [gauge-fixed action](../../../relativistic-quantum-field.md#gauge-fixed-action) $S=S_{\rm Maxwell}+s\Psi$ is

$$
\boxed{S=\int d^4x\left[-\frac14F_{\mu\nu}F^{\mu\nu}
+h(\partial\cdot A+A^2)+\frac\xi2h^2
-\bar c(\Box+2A\cdot\partial)c\right].}
$$

Here the tensor $F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu$ is distinct from the scalar gauge functional $F[A]$. With $\xi=0$, integrating over $h$ imposes the exact printed constraint. For nonzero $\xi$, eliminating $h=-F[A]/\xi$ instead gives

$$
\mathcal L=-\frac14F_{\mu\nu}F^{\mu\nu}-\frac1{2\xi}(\partial\cdot A+A^2)^2
-\bar c\Box c-2\bar c A^\mu\partial_\mu c.
$$

This version displays the additional gauge-dependent cubic and quartic gauge-field vertices as well as the ghost interaction; the strict condition is its $\xi\to0$ limit.

For the [Fourier transform](../../../analysis.md#fourier-transform) convention $c(x)=\int d^4p\,(2\pi)^{-4}e^{-ipx}c(p)$, the quadratic ghost kernel is $p^2$. With the ordering $\langle c(p)\bar c(q)\rangle$,

$$
\boxed{\langle c(p)\bar c(q)\rangle=(2\pi)^4\delta^{(4)}(p+q)\frac{i}{p^2+i0}.}
$$

The term $-2\bar c A^\mu\partial_\mu c$ has Fourier coefficient $2ip_\mu$, where $p$ is the incoming ghost momentum. Multiplication by $i$ in the [Feynman rule](../../../perturbative-quantum-field-theory.md#feynman-rule) gives

$$
\boxed{V_\mu(\bar c(q),c(p),A(k))=-2p_\mu,\qquad p+q+k=0.}
$$

These signs refer to the displayed action, Fourier convention and ghost ordering. Reversing the ghost/antighost convention changes corresponding signs consistently. A closed [ghost loop](../../../relativistic-quantum-field.md#ghost-loop) has the additional minus sign from [Grassmann variables](../../../linear-algebra.md#grassmann-variable).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

A gauge-invariant observable is [BRST-closed](../../../relativistic-quantum-field.md#brst-closed-operator): replacing its infinitesimal gauge parameter by the ghost gives $s\mathcal O=0$. Change the gauge functional continuously, or interpolate between two admissible choices, by changing the [gauge-fixing fermion](../../../relativistic-quantum-field.md#gauge-fixing-fermion) to $\Psi_t$. The action changes by the [BRST-exact operator](../../../relativistic-quantum-field.md#brst-exact-operator) $\partial_tS=s(\partial_t\Psi_t)$.

For a normalized correlator of $\mathcal O=\prod_i\mathcal O_i$ with each insertion [BRST-closed](../../../relativistic-quantum-field.md#brst-closed-operator), differentiation of the [functional integral](../../../quantum-field-theory.md#functional-measure) gives

$$
\partial_t\langle\mathcal O\rangle
=i\left[\langle\mathcal O\,s(\partial_t\Psi_t)\rangle
-\langle\mathcal O\rangle\langle s(\partial_t\Psi_t)\rangle\right].
$$

The [BRST Ward identity](../../../relativistic-quantum-field.md#brst-ward-identity) says $\langle sX\rangle=0$ for an invariant measure and action, with appropriate boundary conditions. Since $s\mathcal O=0$, the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule) makes the first insertion an exact variation of $\mathcal O\,\partial_t\Psi_t$ up to its harmless parity sign, and both terms vanish. Thus

$$
\boxed{\partial_t\langle\mathcal O_1\cdots\mathcal O_n\rangle=0.}
$$

**Physical gauge-invariant correlation functions are independent of this gauge condition**, even though individual gauge-field and ghost [Feynman diagrams](../../../perturbative-quantum-field-theory.md#feynman-diagram) change. This argument assumes an admissible perturbative gauge fixing, a [BRST symmetry](../../../relativistic-quantum-field.md#brst-symmetry)-preserving regulator/measure and no uncanceled boundary contribution. A global failure of those assumptions is not settled by the formal local calculation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
