# Paper 301

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20301.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20301.pdf)

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

↑ **Parent:** [Paper 301](paper-301.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The translation changes the [Lagrangian density](../../../quantum-field-theory.md#lagrangian-density) by $\delta\mathcal L_0=\epsilon^\nu\partial_\nu\mathcal L_0=\partial_\mu(\epsilon^\mu\mathcal L_0)$. The [Noether current](../../../quantum-field-theory.md#noether-current) is therefore

$$
j^\mu=\frac{\partial\mathcal L_0}{\partial(\partial_\mu\psi)}\delta\psi-\epsilon^\mu\mathcal L_0
=\epsilon_\nu T^{\mu\nu},
\qquad
T^{\mu\nu}=i\bar\psi\gamma^\mu\partial^\nu\psi-\eta^{\mu\nu}\mathcal L_0.
$$

This is the [canonical stress-energy tensor](../../../quantum-field-theory.md#canonical-stress-energy-tensor). Directly,

$$
\partial_\mu T^{\mu\nu}
=\left(\frac{\partial\mathcal L_0}{\partial\psi}
-\partial_\mu\frac{\partial\mathcal L_0}{\partial(\partial_\mu\psi)}\right)\partial^\nu\psi
$$

up to the analogous adjoint-field term, so the [Euler-Lagrange field equations](../../../quantum-field-theory.md#euler-lagrange-field-equation) imply $\partial_\mu T^{\mu\nu}=0$ [on shell](../../../quantum-field-theory.md#on-shell). The [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) also gives $\mathcal L_0=0$ on shell.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

After using the [Clifford algebra](../../../algebra.md#clifford-algebra), integrations by parts and the [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation), every allowed Lorentz-covariant symmetric rank-two expression with one derivative reduces, modulo terms vanishing [on shell](../../../quantum-field-theory.md#on-shell) and identically conserved improvements, to an overall multiple of

$$
\bar\psi\gamma^{(\mu}\overleftrightarrow{\partial}^{\nu)}\psi.
$$

Thus the general nontrivial tensor in the stated class is

$$
\widehat T^{\mu\nu}
=C\left[
\bar\psi\gamma^\mu\partial^\nu\psi
+\bar\psi\gamma^\nu\partial^\mu\psi
-(\partial^\nu\bar\psi)\gamma^\mu\psi
-(\partial^\mu\bar\psi)\gamma^\nu\psi
\right].
$$

It is manifestly symmetric. Differentiating it, commuting partial derivatives and using

$$
i\gamma^\rho\partial_\rho\psi=m\psi,
\qquad
i(\partial_\rho\bar\psi)\gamma^\rho=-m\bar\psi,
$$

makes the terms cancel pairwise, proving $\partial_\mu\widehat T^{\mu\nu}=0$ on shell. The normalization $C$ remains free at this stage.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Choose $C=i/4$. Expanding

$$
S^{\lambda\mu\nu}=\frac12\bar\psi[\gamma^\lambda,\gamma^\mu]\gamma^\nu\psi
$$

with the [Clifford algebra](../../../algebra.md#clifford-algebra), applying the product rule and then using the [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) and its adjoint gives

$$
\widehat T^{\mu\nu}
=T^{\mu\nu}+\frac i4\left[
\partial_\lambda S^{\lambda\mu\nu}
-\partial^\nu(\bar\psi\gamma^\mu\psi)
\right].
$$

This is the [Belinfante-Rosenfeld stress-energy tensor](../../../quantum-field-theory.md#belinfante-rosenfeld-stress-energy-tensor) written as an improvement of the canonical tensor.

The translation charges are

$$
P^\nu=\int d^3x\,T^{0\nu},
\qquad
\widehat P^\nu=\int d^3x\,\widehat T^{0\nu}.
$$

For spatial $\nu$, their difference is the integral of $\partial_iS^{i0\nu}-\partial^\nu(\bar\psi\gamma^0\psi)$. For $\nu=0$, use conservation of the [Dirac current](../../../quantum-field-theory.md#dirac-current) to replace $\partial^0(\bar\psi\gamma^0\psi)$ by a spatial divergence; also $S^{00\nu}=0$. Hence $\widehat P^\nu-P^\nu$ is always a spatial boundary integral. Under the usual decay boundary condition it vanishes, so both currents generate the same four-momentum.

## 2

↑ **Parent:** [Paper 301](paper-301.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Under [spatial reflection](../../../quantum-mechanics.md#spatial-reflection), $\phi'(t,\mathbf x)=\gamma_p\phi(t,-\mathbf x)$, so

$$
\partial_0\phi'(t,\mathbf x)=\gamma_p\partial_0\phi(t,-\mathbf x),
\qquad
\partial_i\phi'(t,\mathbf x)=-\gamma_p\partial_i\phi(t,-\mathbf x).
$$

Because $\gamma_p^2=1$, the Lorentz scalar $\partial_\mu\phi\partial^\mu\phi$ and the mass term $m^2\phi^2$ are unchanged after evaluating at the reflected point. The spatial change of variables $\mathbf x\mapsto-\mathbf x$ has unit absolute Jacobian, so the action of the free [real scalar field](../../../scalar-field-theory.md#real-scalar-field) is invariant.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Insert the [mode expansion of a free field](../../../quantum-field-theory.md#mode-expansion-of-a-free-field) into the parity law and change integration variable $\mathbf k\mapsto-\mathbf k$. Independence of the plane waves gives

$$
\mathcal P a_{\mathbf k}\mathcal P^{-1}=\gamma_p a_{-\mathbf k},
\qquad
\mathcal P a_{\mathbf k}^\dagger\mathcal P^{-1}=\gamma_p a_{-\mathbf k}^\dagger.
$$

Since $\mathcal P|0\rangle=|0\rangle$, an $n$-particle [Fock state](../../../quantum-field-theory.md#fock-state) therefore transforms as

$$
\boxed{\mathcal P|\mathbf k_1,\ldots,\mathbf k_n\rangle
=(\gamma_p)^n|-\mathbf k_1,\ldots,-\mathbf k_n\rangle.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let

$$
N=\int\frac{d^3q}{(2\pi)^3}a_{\mathbf q}^\dagger a_{\mathbf q},
\qquad
K=\int\frac{d^3q}{(2\pi)^3}a_{\mathbf q}^\dagger a_{-\mathbf q}.
$$

The canonical commutation relations give $[N,a_{\mathbf k}]=-a_{\mathbf k}$ and $[K,a_{\mathbf k}]=-a_{-\mathbf k}$. Hence exponentiating the adjoint action gives

$$
\mathcal P_1a_{\mathbf k}\mathcal P_1^{-1}
=e^{i\pi/2}a_{\mathbf k}=ia_{\mathbf k}.
$$

Writing $R a_{\mathbf k}=a_{-\mathbf k}$, one has $R^2=1$ and $\operatorname{ad}_K=-R$ on annihilation operators. Therefore

$$
\boxed{\mathcal P_2a_{\mathbf k}\mathcal P_2^{-1}
=e^{-i\gamma_p\pi R/2}a_{\mathbf k}
=-i\gamma_p a_{-\mathbf k}.}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [number operator](../../../quantum-mechanics.md#number-operator) $N$ is self-adjoint. Also

$$
K^\dagger=\int\frac{d^3q}{(2\pi)^3}a_{-\mathbf q}^\dagger a_{\mathbf q}=K
$$

after $\mathbf q\mapsto-\mathbf q$. Thus both exponents are anti-Hermitian and $\mathcal P_1,\mathcal P_2$ are [unitary](../../../vector-space.md#unitary-operator). Their product obeys

$$
(\mathcal P_1\mathcal P_2)a_{\mathbf k}(\mathcal P_1\mathcal P_2)^{-1}
=\gamma_pa_{-\mathbf k},
$$

and likewise for creation operators. Both generators annihilate the vacuum, so the product leaves it invariant. Substitution in the free-field mode expansion yields

$$
(\mathcal P_1\mathcal P_2)\phi(t,\mathbf x)(\mathcal P_1\mathcal P_2)^{-1}
=\gamma_p\phi(t,-\mathbf x).
$$

**Hence $\mathcal P=\mathcal P_1\mathcal P_2$ implements parity with [intrinsic parity](../../../quantum-field-theory.md#intrinsic-parity) $\gamma_p$.**

## 3

↑ **Parent:** [Paper 301](paper-301.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Varying the displayed gauge-fixed [Lagrangian density](../../../quantum-field-theory.md#lagrangian-density) gives the kinetic operator

$$
D^{\mu\rho}=\eta^{\mu\rho}\Box-\left(1-\frac1\alpha\right)\partial^\mu\partial^\rho.
$$

Its [quantum field theory propagator](../../../quantum-field-theory.md#propagator) should satisfy

$$
D_x^{\mu\rho}\Delta_{\rho\nu}(x-y)=i\delta^\mu_\nu\delta^{(4)}(x-y),
$$

and inversion into transverse and longitudinal projectors gives the numerator

$$
\Pi_{\mu\nu}^{\mathrm{correct}}
=-\eta_{\mu\nu}+(1-\alpha)\frac{k_\mu k_\nu}{k^2}.
$$

The paper instead prints $-\eta_{\mu\nu}+(\alpha-1)k_\mu k_\nu/k^2$. Except at $\alpha=1$, that is not the inverse of the displayed Lagrangian's kinetic operator. Taken literally, for $\alpha\ne2$ it is the Green function of

$$
\left[\eta^{\mu\rho}\Box+\frac{\alpha-1}{2-\alpha}
\partial^\mu\partial^\rho\right]\Delta_{\rho\nu}
=i\delta^\mu_\nu\delta^{(4)},
$$

and at $\alpha=2$ its longitudinal part is noninvertible. Thus the longitudinal sign in the printed propagator is a typographical error; the two forms coincide in [Feynman gauge](../../../relativistic-quantum-field.md#feynman-gauge).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $G_{\mu\nu}(x,y)=\langle\Omega|T A_\mu(x)A_\nu(y)|\Omega\rangle$. Invariance of the normalized path integral under $A\mapsto A+\delta A$ gives the [Schwinger-Dyson equation](../../../perturbative-quantum-field-theory.md#schwinger-dyson-equation)

$$
D_x^{\mu\rho}G_{\rho\nu}(x,y)
=i\delta^\mu_\nu\delta^{(4)}(x-y)
+e j^\mu(x)\langle A_\nu(y)\rangle_j,
$$

together with $D^{\mu\rho}\langle A_\rho\rangle_j=e j^\mu$. This assumes the functional measure is translation invariant, boundary terms in field space vanish, and vacuum bubbles are removed by normalization. The current is a fixed c-number and conserved; conservation removes dependence on the longitudinal, gauge-parameter part of the [photon propagator](../../../quantum-field-theory.md#photon-propagator). An $i\epsilon$ prescription and adiabatic switching select the interacting vacuum.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Since $D\Delta=i\delta$, the source-induced one-point function is

$$
\langle A_\mu(x)\rangle_j
=-ie\int d^4z\,\Delta_{\mu\rho}(x-z)j^\rho(z).
$$

The action is quadratic and the source is linear, so completing the square gives the exact full two-point function

$$
G_{\mu\nu}(x,y)=\Delta_{\mu\nu}(x-y)
-e^2\int d^4z\,d^4w\,
\Delta_{\mu\rho}(x-z)j^\rho(z)
\Delta_{\nu\sigma}(y-w)j^\sigma(w).
$$

Diagrammatically these are a free line joining $x$ to $y$ and a disconnected pair of lines, each joining one external insertion to one current cross. The connected two-point function remains exactly $\Delta_{\mu\nu}$. The expansion truncates at $e^2$ because a Gaussian integral has no interaction vertices and its mean is linear in $e$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For [quantum electrodynamics](../../../perturbative-quantum-field-theory.md#quantum-electrodynamics), $j^\mu=\bar\psi\gamma^\mu\psi$ is an operator built from a dynamical [Dirac field](../../../relativistic-quantum-field.md#dirac-field). Integrating over $\psi,\bar\psi$ generates arbitrarily high powers of $e$, so the Gaussian-source truncation fails.

For the connected photon two-point function, the required diagrams through $e^4$ are: the bare photon line at $e^0$; one fermion-loop [photon vacuum polarization](../../../perturbative-quantum-field-theory.md#photon-vacuum-polarization) insertion at $e^2$; and at $e^4$, a photon line with two successive one-loop polarization insertions together with the two-loop one-particle-irreducible fermion loop whose loop contains one internal photon chord. The latter includes the cyclic placements conventionally interpreted as self-energy and vertex corrections. Counterterm insertions must be added in a renormalized calculation. Disconnected vacuum bubbles cancel against the vacuum normalization.

## 4

↑ **Parent:** [Paper 301](paper-301.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Expanding the covariant derivatives of [scalar quantum electrodynamics](../../../relativistic-quantum-field.md#scalar-electrodynamics) gives

$$
\mathcal L_{\mathrm{free}}
=-\frac14F_{\mu\nu}F^{\mu\nu}
+\partial_\mu\phi^*\partial^\mu\phi-m^2\phi^*\phi
$$

and

$$
\mathcal L_{\mathrm{int}}
=ieA_\mu(\phi\partial^\mu\phi^*-\phi^*\partial^\mu\phi)
+e^2A_\mu A^\mu\phi^*\phi.
$$

In four dimensions, $[A_\mu]=[\phi]=1$ and $[\partial_\mu]=1$, so $[e]=0$. Both interactions have dimension four and $e$ is a [marginal coupling](../../../perturbative-quantum-field-theory.md#marginal-coupling) by [power counting in quantum field theory](../../../perturbative-quantum-field-theory.md#power-counting-in-quantum-field-theory).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

With all momenta directed into each vertex, the momentum-space [Feynman rules](../../../perturbative-quantum-field-theory.md#feynman-rule) are:

- scalar line of momentum $p$: $i/(p^2-m^2+i\epsilon)$;
- photon line in [Feynman gauge](../../../relativistic-quantum-field.md#feynman-gauge): $-i\eta_{\mu\nu}/(k^2+i\epsilon)$;
- one photon of index $\mu$, scalar momentum $p$ and conjugate-scalar momentum $p'$: $ie(p-p')^\mu$;
- the [seagull vertex](../../../perturbative-quantum-field-theory.md#seagull-vertex) with photon indices $\mu,\nu$: $2ie^2\eta^{\mu\nu}$.

Each vertex also carries its momentum-conserving delta function; integrate every independent loop momentum and attach the appropriate external wavefunctions and photon polarization vectors.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Three connected [tree-level Feynman diagrams](../../../perturbative-quantum-field-theory.md#tree-level-feynman-diagram) contribute at order $e^2$: a scalar-exchange diagram in which photon $k_1$ is emitted before $k_2$ along the charged scalar line; the crossed scalar-exchange diagram with $k_1$ and $k_2$ interchanged; and the local [seagull vertex](../../../perturbative-quantum-field-theory.md#seagull-vertex) joining both incoming scalars and both outgoing photons. The exchange denominators are $(p_1-k_1)^2-m^2$ and $(p_1-k_2)^2-m^2$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Let $p_1,p_2$ be the incoming scalar and antiscalar momenta and $k_1,k_2$ the outgoing photon momenta, so $p_1+p_2=k_1+k_2$. Up to the common overall phase fixed by the $S$-matrix convention, the connected leading amplitude is

$$
\mathcal M=e^2\epsilon_{1\mu}^*\epsilon_{2\nu}^*\mathcal M^{\mu\nu},
$$

where

$$
\mathcal M^{\mu\nu}
=2\eta^{\mu\nu}
+\frac{(2p_1-k_1)^\mu(2p_2-k_2)^\nu}{(p_1-k_1)^2-m^2}
+\frac{(2p_2-k_1)^\mu(2p_1-k_2)^\nu}{(p_1-k_2)^2-m^2}.
$$

On shell, the denominators are $-2p_1\cdot k_1=-2p_2\cdot k_2$ and $-2p_1\cdot k_2=-2p_2\cdot k_1$. Contracting with $k_{1\mu}$ therefore gives

$$
k_{1\mu}\mathcal M^{\mu\nu}epsilon_{2\nu}^*
=2k_1\cdot\epsilon_2^*
-(2p_2-k_2)\cdot\epsilon_2^*
-(2p_1-k_2)\cdot\epsilon_2^*=0,
$$

using momentum conservation and $k_2\cdot\epsilon_2=0$. The same calculation with the photons interchanged gives $k_{2\nu}\mathcal M^{\mu\nu}\epsilon_{1\mu}^*=0$. The two exchange diagrams and the seagull term are all required for this [Ward identity](../../../perturbative-quantum-field-theory.md#ward-identity).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
