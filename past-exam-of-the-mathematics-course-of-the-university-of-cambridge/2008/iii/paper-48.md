# Paper 48

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper48.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper48.pdf)

For the whole paper use $\eta=\operatorname{diag}(1,-1,-1,-1)$, natural units and the usual [Dirac adjoint](../../../relativistic-quantum-field.md#dirac-adjoint) $\bar\psi=\psi^\dagger\gamma^0$. The [Lorentz algebra](../../../semisimple-lie-algebra.md#lorentz-algebra) generators below have the real-generator convention of the PDF, with no extra factor of $i$.

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
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
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $I=I_2$. The [Pauli matrix multiplication law](../../../algebra.md#pauli-matrix-multiplication-law) gives $\sigma^i\sigma^j+\sigma^j\sigma^i=2\delta^{ij}I$. Block multiplication of the [Weyl representation of the gamma matrices](../../../relativistic-quantum-field.md#weyl-representation-of-the-gamma-matrices) gives

$$
(\gamma^0)^2=I_4,\qquad
\gamma^0\gamma^i=\begin{pmatrix}-\sigma^i&0\\0&\sigma^i\end{pmatrix},\qquad
\gamma^i\gamma^0=\begin{pmatrix}\sigma^i&0\\0&-\sigma^i\end{pmatrix},
$$

and

$$
\gamma^i\gamma^j=-\begin{pmatrix}\sigma^i\sigma^j&0\\0&\sigma^i\sigma^j\end{pmatrix}.
$$

Thus the mixed time-space anticommutators vanish, the time-time anticommutator is $2I_4$, and the spatial anticommutators are $-2\delta^{ij}I_4$. Together these prove the [Clifford algebra](../../../algebra.md#clifford-algebra) identity

$$
\boxed{\{\gamma^\mu,\gamma^\nu\}=2\eta^{\mu\nu}I_4.}
$$

The negative spatial sign comes from the lower-left block of each spatial [gamma matrix](../../../algebra.md#gamma-matrices).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Construct the [Lorentz-spinor generators from a Clifford algebra](../../../relativistic-quantum-field.md#lorentz-spinor-generators-from-a-clifford-algebra) as

$$
M^{\rho\sigma}=\frac14[\gamma^\rho,\gamma^\sigma]
=\frac12\gamma^\rho\gamma^\sigma-\frac12\eta^{\rho\sigma}I_4.
$$

They are antisymmetric in $\rho,\sigma$. Reordering a third [gamma matrix](../../../algebra.md#gamma-matrices) with the [Clifford algebra](../../../algebra.md#clifford-algebra) yields

$$
[\gamma^\rho\gamma^\sigma,\gamma^\tau]
=2\eta^{\sigma\tau}\gamma^\rho-2\eta^{\rho\tau}\gamma^\sigma,
\qquad
[M^{\rho\sigma},\gamma^\tau]
=\eta^{\sigma\tau}\gamma^\rho-\eta^{\rho\tau}\gamma^\sigma.
$$

Use the [commutator derivation identity](../../../lie-algebra.md#commutator-derivation-identity) on the two factors in $M^{\tau\nu}=\frac14[\gamma^\tau,\gamma^\nu]$:

$$
\begin{aligned}
[M^{\rho\sigma},M^{\tau\nu}]
&=\frac14\left([[M^{\rho\sigma},\gamma^\tau],\gamma^\nu]
+[\gamma^\tau,[M^{\rho\sigma},\gamma^\nu]]\right)\\
&=\eta^{\sigma\tau}M^{\rho\nu}-\eta^{\rho\tau}M^{\sigma\nu}
+\eta^{\rho\nu}M^{\sigma\tau}-\eta^{\sigma\nu}M^{\rho\tau}.
\end{aligned}
$$

This derives every [Lorentz algebra](../../../semisimple-lie-algebra.md#lorentz-algebra) commutation relation, so **the matrices $M^{\rho\sigma}$ form its spinor representation**. Their finite exponentials describe the connected [Spinor representation of the Lorentz group](../../../relativistic-quantum-field.md#spinor-representation-of-the-lorentz-group), more precisely the lift to its double cover.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For $x'=\Lambda x$, choose the corresponding spin lift

$$
S(\Lambda)=\exp\!\left(\frac12\Omega_{\rho\sigma}M^{\rho\sigma}\right).
$$

The [spinor field](../../../riemannian-geometry.md#spinor-field) transforms as

$$
\boxed{\psi'(x')=S(\Lambda)\psi(x),\qquad
\psi'(x)=S(\Lambda)\psi(\Lambda^{-1}x).}
$$

The infinitesimal [Clifford algebra](../../../algebra.md#clifford-algebra) identity from part (b) exponentiates to $S^{-1}\gamma^\mu S=\Lambda^\mu{}_{\nu}\gamma^\nu$, establishing [Lorentz covariance of the Dirac operator](../../../relativistic-quantum-field.md#lorentz-covariance-of-the-dirac-operator). At fixed coordinates the infinitesimal variation also includes the orbital term $-\Omega^\mu{}_{\nu}x^\nu\partial_\mu\psi$.

A spatial rotation generator $M^{ij}$ is anti-Hermitian, but a [Lorentz boost](../../../special-relativity.md#lorentz-boost) generator is Hermitian. For example,

$$
M^{01}=\frac12\gamma^0\gamma^1
=\frac12\begin{pmatrix}-\sigma^1&0\\0&\sigma^1\end{pmatrix}.
$$

Its eigenvalues are $\pm\tfrac12$. A nonzero rapidity $\zeta$ gives boost eigenvalues $e^{\pm\zeta/2}$, which are not all on the unit circle. This proves that the finite-dimensional component [Spinor representation of the Lorentz group](../../../relativistic-quantum-field.md#spinor-representation-of-the-lorentz-group) cannot be unitary for a positive-definite component inner product, even after a change of basis. It does not contradict a unitary action on the physical space of quantum states.

Consequently $\psi'^\dagger(x')\psi'(x')=\psi^\dagger S^\dagger S\psi$ need not equal $\psi^\dagger\psi$: it is the time component of the [Dirac current](../../../quantum-field-theory.md#dirac-current), not a [Lorentz scalar](../../../special-relativity.md#lorentz-scalar). The appropriate invariant form is indefinite. From $(\gamma^\mu)^\dagger=\gamma^0\gamma^\mu\gamma^0$ one obtains

$$
(M^{\rho\sigma})^\dagger\gamma^0+\gamma^0M^{\rho\sigma}=0,
\qquad S^\dagger\gamma^0S=\gamma^0.
$$

This [Dirac spinor pseudo-unitarity](../../../relativistic-quantum-field.md#dirac-spinor-pseudo-unitarity) gives $\bar\psi'(x')=\bar\psi(x)S^{-1}$ and hence the [Dirac scalar bilinear](../../../relativistic-quantum-field.md#dirac-scalar-bilinear)

$$
\boxed{\bar\psi'(x')\psi'(x')=\bar\psi(x)\psi(x).}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Use the PDF's convention in which $C$ multiplies $\psi^*$, rather than $\bar\psi^T$. Its unitarity converts the given [gamma matrix](../../../algebra.md#gamma-matrices) identity into

$$
\gamma^\mu C=-C(\gamma^\mu)^*.
$$

Applying it twice gives

$$
M^{\rho\sigma}C
=\frac14[\gamma^\rho,\gamma^\sigma]C
=C\frac14[(\gamma^\rho)^*,(\gamma^\sigma)^*]
=C(M^{\rho\sigma})^*.
$$

For real infinitesimal [Lorentz transformation](../../../special-relativity.md#lorentz-transformation) parameters,

$$
C\left(I+\frac12\Omega_{\rho\sigma}M^{\rho\sigma}\right)^*
=\left(I+\frac12\Omega_{\rho\sigma}M^{\rho\sigma}\right)C.
$$

Therefore **$\psi^c=C\psi^*$ transforms in exactly the same spinor representation as $\psi$**. The coordinate pullback is real and transforms identically as well. This is the [antilinear charge-conjugation intertwiner](../../../quantum-field-theory.md#antilinear-charge-conjugation-intertwiner) relation; exponentiating also gives $CS^*=SC$ for connected transformations.

For real mass, complex conjugation of the free [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) gives $(-i\gamma^{\mu*}\partial_\mu-m)\psi^*=0$. Multiply by $C$ and move it through the [gamma matrices](../../../algebra.md#gamma-matrices):

$$
0=C(-i\gamma^{\mu*}\partial_\mu-m)\psi^*
=(i\gamma^\mu\partial_\mu-m)C\psi^*.
$$

Thus

$$
\boxed{(i\gamma^\mu\partial_\mu-m)\psi^c=0.}
$$

As an explicit check, in the given [Weyl representation of the gamma matrices](../../../relativistic-quantum-field.md#weyl-representation-of-the-gamma-matrices) one may take $C=i\gamma^2$. It is unitary and obeys the required conjugation identity. The free-equation conclusion does not assert that a charge-conjugated field retains the same charge in a fixed electromagnetic background.

## 2

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Split the free [scalar field](../../../quantum-field-theory.md#scalar-field) into its annihilation part $\phi^{(+)}$ and creation part $\phi^{(-)}$. [Normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering) moves every creation operator to the left of every annihilation operator, without adding the commutators produced by that rearrangement. For two fields,

$$
:\phi(x)\phi(y):=
\phi^{(-)}(x)\phi^{(-)}(y)+\phi^{(-)}(x)\phi^{(+)}(y)
+\phi^{(-)}(y)\phi^{(+)}(x)+\phi^{(+)}(x)\phi^{(+)}(y).
$$

Its vacuum expectation is zero. [Time ordering](../../../perturbative-quantum-field-theory.md#time-ordering) instead places the field at the later time on the left:

$$
T\{\phi(x)\phi(y)\}
=\theta(x^0-y^0)\phi(x)\phi(y)+\theta(y^0-x^0)\phi(y)\phi(x).
$$

The equal-time convention is immaterial away from coincident singularities; these expressions are understood as [operator-valued distributions](../../../quantum-field-theory.md#operator-valued-distribution).

The only nonzero vacuum contraction uses $a_{\mathbf p}a^\dagger_{\mathbf q}$. The oscillator [commutator](../../../lie-algebra.md#commutator) therefore gives the [Wightman function](../../../quantum-field-theory.md#wightman-function)

$$
W(x-y)=\langle0|\phi(x)\phi(y)|0\rangle
=\int\frac{d^3p}{(2\pi)^3}\frac{e^{-iE_{\mathbf p}(x^0-y^0)+i\mathbf p\cdot(\mathbf x-\mathbf y)}}{2E_{\mathbf p}}.
$$

Put $\tau=x^0-y^0$ and $\mathbf r=\mathbf x-\mathbf y$. Combining the two time orders, and reversing $\mathbf p$ in the second when necessary, gives

$$
\Delta_F(\tau,\mathbf r)
=\int\frac{d^3p}{(2\pi)^3}\frac{e^{i\mathbf p\cdot\mathbf r-iE_{\mathbf p}|\tau|}}{2E_{\mathbf p}}.
$$

To recover the four-dimensional [Fourier transform](../../../analysis.md#fourier-transform), use the [Feynman i-epsilon prescription](../../../quantum-field-theory.md#feynman-i-epsilon-prescription) in the energy variable:

$$
\int\frac{dp^0}{2\pi}\frac{i e^{-ip^0\tau}}{(p^0)^2-E_{\mathbf p}^2+i0}
=\frac{e^{-iE_{\mathbf p}|\tau|}}{2E_{\mathbf p}}.
$$

The positive-energy pole lies just below the real axis, and the negative-energy pole just above it. For $\tau>0$, close below clockwise: the residue at $E_{\mathbf p}-i0$ is $i e^{-iE_{\mathbf p}\tau}/(2E_{\mathbf p})$, and the clockwise factor $-i$ after dividing by $2\pi$ gives the required positive coefficient. For $\tau<0$, close above counterclockwise: the residue at $-E_{\mathbf p}+i0$ is $-i e^{iE_{\mathbf p}\tau}/(2E_{\mathbf p})$, and the factor $+i$ gives the other time order. Equivalently the energy contour passes above the positive-energy pole and below the negative-energy pole. Hence

$$
\boxed{\Delta_F(x-y)=\lim_{\epsilon\downarrow0}
\int\frac{d^4p}{(2\pi)^4}\frac{i e^{-ip\cdot(x-y)}}{p^2-\mu^2+i\epsilon}.}
$$

The limit is distributional. The [scalar Feynman propagator pole prescription](../../../quantum-field-theory.md#scalar-feynman-propagator-pole-prescription) is essential; omitting it from the denominator must be accompanied by the specified contour.

Finally, moving the annihilation part of $\phi(x)$ past the creation part of $\phi(y)$ gives

$$
\phi(x)\phi(y)=:\phi(x)\phi(y):+W(x-y)\mathbf1.
$$

The normal-ordered two-field product is symmetric in $x,y$, because the two creation parts commute and the two annihilation parts commute. Applying the two time orders thus proves the [two-field scalar Wick identity](../../../perturbative-quantum-field-theory.md#two-field-scalar-wick-identity)

$$
\boxed{T\{\phi(x)\phi(y)\}=:\phi(x)\phi(y):+\Delta_F(x-y)\mathbf1.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use the momentum-space [Feynman rules](../../../perturbative-quantum-field-theory.md#feynman-rule) with all momenta conserved at each vertex. The free [scalar propagator](../../../scalar-field-theory.md#scalar-propagator), free [Dirac propagator](../../../quantum-field-theory.md#dirac-propagator) and [pseudoscalar Yukawa interaction](../../../standard-model.md#pseudoscalar-yukawa-interaction) vertex are respectively

$$
\boxed{\frac{i}{k^2-\mu^2+i0},\qquad
\frac{i(\not p+m)}{p^2-m^2+i0},\qquad
-i\lambda\gamma^5.}
$$

The [Dirac propagator](../../../quantum-field-theory.md#dirac-propagator) follows by multiplying the inverse kinetic matrix $\not p-m$ by $\not p+m$, using the [Clifford algebra](../../../algebra.md#clifford-algebra) to obtain $(\not p-m)(\not p+m)=(p^2-m^2)I_4$. The vertex follows by expanding $e^{iS_{\mathrm{int}}}$ once: there is no factorial because it has one scalar and two distinct spinor field factors. An internal scalar has no spinor indices; an internal fermion line carries the displayed matrix with its momentum directed along [fermion flow](../../../perturbative-quantum-field-theory.md#fermion-flow).

These rules use the coefficient exactly as printed. With the standard Hermitian $\gamma^5=i\gamma^0\gamma^1\gamma^2\gamma^3$, the [Hermiticity of a pseudoscalar Dirac bilinear](../../../standard-model.md#hermiticity-of-a-pseudoscalar-dirac-bilinear) gives $(\bar\psi\gamma^5\psi)^\dagger=-\bar\psi\gamma^5\psi$. A Hermitian physical interaction therefore requires $\lambda^*=-\lambda$; writing $\lambda=ig$ with real $g$ changes the vertex to $g\gamma^5$. This convention issue does not alter the formal rules above, and no unstated real-coupling assumption is needed.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Label the incoming momenta and spin states $(p_1,r_1),(p_2,r_2)$ and the outgoing ones $(p_3,r_3),(p_4,r_4)$, with $p_1+p_2=p_3+p_4$. Write $u_i=u^{r_i}(\mathbf p_i)$ and $v_i=v^{r_i}(\mathbf p_i)$. The [Mandelstam variables](../../../special-relativity.md#mandelstam-variables) are $s=(p_1+p_2)^2$, $t=(p_1-p_3)^2$ and $u=(p_1-p_4)^2$. At lowest order, each connected [Feynman diagram](../../../perturbative-quantum-field-theory.md#feynman-diagram) has two [pseudoscalar Yukawa interaction](../../../standard-model.md#pseudoscalar-yukawa-interaction) vertices and one internal [scalar propagator](../../../scalar-field-theory.md#scalar-propagator).

<a id="2/c/image-the-t-and-u-exchanges-for-two-fermions-and-the-t-exchange-and-s-annihilation-for-a-fermion-antifermion-pair-with-external-momentum-and-spin-labels"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-48-yukawa-trees.png)

**[Figure 1](#2/c/image-the-t-and-u-exchanges-for-two-fermions-and-the-t-exchange-and-s-annihilation-for-a-fermion-antifermion-pair-with-external-momentum-and-spin-labels). The t and u exchanges for two fermions, and the t exchange and s annihilation for a fermion-antifermion pair, with external momentum and spin labels**.

Define the [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude) by $S_{fi}^{\mathrm{connected}}=i(2\pi)^4\delta^4(p_1+p_2-p_3-p_4)\mathcal M$. Fix the external [Fock state](../../../quantum-field-theory.md#fock-state) ordering as $b_1^\dagger b_2^\dagger|0\rangle$ to $b_3^\dagger b_4^\dagger|0\rangle$ for the two-fermion process. The $t$ exchange connects $1$ to $3$ and $2$ to $4$; the $u$ exchange connects $1$ to $4$ and $2$ to $3$. The two [Feynman vertices](../../../perturbative-quantum-field-theory.md#interaction-vertex) contribute $(-i\lambda)^2$, and the internal [scalar propagator](../../../scalar-field-theory.md#scalar-propagator) contributes $i$ divided by its denominator. Exchanging the two identical final fermions supplies a relative [fermionic sign](../../../perturbative-quantum-field-theory.md#fermionic-sign). Thus

$$
\boxed{\mathcal M_{\psi\psi}
=-\lambda^2\left[
\frac{(\bar u_3\gamma^5u_1)(\bar u_4\gamma^5u_2)}{t-\mu^2+i0}
-\frac{(\bar u_4\gamma^5u_1)(\bar u_3\gamma^5u_2)}{u-\mu^2+i0}
\right].}
$$

This changes sign when the two outgoing labels are exchanged, as identical-fermion antisymmetry requires. There is no $s$ annihilation diagram for two incoming fermions: the interaction preserves [Dirac fermion number conservation](../../../relativistic-quantum-field.md#dirac-fermion-number-conservation).

For the fermion-antifermion process take initial state $b_1^\dagger d_2^\dagger|0\rangle$ and final state $b_3^\dagger d_4^\dagger|0\rangle$. The $t$ exchange uses bilinears $(\bar u_3\gamma^5u_1)(\bar v_2\gamma^5v_4)$, and the $s$ annihilation uses $(\bar v_2\gamma^5u_1)(\bar u_3\gamma^5v_4)$. To fix the sign without a guess, expand the current $J=:\bar\psi\gamma^5\psi:$ in creation and annihilation operators. Its relevant terms have the signs

$$
J\supset b^\dagger b\,\bar u\gamma^5u
-d^\dagger d\,\bar v\gamma^5v
+d b\,\bar v\gamma^5u
+b^\dagger d^\dagger\,\bar u\gamma^5v.
$$

The [antifermion sign of a normal-ordered bilinear](../../../perturbative-quantum-field-theory.md#antifermion-sign-of-a-normal-ordered-bilinear) makes the exchange contraction negative, whereas the product of annihilation and creation contractions is positive for the specified external ordering. Multiplying by $(-i\lambda)^2i=-i\lambda^2$ therefore gives

$$
\boxed{\mathcal M_{\psi\bar\psi}
=\lambda^2\left[
\frac{(\bar u_3\gamma^5u_1)(\bar v_2\gamma^5v_4)}{t-\mu^2+i0}
-\frac{(\bar v_2\gamma^5u_1)(\bar u_3\gamma^5v_4)}{s-\mu^2+i0}
\right].}
$$

A different common phase convention for an external state can reverse the overall amplitude, but never the relative sign of its two contributions. Both results are [tree scattering with pseudoscalar exchange](../../../standard-model.md#tree-scattering-with-pseudoscalar-exchange) and are of order $\lambda^2$.

## 3

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Maxwell field](../../../electromagnetism.md#electromagnetic-field) has the [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance) $A_\mu\mapsto A_\mu+\partial_\mu\alpha(x)$ for an arbitrary smooth scalar function $\alpha$. Commuting the two derivatives shows that $F_{\mu\nu}$ is unchanged, so the [Maxwell Lagrangian](../../../electromagnetism.md#maxwell-lagrangian) is invariant. Vary the action, use antisymmetry of $F$ and integrate by parts with variations vanishing on the boundary:

$$
\delta S=-\frac12\int d^4x\,F^{\mu\nu}\delta F_{\mu\nu}
=-\int d^4x\,F^{\mu\nu}\partial_\mu\delta A_\nu
=\int d^4x\,(\partial_\mu F^{\mu\nu})\delta A_\nu.
$$

The [Euler-Lagrange field equations](../../../quantum-field-theory.md#euler-lagrange-field-equation) are therefore $\partial_\mu F^{\mu\nu}=0$. Expanding $F$ gives

$$
\Box A^\nu-\partial^\nu(\partial_\mu A^\mu)=0,
\qquad \Box=\partial_\mu\partial^\mu.
$$

In [Lorenz gauge](../../../electromagnetism.md#lorenz-gauge-condition) the second term vanishes, leaving

$$
\boxed{\Box A_\nu=0.}
$$

The PDF calls this “Lorentz gauge”; the standard name is [Lorenz gauge](../../../electromagnetism.md#lorenz-gauge-condition). A residual [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance) preserves this condition when $\Box\alpha=0$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Put $D=\partial_\rho A^\rho$. The gauge-fixing variation is

$$
\delta\!\left(-\frac12D^2\right)=-D\partial^\nu\delta A_\nu.
$$

After integration by parts its contribution to the [Euler-Lagrange field equations](../../../quantum-field-theory.md#euler-lagrange-field-equation) is $+\partial^\nu D$. It cancels the $-\partial^\nu D$ from the [Maxwell Lagrangian](../../../electromagnetism.md#maxwell-lagrangian), giving **$\Box A^\nu=0$ for all four components**. This is the [Feynman gauge](../../../relativistic-quantum-field.md#feynman-gauge) equation; the physical [Lorenz gauge](../../../electromagnetism.md#lorenz-gauge-condition) condition must still be imposed on states rather than inferred as an additional classical equation from this gauge-fixed density.

Treating the covariant components $A_\mu$ as coordinates, the derivative of the actual displayed density with respect to $\partial_0A_\mu$ gives the [canonical momenta](../../../classical-mechanics.md#canonical-momentum)

$$
\boxed{\pi^\mu=-F^{0\mu}-\eta^{0\mu}D.}
$$

In terms of lower-index spatial coordinates,

$$
\pi^0=-\dot A_0+\partial_iA_i,\qquad
\pi^i=\dot A_i-\partial_iA_0\quad(i=1,2,3).
$$

The [gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing) has supplied the nonzero momentum of $A_0$, absent from the ungauge-fixed [Maxwell Lagrangian](../../../electromagnetism.md#maxwell-lagrangian).

There is a boundary-term convention needed for the next part's printed momentum expansion. Direct expansion gives the [Feynman-gauge Maxwell kinetic density after a boundary-term subtraction](../../../relativistic-quantum-field.md#feynman-gauge-maxwell-kinetic-density-after-a-boundary-term-subtraction):

$$
\mathcal L=\mathcal L'+\partial_\rho K^\rho,
\qquad\mathcal L'=-\frac12\partial_\rho A_\sigma\partial^\rho A^\sigma,
\qquad K^\rho=\frac12(A_\sigma\partial^\sigma A^\rho-A^\rho D).
$$

To verify it, the difference of the densities is $\tfrac12[(\partial_\rho A_\sigma)(\partial^\sigma A^\rho)-D^2]$; differentiating $K^\rho$ gives these two terms, while the remaining second-derivative terms cancel after renaming indices. The subtracted density has $\widetilde\pi^\mu=-\dot A^\mu$, which is exactly the momentum used by the mode expansion in part (c). The literal momenta asked for here are the boxed expression, not $-\dot A^\mu$. Both densities have the same field equations, and their [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation) agree through the [boundary-induced canonical transformation in Feynman gauge](../../../relativistic-quantum-field.md#boundary-induced-canonical-transformation-in-feynman-gauge).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Denote the momentum in the printed mode expansion by $\widetilde\pi^\nu$, as it equals $-\dot A^\nu$ for the boundary-subtracted density discussed in part (b). Take a real complete basis of [polarization vectors](../../../relativistic-quantum-field.md#polarization-vector). Its completeness relation with one index raised is

$$
\sum_{\lambda,\lambda'}\epsilon_\mu^\lambda(\mathbf p)
\epsilon^{\nu\lambda'}(\mathbf p)\eta^{\lambda\lambda'}=\delta_\mu{}^\nu.
$$

Here raising or lowering the polarization labels uses the same diagonal matrix $\eta$, so this is just the completeness relation in the PDF. Write $\mathbf r=\mathbf x-\mathbf y$. In the mixed field-momentum [commutator](../../../lie-algebra.md#commutator), the $aa^\dagger$ term gives the product of the minus sign in $\widetilde\pi$'s creation part and the minus sign in the oscillator [commutator](../../../lie-algebra.md#commutator). The $a^\dagger a$ term gives the same sign. The two mode normalization factors multiply to $1/2$, and the momentum delta function removes one integral. Consequently

$$
\begin{aligned}
[A_\mu(\mathbf x),\widetilde\pi^\nu(\mathbf y)]
&=\frac i2\int\frac{d^3p}{(2\pi)^3}
\sum_{\lambda,\lambda'}\epsilon_\mu^\lambda\epsilon^{\nu\lambda'}\eta^{\lambda\lambda'}
\left(e^{i\mathbf p\cdot\mathbf r}+e^{-i\mathbf p\cdot\mathbf r}\right)\\
&=i\delta_\mu{}^\nu\delta^{(3)}(\mathbf x-\mathbf y).
\end{aligned}
$$

For the field-field [commutator](../../../lie-algebra.md#commutator), the polarization sum gives instead

$$
[A_\mu(\mathbf x),A_\nu(\mathbf y)]
=-\eta_{\mu\nu}\int\frac{d^3p}{(2\pi)^3}\frac{e^{i\mathbf p\cdot\mathbf r}-e^{-i\mathbf p\cdot\mathbf r}}{2|\mathbf p|}=0,
$$

because the integrand is odd under $\mathbf p\mapsto-\mathbf p$. Similarly,

$$
[\widetilde\pi^\mu(\mathbf x),\widetilde\pi^\nu(\mathbf y)]
=-\eta^{\mu\nu}\int\frac{d^3p}{(2\pi)^3}\frac{|\mathbf p|}{2}
\left(e^{i\mathbf p\cdot\mathbf r}-e^{-i\mathbf p\cdot\mathbf r}\right)=0.
$$

These are the requested [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation), derived by [photon oscillator completeness and canonical brackets](../../../relativistic-quantum-field.md#photon-oscillator-completeness-and-canonical-brackets).

They also hold for the literal momenta of part (b). The shifts are

$$
\pi^0=\widetilde\pi^0+\partial_iA_i,\qquad
\pi^i=\widetilde\pi^i-\partial_iA_0.
$$

Since the fields commute at equal times, their mixed brackets with the momenta do not change. The only potentially new momentum bracket is

$$
[\pi^0(\mathbf x),\pi^i(\mathbf y)]
=i\bigl(\partial_{y^i}+\partial_{x^i}\bigr)\delta^{(3)}(\mathbf x-\mathbf y)=0.
$$

All other momentum brackets vanish separately. Thus **both canonical conventions have $[A_\mu,\pi^\nu]=i\delta_\mu{}^\nu\delta^3$ and vanishing coordinate-coordinate and momentum-momentum brackets**, even though the momentum operators differ by spatial derivatives. This resolves the density/expansion mismatch without changing the printed oscillator algebra.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The oscillator [commutator](../../../lie-algebra.md#commutator) gives

$$
\langle0|a_{\mathbf p}^{\lambda}a_{\mathbf q}^{\lambda'\dagger}|0\rangle
=-\eta^{\lambda\lambda'}(2\pi)^3\delta^{(3)}(\mathbf p-\mathbf q).
$$

The temporal mode $\lambda=0$ has negative norm. More precisely, the nonzero [wave packet](../../../wave-equation.md#wave-packet) $|f,0\rangle=\int d^3p\,f(\mathbf p)a_{\mathbf p}^{0\dagger}|0\rangle/(2\pi)^3$ has norm $-\int d^3p\,|f(\mathbf p)|^2/(2\pi)^3<0$. The difficulty is an [indefinite Hermitian form](../../../linear-algebra.md#indefinite-hermitian-form), not the divergent normalization of an unsmeared [momentum eigenstate](../../../quantum-mechanics.md#momentum-eigenstate). The [covariant photon Fock space](../../../relativistic-quantum-field.md#covariant-photon-fock-space) is therefore not a positive physical [Hilbert space](../../../hilbert-space.md).

[Gupta-Bleuler quantization](../../../relativistic-quantum-field.md#gupta-bleuler-formalism) imposes only the annihilation, or [positive-frequency part of a quantum field](../../../quantum-field-theory.md#positive-frequency-part-of-a-quantum-field), of the divergence:

$$
\boxed{(\partial_\mu A^\mu)^{(+)}|\mathrm{phys}\rangle=0.}
$$

A strong operator identity $\partial\cdot A=0$ is incompatible with the four unconstrained [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation); in the literal momentum convention it would set $\pi^0=0$. The weaker condition instead implies $\langle\Phi|\partial\cdot A|\Psi\rangle=0$ between physical states: the positive-frequency part annihilates the ket, and its adjoint annihilates the bra.

For a nonzero [momentum](../../../classical-mechanics.md#momentum) choose upper-index [polarization vectors](../../../relativistic-quantum-field.md#polarization-vector)

$$
\epsilon^{\mu0}=(1,\mathbf0),\quad
\epsilon^{\mu1}=(0,\mathbf e_1),\quad
\epsilon^{\mu2}=(0,\mathbf e_2),\quad
\epsilon^{\mu3}=(0,\widehat{\mathbf p}),
$$

where $\mathbf e_1,\mathbf e_2$ are an orthonormal pair perpendicular to $\mathbf p$. Labels 1 and 2 have [transverse polarization](../../../wave-equation.md#transverse-polarization), label 3 has spatial [longitudinal polarization](../../../wave-equation.md#longitudinal-polarization), and label 0 has [timelike photon polarization](../../../relativistic-quantum-field.md#timelike-photon-polarization). With $p^0=|\mathbf p|=\omega$, the divergence of the annihilation part is proportional to $-i\omega(a^0_{\mathbf p}-a^3_{\mathbf p})$. The physical condition is therefore

$$
(a^0_{\mathbf p}-a^3_{\mathbf p})|\mathrm{phys}\rangle=0.
$$

For a one-mode state $|\chi\rangle=\sum_\lambda c_\lambda a^{\lambda\dagger}|0\rangle$, the condition reads $-c_0-c_3=0$. Thus

$$
|\chi\rangle=c_1a^{1\dagger}|0\rangle+c_2a^{2\dagger}|0\rangle
+c_0(a^{0\dagger}-a^{3\dagger})|0\rangle,
\qquad
\langle\chi|\chi\rangle=|c_1|^2+|c_2|^2.
$$

The last direction has zero norm and is orthogonal to every constrained state. Its field wavefunction is proportional to $\epsilon^{\mu0}+\epsilon^{\mu3}=p^\mu/\omega$, hence it is a pure [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance) direction. A purely longitudinal creator $a^{3\dagger}$ alone is not physical, despite having positive norm.

For the multiparticle sketch, put $C=a^0-a^3$ and $C^\dagger=a^{0\dagger}-a^{3\dagger}$. The [commutator](../../../lie-algebra.md#commutator) $[C,C^\dagger]=0$ allows polynomials in $C^\dagger$ times transverse creator states to obey the constraint. Conversely, on creator polynomials the constraint is $-\partial_{a^{0\dagger}}-\partial_{a^{3\dagger}}$, so these are all the constrained polynomials. Every term containing $C^\dagger$ is orthogonal to every constrained bra, since $\langle\Phi|C^\dagger=\langle C\Phi|=0$. Quotienting those null vectors and completing the remaining positive space is the [Gupta-Bleuler null-state quotient](../../../relativistic-quantum-field.md#gupta-bleuler-null-state-quotient). It gives

$$
\boxed{\text{two physical transverse photon polarizations, or helicities }+1,-1.}
$$

The one-particle instance is the [transverse one-photon physical quotient](../../../relativistic-quantum-field.md#transverse-one-photon-physical-quotient).

## 4

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A symmetry of a [classical field theory](../../../quantum-field-theory.md#classical-field-theory) maps solutions to solutions; for the [Noether theorem](../../../calculus-of-variations.md#noether-theorem) we require a continuous variational symmetry of the action, allowing its density to change by a total divergence. This is stronger than simply observing an accidental symmetry of one solution. Consider first-derivative fields $\phi_a$ and define

$$
\Pi_a^\mu=\frac{\partial\mathcal L}{\partial(\partial_\mu\phi_a)},\qquad
E_a=\frac{\partial\mathcal L}{\partial\phi_a}-\partial_\mu\Pi_a^\mu.
$$

The [Euler-Lagrange field equations](../../../quantum-field-theory.md#euler-lagrange-field-equation) are $E_a=0$. For a fixed-coordinate variation $\delta_0\phi_a=\varepsilon Q_a$, the product rule gives the off-shell identity

$$
\frac{\delta_0\mathcal L}{\varepsilon}
=\sum_a E_aQ_a+\partial_\mu\!\left(\sum_a\Pi_a^\mu Q_a\right).
$$

This identity is the proof's essential integration-by-parts step.

For a general spacetime symmetry write $x'^\mu=x^\mu+\varepsilon\xi^\mu$ and $\phi'_a(x')=\phi_a(x)+\varepsilon\Delta_a$. At a fixed point $Q_a=\Delta_a-\xi^\nu\partial_\nu\phi_a$, while the volume-element variation contributes $\partial_\mu(\mathcal L\xi^\mu)$. Suppose action invariance takes the form

$$
\frac{\delta_0\mathcal L}{\varepsilon}+\partial_\mu(\mathcal L\xi^\mu)=\partial_\mu K^\mu.
$$

Combining with the preceding identity proves

$$
\boxed{j^\mu=\sum_a\Pi_a^\mu Q_a+\mathcal L\xi^\mu-K^\mu,
\qquad\partial_\mu j^\mu=-\sum_aE_aQ_a=0\ \text{on shell}.}
$$

This is the [Noether current for a spacetime symmetry](../../../quantum-field-theory.md#noether-current-for-a-spacetime-symmetry). It also covers internal symmetries, for which $\xi=0$. A constant parameter corresponds to one [Noether current](../../../quantum-field-theory.md#noether-current); several independent parameters give several currents. Integrating the continuity equation gives

$$
\frac{dQ}{dt}=-\int_{\partial\Sigma}\mathbf j\cdot d\mathbf S,
\qquad Q=\int_\Sigma j^0\,d^3x.
$$

Thus the [Noether charge](../../../quantum-field-theory.md#noether-charge) is conserved when the fields have suitable falloff or no flux through the spatial boundary. These are classical identities; quantum symmetries may additionally require absence of an [quantum anomaly](../../../relativistic-quantum-field.md#anomaly-physics).

**Translations conserve energy and momentum.** If the density has no explicit coordinate dependence, take the active fixed-coordinate variation $Q_a=\partial_\nu\phi_a$ for translation in direction $\nu$. Then $\delta_0\mathcal L/\varepsilon=\partial_\nu\mathcal L$, and the internal-form proof with $K^\mu=\delta^\mu{}_{\nu}\mathcal L$ gives the [canonical energy-momentum tensor](../../../quantum-field-theory.md#canonical-stress-energy-tensor)

$$
T^\mu{}_{\nu}=\sum_a\Pi_a^\mu\partial_\nu\phi_a-\delta^\mu{}_{\nu}\mathcal L,
\qquad \partial_\mu T^\mu{}_{\nu}=0.
$$

Its four spatial integrals are the conserved energy and momentum. For a real [scalar field](../../../quantum-field-theory.md#scalar-field) with density $\tfrac12(\partial\phi)^2-V(\phi)$ this becomes $T^{\mu\nu}=\partial^\mu\phi\partial^\nu\phi-\eta^{\mu\nu}\mathcal L$. Direct differentiation gives $\partial_\mu T^{\mu\nu}=(\Box\phi+V'(\phi))\partial^\nu\phi$, which vanishes by the field equation.

**Lorentz symmetry conserves angular momentum and boost charges.** For that scalar example, $T^{\mu\nu}$ is symmetric, so the [Lorentz transformation](../../../special-relativity.md#lorentz-transformation) currents can be written

$$
J^{\mu\rho\sigma}=x^\rho T^{\mu\sigma}-x^\sigma T^{\mu\rho}.
$$

Their divergence is $T^{\rho\sigma}-T^{\sigma\rho}=0$. Spatial pairs give [angular momentum](../../../classical-mechanics.md#angular-momentum), and time-space pairs give the conserved boost charges. For a [spinor field](../../../riemannian-geometry.md#spinor-field) or a [vector field](../../../calculus.md#vector-field), the intrinsic field variation supplies an additional spin current; equivalently the [Belinfante-Rosenfeld stress-energy tensor](../../../quantum-field-theory.md#belinfante-rosenfeld-stress-energy-tensor) combines spin and orbital pieces into a symmetric stress tensor. The nonunitarity of the finite component [Spinor representation of the Lorentz group](../../../relativistic-quantum-field.md#spinor-representation-of-the-lorentz-group) does not obstruct conservation of these physical spacetime charges.

**Global phase symmetry conserves particle charge.** For a complex [scalar field](../../../quantum-field-theory.md#scalar-field) with density $\partial_\mu\Phi^*\partial^\mu\Phi-V(\Phi^*\Phi)$, the constant transformation $\Phi\mapsto e^{-i\alpha}\Phi$ leaves the density invariant. Using $Q_\Phi=-i\Phi$ and $Q_{\Phi^*}=i\Phi^*$ gives the [Noether current](../../../quantum-field-theory.md#noether-current)

$$
j^\mu=i(\Phi^*\partial^\mu\Phi-\Phi\partial^\mu\Phi^*).
$$

For a [Dirac field](../../../relativistic-quantum-field.md#dirac-field), the corresponding variations $Q_\psi=-i\psi$, $Q_{\bar\psi}=i\bar\psi$ yield instead $j^\mu=\bar\psi\gamma^\mu\psi$, the [Dirac current](../../../quantum-field-theory.md#dirac-current). Its divergence vanishes by the [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) and [adjoint Dirac equation](../../../relativistic-quantum-field.md#adjoint-dirac-equation). The [Yukawa interaction](../../../standard-model.md#yukawa-interaction) of part 2 also preserves this phase symmetry, because each bilinear has one $\psi$ and one $\bar\psi$. Thus it preserves fermion number and forbids annihilation of two fermions into a single scalar. These currents express charge or particle-minus-antiparticle-number conservation, rather than conservation of total particle count in arbitrary interacting processes.

A [global symmetry in field theory](../../../quantum-field-theory.md#global-symmetry-in-field-theory) uses a spacetime-independent parameter and ordinarily relates physically distinct configurations. A [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance) instead has arbitrary local parameters and represents redundancy in the description. For example, the [Maxwell field](../../../electromagnetism.md#electromagnetic-field) is unchanged physically by $A_\mu\mapsto A_\mu+\partial_\mu\alpha(x)$: its [electromagnetic field tensor](../../../electromagnetism.md#electromagnetic-field-tensor) is unchanged. For charged matter use $D_\mu=\partial_\mu+iqA_\mu$ together with $\psi\mapsto e^{-iq\alpha(x)}\psi$. Differentiating shows $D'_\mu\psi'=e^{-iq\alpha}D_\mu\psi$, so the coupled [Dirac action](../../../relativistic-quantum-field.md#dirac-action) is locally gauge invariant. A local phase applied to free matter alone produces extra derivatives of $\alpha$ and is not an invariance; the compensating gauge field is necessary.

Local arbitrariness gives identities among field equations, rather than an independent physical charge for every function $\alpha$. In the pure [Maxwell field](../../../electromagnetism.md#electromagnetic-field), action invariance under a compactly supported $\alpha$ implies

$$
0=\int d^4x\,E^\nu\partial_\nu\alpha
=-\int d^4x\,\alpha\partial_\nu E^\nu,
\qquad E^\nu=\partial_\mu F^{\mu\nu}.
$$

Thus $\partial_\nu E^\nu=0$ holds off shell, directly because $F^{\mu\nu}$ is antisymmetric. This exemplifies the [Noether second theorem](../../../calculus-of-variations.md#noether-second-theorem). Gauge fixing and the [Gupta-Bleuler null-state quotient](../../../relativistic-quantum-field.md#gupta-bleuler-null-state-quotient) remove redundant photon components; they do not remove a physical global charge. Gauge transformations that are nontrivial at a boundary can carry boundary charges, so the redundancy statement concerns transformations satisfying the chosen boundary conditions. Finally, discrete symmetries such as the sign reversal of a real scalar or [parity symmetry in quantum field theory](../../../quantum-field-theory.md#parity-symmetry-in-quantum-field-theory) can be important without furnishing a continuous-parameter [Noether current](../../../quantum-field-theory.md#noether-current).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
