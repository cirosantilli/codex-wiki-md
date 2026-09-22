# Paper 301

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_301.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_301.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
    - [iv](#2/a/iv)
      - [Solution](#2/a/iv/solution)
    - [v](#2/a/v)
      - [Solution](#2/a/v/solution)
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
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
    - [iv](#3/a/iv)
      - [Solution](#3/a/iv/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
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

↑ **Parent:** [Paper 301](paper-301.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

In four dimensions, $[\psi]=3/2$, $[A_\mu]=1$, and $[F_{\mu\nu}]=2$. The minimal-coupling operator $\bar\psi\gamma^\mu A_\mu\psi$ has dimension four, so $[e]=0$ and $e$ is a [marginal coupling](../../../perturbative-quantum-field-theory.md#marginal-coupling). The [Pauli term](../../../perturbative-quantum-field-theory.md#pauli-term) $\bar\psi[\gamma^\mu,\gamma^\nu]F_{\mu\nu}\psi$ has dimension five, so $[\lambda]=-1$ and $\lambda$ is an [irrelevant coupling](../../../perturbative-quantum-field-theory.md#irrelevant-coupling) by [power counting in quantum field theory](../../../perturbative-quantum-field-theory.md#power-counting-in-quantum-field-theory).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For $x'=\Lambda x$, a [Dirac spinor](../../../relativistic-quantum-field.md#dirac-spinor) and vector field transform as

$$
\psi'(x')=S(\Lambda)\psi(x),
\qquad
\bar\psi'(x')=\bar\psi(x)S(\Lambda)^{-1},
\qquad
A'_\mu(x')=\Lambda_\mu{}^\nu A_\nu(x),
$$

where $S^{-1}\gamma^\mu S=\Lambda^\mu{}_\nu\gamma^\nu$. Hence the spinor terms and $F_{\mu\nu}F^{\mu\nu}$ are [Lorentz scalars](../../../special-relativity.md#lorentz-scalar). The Maxwell term is real. Integration by parts and $(\gamma^\mu)^\dagger=\gamma^0\gamma^\mu\gamma^0$ show that the adjoint of $i\bar\psi\gamma^\mu D_\mu\psi$ differs from it by $-i\partial_\mu(\bar\psi\gamma^\mu\psi)$. Finally, $i[\gamma^\mu,\gamma^\nu]$ is Dirac-Hermitian, so the real coefficient $\lambda$ makes the Pauli bilinear real. Thus the action is real.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Varying $\bar\psi$ and $\psi$ independently gives

$$
\left(i\not D-i\lambda[\gamma^\mu,\gamma^\nu]F_{\mu\nu}\right)\psi=0
$$

and its adjoint

$$
i(D_\mu\bar\psi)\gamma^\mu
+i\lambda\bar\psi[\gamma^\mu,\gamma^\nu]F_{\mu\nu}=0,
$$

where $D_\mu\bar\psi=\partial_\mu\bar\psi-ieA_\mu\bar\psi$. Varying $A_\nu$ and integrating the Pauli term by parts gives the modified [Maxwell equations](../../../electromagnetism.md#maxwell-equations)

$$
\boxed{\partial_\mu F^{\mu\nu}
=e\bar\psi\gamma^\nu\psi
-2i\lambda\partial_\mu\!\left(
\bar\psi[\gamma^\mu,\gamma^\nu]\psi\right).}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The local [U(1) gauge symmetry](../../../relativistic-quantum-field.md#u-1-gauge-symmetry) is

$$
\psi\mapsto e^{ie\chi(x)}\psi,
\qquad
\bar\psi\mapsto\bar\psi e^{-ie\chi(x)},
\qquad
A_\mu\mapsto A_\mu-\partial_\mu\chi.
$$

The global phase subgroup has [Noether current](../../../quantum-field-theory.md#noether-current) and charge

$$
j^\mu=\bar\psi\gamma^\mu\psi,
\qquad
Q=\int d^3x\,j^0=\int d^3x\,\psi^\dagger\psi.
$$

Multiplying the fermion equation by $\bar\psi$, its adjoint by $\psi$, and subtracting shows $\partial_\mu j^\mu=0$ on shell. Therefore $\dot Q=-\int d^3x\,\boldsymbol\nabla\cdot\mathbf j=0$ under vanishing boundary flux.

The source in Maxwell's equation is

$$
J^\nu=e j^\nu-2i\lambda\partial_\mu
(\bar\psi[\gamma^\mu,\gamma^\nu]\psi).
$$

The second term is an identically conserved [magnetization current](../../../electromagnetism.md#magnetization-current), because it is the divergence of an antisymmetric tensor. It changes the local source but contributes only a boundary term to the total charge.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

For the [chiral transformation](../../../relativistic-quantum-field.md#chiral-transformation) $\psi\mapsto e^{i\alpha\gamma^5}\psi$, one also has $\bar\psi\mapsto\bar\psi e^{i\alpha\gamma^5}$. The massless kinetic and vector-current terms are invariant because $\{\gamma^5,\gamma^\mu\}=0$. Since $\gamma^5$ commutes with $[\gamma^\mu,\gamma^\nu]$, the Pauli bilinear transforms with $e^{2i\alpha\gamma^5}$ and is not invariant. Thus the continuous classical axial symmetry requires $\lambda=0$.

A fermion mass also breaks the symmetry, so in the massive theory one additionally needs $m=0$, which contradicts a genuinely massive fermion. Making $\alpha$ local produces $(\partial_\mu\alpha)\bar\psi\gamma^\mu\gamma^5\psi$. No choice of the vector coupling $e$ or Pauli coupling $\lambda$ cancels this term; gauging it requires an axial gauge field, and at the quantum level one must also address the [chiral anomaly](../../../relativistic-quantum-field.md#chiral-anomaly).

## 2

↑ **Parent:** [Paper 301](paper-301.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

Integrating by parts gives

$$
\widetilde a=-a,
\qquad
\widetilde b=-(b+c),
$$

because the $b$ and $c$ terms differ only by a total derivative. Hence

$$
\boxed{\mathcal L\simeq
\widetilde a V_\nu\Box V^\nu
+\widetilde b V^\nu\partial_\nu\partial_\mu V^\mu
+m^2V^\mu V_\mu.}
$$

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

The differential operators are self-adjoint under integration by parts, so the [Euler-Lagrange field equations](../../../quantum-field-theory.md#euler-lagrange-field-equation) are

$$
\boxed{\widetilde a\Box V^\nu
+\widetilde b\partial^\nu(\partial\cdot V)
+m^2V^\nu=0.}
$$

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

Using the original first-derivative Lagrangian, its momentum current is

$$
\Pi^{\mu\rho}
=2a\partial^\mu V^\rho
+2b\partial^\rho V^\mu
+2c\eta^{\mu\rho}\partial\cdot V.
$$

Translation invariance and [Noether theorem](../../../calculus-of-variations.md#noether-theorem) give the [canonical stress-energy tensor](../../../quantum-field-theory.md#canonical-stress-energy-tensor)

$$
T^{\mu}{}_{\nu}=\Pi^{\mu\rho}\partial_\nu V_\rho
-\delta^\mu_\nu\mathcal L,
\qquad
\partial_\mu T^{\mu}{}_{\nu}=0
$$

on shell. The Hamiltonian is

$$
\boxed{H=\int d^3x\,T^0{}_0
=\int d^3x\left(\Pi^{0\rho}\dot V_\rho-\mathcal L\right).}
$$

<h4 id="2/a/iv">iv</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/a/iv)

When $\widetilde b=0$, integration by parts makes the kinetic term $-\widetilde a\partial_\mu V_\nu\partial^\mu V^\nu$. The Lorentzian contraction over the field index gives the time component and the three spatial components opposite kinetic-energy signs. Reversing the sign of $\widetilde a$ merely exchanges which component is a [ghost field](../../../quantum-field-theory.md#ghost-field); no nonzero choice makes all four energies positive. At $\widetilde a=0$ there is no healthy kinetic term. Thus the Hamiltonian is never positive definite.

<h4 id="2/a/v">v</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/v/solution">Solution</h5>

↑ **Parent:** [V](#2/a/v)

Positivity selects

$$
\widetilde b=-\widetilde a,
$$

for which the kinetic terms combine, up to normalization and a total derivative, into the [Proca field](../../../electromagnetism.md#proca-field) form $-F_{\mu\nu}F^{\mu\nu}/4$. Taking the divergence of the equation of motion gives

$$
(\widetilde a+\widetilde b)\Box(\partial\cdot V)
+m^2\partial\cdot V=0.
$$

For the selected relation and $m\ne0$, this implies the [transverse vector field](../../../electromagnetism.md#transverse-vector-field) condition $\partial_\mu V^\mu=0$. The remaining three massive polarizations have positive on-shell energy when $\widetilde a>0$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Put $\widetilde c=\widetilde a+\widetilde b$. Substituting the [transverse-longitudinal decomposition](../../../quantum-field-theory.md#transverse-longitudinal-decomposition) $V_\mu=A_\mu+\partial_\mu\pi$ and integrating cross terms by parts gives

$$
\mathcal L\simeq
\widetilde a A_\mu\Box A^\mu+m^2A_\mu A^\mu
-\widetilde c(\Box\pi)^2+m^2\partial_\mu\pi\partial^\mu\pi.
$$

The equations are

$$
(\widetilde a\Box+m^2)A_\mu=0,
\qquad
\Box(\widetilde c\Box+m^2)\pi=0,
$$

together with $\partial_\mu A^\mu=0$.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

The scalar kinetic operator is proportional in momentum space to $k^2(\widetilde c k^2-m^2)$. Its inverse has the partial-fraction decomposition

$$
\frac{i}{k^2(\widetilde c k^2-m^2)}
=-\frac{i}{m^2}\left(
\frac1{k^2}-\frac{\widetilde c}{\widetilde c k^2-m^2}
\right),
$$

up to the overall convention-dependent factor allowed in the question. Thus $\widetilde c=\widetilde a+\widetilde b$. Under the physical relation $\widetilde b=-\widetilde a$, one has $\widetilde c=0$, so the extra massive pole and its ghost residue disappear.

## 3

↑ **Parent:** [Paper 301](paper-301.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

The classical equations are

$$
(\Box+M^2)\phi+\lambda\bar\psi\psi=0,
\qquad
(i\not\partial-m-\lambda\phi)\psi=0,
\qquad
i(\partial_\mu\bar\psi)\gamma^\mu+m\bar\psi+\lambda\phi\bar\psi=0.
$$

For any time-ordered functional $\mathcal O$, the three [Schwinger-Dyson equations](../../../perturbative-quantum-field-theory.md#schwinger-dyson-equation) state that insertion of each left-hand side equals the corresponding contact terms obtained by $-i$ times the functional derivative of $\mathcal O$ with respect to $phi$, $\bar\psi$, or $\psi$, with the usual reversed order and Grassmann signs for fermionic derivatives.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Define asymptotic states $|\phi(k)\rangle=a_k^\dagger|0\rangle$ and $|\psi(p,s)\bar\psi(q,s')\rangle=b_{p,s}^\dagger c_{q,s'}^\dagger|0\rangle$. The [LSZ reduction formula](../../../perturbative-quantum-field-theory.md#lsz-reduction-formula) reduces the decay matrix element from the connected three-point function

$$
G(x,y,z)=\langle0|T\phi(x)\psi(y)\bar\psi(z)|0\rangle_c.
$$

In momentum space, amputate the scalar leg with $i(k^2-M^2)$ and the fermion legs with the inverse Dirac propagators, contract them with $\bar u^s(p)$ and $v^{s'}(q)$, and take $k^2=M^2$, $p^2=q^2=m^2$. The spacetime integrations produce $(2\pi)^4\delta^{(4)}(k-p-q)$.

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

Iterating the Schwinger-Dyson equations once, the leading connected correlator is one scalar propagator and two Dirac propagators meeting at one [Yukawa interaction](../../../standard-model.md#yukawa-interaction) vertex. Amputation gives

$$
\langle p,s;q,s'\,\mathrm{out}|k\,\mathrm{in}\rangle_c
=(2\pi)^4\delta^{(4)}(k-p-q)
\left[-i\lambda\bar u^s(p)v^{s'}(q)\right].
$$

**Thus the invariant amplitude, in the convention $S_{fi}=i(2\pi)^4\delta^{(4)}\mathcal M_{fi}$, is $\mathcal M_{s,s'}=-\lambda\bar u^s(p)v^{s'}(q)$.**

<h4 id="3/a/iv">iv</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/a/iv)

The [spin sum](../../../relativistic-quantum-field.md#spin-sum) becomes a [gamma-matrix trace](../../../relativistic-quantum-field.md#gamma-matrix-trace):

$$
\sum_{s,s'}|\lambda\bar u^s(p)v^{s'}(q)|^2
=\lambda^2\operatorname{tr}[(\not p+m)(\not q-m)]
=4\lambda^2(p\cdot q-m^2).
$$

Since $(p+q)^2=M^2$, $p\cdot q=(M^2-2m^2)/2$. Therefore the normalization requested in the paper gives

$$
\boxed{\mathcal P=\frac14\sum_{s,s'}|\mathcal A_{s,s'}|^2
=\frac{\lambda^2}{2}(M^2-4m^2).}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The pseudoscalar vertex replaces $-i\lambda$ by $g\gamma^5$, so

$$
S_{fi}^{(5)}=(2\pi)^4\delta^{(4)}(k-p-q)
g\bar u^s(p)\gamma^5v^{s'}(q).
$$

Using $\gamma^5\not q\gamma^5=-\not q$ with the conjugation sign gives

$$
\mathcal P_5=\frac{g^2}{2}M^2.
$$

The interactions are experimentally distinguishable through the decay rate and its threshold behavior: scalar decay is proportional to $(1-4m^2/M^2)^{3/2}$, whereas pseudoscalar decay is proportional to $(1-4m^2/M^2)^{1/2}$. Spin and parity correlations provide further discrimination.

## 4

↑ **Parent:** [Paper 301](paper-301.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Substitution of $\Phi=\varphi+\lambda\varphi^2$ gives

$$
\mathcal L_{\mathrm{free}}
=\frac12(\partial\varphi)^2-\frac12m^2\varphi^2
$$

and

$$
\mathcal L_{\mathrm{int}}
=2\lambda\varphi(\partial\varphi)^2-m^2\lambda\varphi^3
+2\lambda^2\varphi^2(\partial\varphi)^2
-\frac12m^2\lambda^2\varphi^4.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

With all momenta incoming, the [Feynman rules](../../../perturbative-quantum-field-theory.md#feynman-rule) are

$$
\text{propagator: }\frac{i}{p^2-m^2+i\epsilon},
$$



$$
\text{three-point vertex: }
2i\lambda\sum_{j=1}^3(p_j^2-m^2),
$$

and

$$
\text{four-point vertex: }
4i\lambda^2\left(\sum_{j=1}^4p_j^2-3m^2\right).
$$

Each vertex includes its momentum-conserving delta function. The combinatorial factors follow by assigning the identical fields to the differentiated and undifferentiated slots in every possible way.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

At order $\lambda^2$, four connected [tree-level Feynman diagrams](../../../perturbative-quantum-field-theory.md#tree-level-feynman-diagram) contribute: one four-point contact diagram and three diagrams with two cubic vertices joined by a scalar propagator in the $s$, $t$, and $u$ channels.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

On shell, the contact vertex is $4i\lambda^2m^2$. At a cubic vertex with two external on-shell legs and internal momentum $k$, the rule reduces to $2i\lambda(k^2-m^2)$. The propagator cancels one such factor, so the three exchange diagrams sum to

$$
-4i\lambda^2[(s-m^2)+(t-m^2)+(u-m^2)].
$$

For equal-mass two-to-two scattering, $s+t+u=4m^2$, and the exchange sum is $-4i\lambda^2m^2$. It cancels the contact diagram exactly. Thus the connected on-shell amplitude vanishes, as required by the [equivalence theorem for field redefinitions](../../../perturbative-quantum-field-theory.md#equivalence-theorem-for-field-redefinitions): an invertible local field redefinition cannot turn a free theory into a physically interacting one.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
