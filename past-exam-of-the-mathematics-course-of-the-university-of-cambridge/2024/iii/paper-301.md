# Paper 301

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_301.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_301.pdf)

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
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
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

## 1

↑ **Parent:** [Paper 301](paper-301.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Under $A_\mu\mapsto A_\mu+\partial_\mu\alpha$, the field strength is unchanged, but the mass term in the [Proca action](../../../electromagnetism.md#proca-action) changes by

$$
\frac{m^2}{2}\{2A^\mu\partial_\mu\alpha+(\partial\alpha)^2\},
$$

which is not generally a total derivative. The mass therefore breaks [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance).

The [Euler-Lagrange field equation](../../../quantum-field-theory.md#euler-lagrange-field-equation) is

$$
\partial_\mu F^{\mu\nu}+m^2A^\nu=0.
$$

Taking its divergence and using the antisymmetry of $F^{\mu\nu}$ gives $m^2\partial_\nu A^\nu=0$. Since $m>0$, the [Lorenz constraint in Proca theory](../../../electromagnetism.md#lorenz-constraint-in-proca-theory) follows. Substitution back into the field equation then gives

$$
\boxed{(\Box+m^2)A^\nu=0,
\qquad
\partial_\nu A^\nu=0.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The symmetric [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) obtained by metric variation is

$$
T^{\mu\nu}=-F^{\mu\rho}F^\nu{}_{\rho}
+\frac14\eta^{\mu\nu}F^{\rho\sigma}F_{\rho\sigma}
+m^2\left(A^\mu A^\nu-\frac12\eta^{\mu\nu}A^\rho A_\rho\right).
$$

It is conserved on shell. With signature $(+---)$ its energy density is

$$
T^{00}=\frac12(\mathbf E^2+\mathbf B^2)
+\frac{m^2}{2}\{(A^0)^2+\mathbf A^2\}\geq0.
$$

The [canonical stress-energy tensor](../../../quantum-field-theory.md#canonical-stress-energy-tensor) differs from this symmetric tensor by the divergence of $F^{\mu\rho}A^\nu$ plus terms proportional to the field equation. Thus its integrated energy agrees after discarding the corresponding total spatial derivative, and positivity holds on shell.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For the [plane wave](../../../quantum-mechanics.md#plane-wave) $A^\mu(x)=\epsilon^\mu(k)e^{-ik\cdot x}$, the equations from part a become

$$
k^2=m^2,
\qquad
k_\mu\epsilon^\mu=0.
$$

In the rest frame $k^\mu=(m,\mathbf0)$, transversality sets $\epsilon^0=0$ while the three spatial components remain independent. Hence a [Proca field](../../../electromagnetism.md#proca-field) has three polarization states, as required for a massive spin-one particle. A covariant orthonormal choice obeys

$$
\boxed{\sum_{\lambda=1}^3\epsilon_\mu^{(\lambda)}(k)epsilon_\nu^{(\lambda)}(k)^*
=-\eta_{\mu\nu}+\frac{k_\mu k_\nu}{m^2}.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The quadratic momentum-space operator is inverted by the [Proca propagator](../../../electromagnetism.md#proca-propagator). With the [Feynman propagator](../../../quantum-field-theory.md#feynman-propagator) boundary prescription,

$$
\Delta_{\mu\nu}(x-y)
=\int\frac{d^4p}{(2\pi)^4}
\frac{-i}{p^2-m^2+i\epsilon}
\left(\eta_{\mu\nu}-\frac{p_\mu p_\nu}{m^2}\right)
e^{-ip\cdot(x-y)}.
$$

Multiplication by the Fourier-space Proca operator gives $i\delta_\mu{}^\nu$, with the overall sign determined by the convention for the Green function.

## 2

↑ **Parent:** [Paper 301](paper-301.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

In four spacetime dimensions the action is dimensionless, so the [mass dimension](../../../perturbative-quantum-field-theory.md#mass-dimension) of the Lagrangian density is $[\mathcal L]=4$. The kinetic term gives $[\phi]=1$, and $g\phi^3$ then gives

$$
[g]=4-3[\phi]=1.
$$

**Thus $g$ has mass dimension one and is a [relevant coupling](../../../perturbative-quantum-field-theory.md#relevant-coupling) under [power counting in quantum field theory](../../../perturbative-quantum-field-theory.md#power-counting-in-quantum-field-theory).**

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The momentum-space [Feynman rules](../../../perturbative-quantum-field-theory.md#feynman-rule) for [Phi cubed theory](../../../scalar-field-theory.md#phi-cubed-theory) are

$$
\text{internal scalar line: }\frac{i}{p^2-m^2+i\epsilon},
\qquad
\text{cubic vertex: }-ig.
$$

Each vertex carries $(2\pi)^4\delta^{(4)}$ of momentum conservation, each independent loop momentum is integrated with $d^4\ell/(2\pi)^4$, and a graph is divided by its [Feynman-diagram symmetry factor](../../../perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor). External propagators are omitted from an amputated [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $G_5$ be the connected time-ordered five-point function. The [LSZ reduction formula](../../../perturbative-quantum-field-theory.md#lsz-reduction-formula) gives, up to one factor $Z^{-1/2}$ per external leg,

$$
\begin{aligned}
\langle k_1k_2k_3,\mathrm{out}|p_1p_2,\mathrm{in}\rangle_c
={}&\prod_{r=1}^3\left[i\int d^4x_r\,e^{ik_r\cdot x_r}(\Box_{x_r}+m^2)\right]\\
&\times\prod_{s=1}^2\left[i\int d^4y_s\,e^{-ip_s\cdot y_s}(\Box_{y_s}+m^2)\right]
G_5(x_1,x_2,x_3,y_1,y_2).
\end{aligned}
$$

Translation invariance factors this as

$$
\boxed{i(2\pi)^4\delta^{(4)}\!\left(p_1+p_2-\sum_{r=1}^3k_r\right)\mathcal M_{2\to3}.}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

A [connected Feynman diagram](../../../perturbative-quantum-field-theory.md#connected-feynman-diagram) that is a cubic tree with five external legs has three vertices and two internal lines. Its unique unlabeled topology is a chain: two external legs meet at each end vertex and one external leg attaches to the middle vertex. The [five-point tree amplitude in phi cubed theory](../../../scalar-field-theory.md#five-point-tree-amplitude-in-phi-cubed-theory) therefore has fifteen labeled [tree-level Feynman diagrams](../../../perturbative-quantum-field-theory.md#tree-level-feynman-diagram): choose the middle external leg in five ways, then partition the remaining four legs into two unordered pairs in three ways.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Take all external momenta incoming, $q_1=p_1$, $q_2=p_2$, and $q_{2+r}=-k_r$. For a diagram whose middle leg is $a$ and whose two end pairs are $\{b,c\}$ and $\{d,e\}$, the [Feynman rules](../../../perturbative-quantum-field-theory.md#feynman-rule) give

$$
i\mathcal M_{a|bc|de}
=(-ig)^3
\frac{i}{(q_b+q_c)^2-m^2+i\epsilon}
\frac{i}{(q_d+q_e)^2-m^2+i\epsilon}.
$$

Equivalently,

$$
\mathcal M_{a|bc|de}
=-\frac{g^3}{[(q_b+q_c)^2-m^2+i\epsilon][(q_d+q_e)^2-m^2+i\epsilon]}.
$$

The full connected tree amplitude is the sum over the fifteen choices described in part d, multiplied by the overall momentum-conserving delta function from part c.

## 3

↑ **Parent:** [Paper 301](paper-301.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use $D_\mu=\partial_\mu+ieA_\mu$. The two Lagrangians are

$$
\mathcal L_{\mathrm{SQED}}=(D_\mu\phi)^*D^\mu\phi-M^2\phi^*\phi-\frac14F_{\mu\nu}F^{\mu\nu}
$$

and

$$
\mathcal L_{\mathrm{QED}}=\bar\psi(i\gamma^\mu D_\mu-m)\psi-\frac14F_{\mu\nu}F^{\mu\nu}.
$$

Both are invariant under the [U(1) gauge symmetry](../../../relativistic-quantum-field.md#u-1-gauge-symmetry)

$$
\phi\mapsto e^{-ie\alpha(x)}\phi,
\qquad
\psi\mapsto e^{-ie\alpha(x)}\psi,
\qquad
A_\mu\mapsto A_\mu+\partial_\mu\alpha.
$$

For the constant phase subgroup, normalized to unit matter charge, the [Noether currents](../../../quantum-field-theory.md#noether-current) are

$$
j^\mu_{\mathrm{SQED}}=i\{\phi^*D^\mu\phi-(D^\mu\phi)^*\phi\},
\qquad
j^\mu_{\mathrm{QED}}=\bar\psi\gamma^\mu\psi.
$$

Their electric currents are $e j^\mu$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Under [charge conjugation](../../../quantum-field-theory.md#charge-conjugation), $\phi\leftrightarrow\phi^*$ must be accompanied by

$$
A_\mu\mapsto-A_\mu.
$$

Then $D_\mu\phi$ is exchanged with $(D_\mu\phi)^*$, while $F_{\mu\nu}\mapsto-F_{\mu\nu}$. The scalar kinetic and mass terms are therefore exchanged with themselves and $F_{\mu\nu}F^{\mu\nu}$ is unchanged, proving invariance of [scalar quantum electrodynamics](../../../relativistic-quantum-field.md#scalar-electrodynamics).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Write $\psi^C=\mathcal C\bar\psi^T$ and $\bar\psi^C=\psi^T\mathcal C$. Anticommuting the spinor fields and using $\mathcal C^{-1}(\gamma^\mu)^T\mathcal C=-\gamma^\mu$ gives

$$
\bar\psi^C\psi^C=\bar\psi\psi,
\qquad
\bar\psi^C\gamma^\mu\psi^C=-\bar\psi\gamma^\mu\psi.
$$

The free Dirac terms are invariant up to the total derivative used to move the derivative between the two anticommuting fields. The QED interaction $-e\bar\psi\gamma^\mu\psi A_\mu$ is also invariant because both the [Dirac current](../../../quantum-field-theory.md#dirac-current) and $A_\mu$ are odd. Together with $F_{\mu\nu}F^{\mu\nu}$ invariance, this proves charge-conjugation invariance of [quantum electrodynamics](../../../perturbative-quantum-field-theory.md#quantum-electrodynamics).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $\widehat C|\Omega\rangle=|\Omega\rangle$. Since charge conjugation sends both $A_\mu$ and either Noether current to its negative and commutes with time ordering,

$$
\langle\Omega|T\mathcal O_1\cdots\mathcal O_n|\Omega\rangle
=(-1)^n\langle\Omega|T\mathcal O_1\cdots\mathcal O_n|\Omega\rangle.
$$

For odd $n$ the correlator equals its negative and hence vanishes. This operator argument is exact and does not use a perturbation expansion. It is [Furry's theorem](../../../quantum-field-theory.md#furry-s-theorem): scattering amplitudes with an odd number of external photons and no charged external particles vanish to every order, whereas even-photon scattering is allowed.

## 4

↑ **Parent:** [Paper 301](paper-301.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

In the [Weyl representation of the gamma matrices](../../../relativistic-quantum-field.md#weyl-representation-of-the-gamma-matrices),

$$
\gamma^\mu=\begin{pmatrix}0&\sigma^\mu\\\bar\sigma^\mu&0\end{pmatrix},
\qquad
\gamma^5=\begin{pmatrix}-I&0\\0&I\end{pmatrix},
\qquad
\psi=\binom{u_L}{u_R}.
$$

A [Lorentz transformation](../../../special-relativity.md#lorentz-transformation) acts as $\psi'(x')=S(\Lambda)\psi(x)$ with $S(\Lambda)=\exp[-\tfrac i4\omega_{\mu\nu}\sigma^{\mu\nu}]$. In this basis a boost is block diagonal and gives $u_L\mapsto e^{\boldsymbol\chi\cdot\boldsymbol\sigma/2}u_L$ and $u_R\mapsto e^{-\boldsymbol\chi\cdot\boldsymbol\sigma/2}u_R$.

For boosts, the two exponentials cancel in $u_L^\dagger u_R$; for rotations, the unitary rotation and its inverse cancel. Hence this bilinear is a [Lorentz scalar](../../../special-relativity.md#lorentz-scalar). The [Pauli matrices](../../../algebra.md#pauli-matrices) obey the identity

$$
i\sigma^2(\sigma^i)^*=-\sigma^i i\sigma^2
$$

shows that $i\sigma^2u_L^*$ acquires the right-handed boost matrix and the usual rotation matrix, so it is right-handed.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The identities $S_L^\dagger\bar\sigma^\mu S_L=\Lambda^\mu{}_{\nu}\bar\sigma^\nu$ and $S_L^T\sigma^2S_L=\sigma^2$ show respectively that the kinetic term and both mass bilinears are Lorentz invariant. Infinitesimally, the first identity makes $u_L^\dagger\bar\sigma^\mu u_L$ transform by the vector law stated in the question, while the second makes $u_L^T\sigma^2u_L$ a scalar.

Varying the anticommuting components of $u_L^\dagger$ gives

$$
i\bar\sigma^\mu\partial_\mu u_L-i m\sigma^2u_L^*=0.
$$

The factor two from varying the antisymmetric quadratic form cancels the $1/2$ in the mass term. This is a [Majorana mass term](../../../relativistic-quantum-field.md#majorana-mass-term): under $u_L\mapsto e^{iq\alpha}u_L$ it carries charge $2q$, so a nonzero mass is compatible with an unbroken electric charge only for $q=0$. A charged massive fermion instead needs an independent Weyl field of opposite chirality to form a Dirac mass.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [Dirac field](../../../relativistic-quantum-field.md#dirac-field) Lagrangian is

$$
\mathcal L_D=i\bar\psi\gamma^\mu\partial_\mu\psi-m\bar\psi\psi.
$$

Choose the [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor)

$$
\psi_M=\binom{u_L}{i\sigma^2u_L^*}.
$$

Substitution shows that its two chiral kinetic terms agree after integration by parts and that

$$
-m\bar\psi_M\psi_M
=i m\{u_L^T\sigma^2u_L-u_L^\dagger\sigma^2u_L^*\}.
$$

Thus $\mathcal L_D[\psi_M]$ equals twice the displayed one-Weyl-field Lagrangian, up to a total derivative.

The lower chiral component of the [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) is

$$
i\bar\sigma^\mu\partial_\mu u_L-mu_R=0.
$$

Putting $u_R=i\sigma^2u_L^*$ gives exactly $i\bar\sigma^\mu\partial_\mu u_L-i m\sigma^2u_L^*=0$; the upper component is its [complex conjugate](../../../complex-analysis.md#complex-conjugate).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
