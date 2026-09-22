# Paper 307

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_307.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_307.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
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
  - [e](#3/e)
    - [Solution](#3/e/solution)

## 1

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For the stated [two-dimensional N=(2,2) supersymmetry](../../../supersymmetry.md#two-dimensional-n-2-2-supersymmetry) conventions, define the [supersymmetric covariant derivatives](../../../supersymmetry.md#supersymmetric-covariant-derivative)

$$
D_\pm=\frac\partial{\partial\theta^\pm}-i\bar\theta^\pm\partial_\pm,
\qquad
\bar D_\pm=-\frac\partial{\partial\bar\theta^\pm}+i\theta^\pm\partial_\pm.
$$

The terms in which a Grassmann derivative hits the explicit Grassmann coordinate cancel the spacetime-derivative terms, while derivatives involving different signs act on independent coordinates. Therefore

$$
\boxed{\{D_+,Q_\pm\}=\{D_+,\bar Q_\pm\}=0}.
$$

The [twisted chiral superfield](../../../supersymmetry.md#twisted-chiral-superfield) constraints $D_-U=\bar D_+U=0$ are solved by the twisted chiral coordinates

$$
\widetilde y^+=x^+-i\theta^+\bar\theta^+,
\qquad
\widetilde y^-=x^-+i\theta^-\bar\theta^-.
$$

The superfield depends only on $(\widetilde y^\pm;\theta^+,\bar\theta^-)$ and has the finite [Grassmann variable](../../../linear-algebra.md#grassmann-variable) expansion

$$
\boxed{U=u+\theta^+\chi_++\bar\theta^-\widetilde\chi_-+\theta^+\bar\theta^-G},
$$

where every component on the right is evaluated at $\widetilde y$; numerical $\sqrt2$ factors may be absorbed into the component definitions.

For one [chiral superfield](../../../supersymmetry.md#chiral-superfield) $\Phi$ and one twisted chiral superfield $U$, the most general local two-derivative supersymmetric action is

$$
\boxed{
\begin{aligned}
S={}&\int d^2x\,d^4\theta\,K(\Phi,\bar\Phi,U,\bar U)\\
&+\left[\int d^2x\,d\theta^+d\theta^-\,W(\Phi)+\mathrm{h.c.}\right]\\
&+\left[\int d^2x\,d\theta^+d\bar\theta^-\,\widetilde W(U)+\mathrm{h.c.}\right].
\end{aligned}}
$$

Here $K$ is real, $W$ is a holomorphic [superpotential](../../../supersymmetry.md#superpotential), and $\widetilde W$ is a holomorphic [twisted superpotential](../../../supersymmetry.md#twisted-superpotential). A full superspace integral, a chiral [F-term](../../../supersymmetry.md#f-term), and a twisted F-term each vary by a spacetime or Berezin total derivative, so all three are supersymmetric.

Choose the [Vector R-symmetry](../../../supersymmetry.md#vector-r-symmetry) and [Axial R-symmetry](../../../supersymmetry.md#axial-r-symmetry) conventions

$$
U(1)_V:\quad\theta^\pm\mapsto e^{i\alpha}\theta^\pm,
\qquad
U(1)_A:\quad\theta^+\mapsto e^{i\beta}\theta^+,
\quad\theta^-\mapsto e^{-i\beta}\theta^-,
$$

with conjugate coordinates transforming oppositely, and assign compatible charges to $\Phi$ and $U$. The D-term is invariant when $K$ is neutral, up to a generalized Kähler transformation. The chiral measure has vector R-charge $-2$ and axial charge zero, whereas the twisted chiral measure has axial R-charge $-2$ and vector charge zero. Hence classical invariance requires

$$
\boxed{
U(1)_V:\ R_V(W)=2,\ R_V(\widetilde W)=0;
\qquad
U(1)_A:\ R_A(W)=0,\ R_A(\widetilde W)=2,
}
$$

together with neutrality of $K$. Equivalently, $W$ and $\widetilde W$ must be quasi-homogeneous with these charges; absent suitable charge assignments, the corresponding superpotential breaks that R-symmetry.

## 2

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The first-order kinetic term makes $\eta^a$ and $\bar\eta_b$ canonically conjugate [Grassmann variables](../../../linear-algebra.md#grassmann-variable). Canonical quantization gives the [canonical anticommutation relations](../../../quantum-mechanics.md#canonical-anticommutation-relations)

$$
\boxed{\{\widehat\eta^a,\widehat{\bar\eta}_b\}=\delta^a{}_b,
\qquad\{\widehat\eta^a,\widehat\eta^b\}=0,
\qquad\{\widehat{\bar\eta}_a,\widehat{\bar\eta}_b\}=0.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The Hilbert space is the [fermionic Fock space](../../../quantum-mechanics.md#fermionic-fock-space)

$$
\boxed{\mathcal H\cong\Lambda^\bullet\mathbb C^n}.
$$

In a polarization where $\widehat\eta^a$ acts by exterior multiplication and $\widehat{\bar\eta}_a$ by contraction, a general state is

$$
\Psi(\eta)=\sum_{p=0}^n\frac1{p!}\Psi_{a_1\cdots a_p}\eta^{a_1}\cdots\eta^{a_p}.
$$

The [fermion number operator](../../../quantum-mechanics.md#fermion-number-operator) $N=\widehat\eta^a\widehat{\bar\eta}_a$ returns the exterior degree, and therefore

$$
\boxed{(-1)^N\Psi(\eta)=\Psi(-\eta)=\sum_p(-1)^p\Psi_{(p)}(\eta)}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The coherent-state representation of an ordinary fermionic trace identifies the endpoints with a minus sign, producing antiperiodic fields. Inserting [fermion parity](../../../topological-quantum-matter.md#fermion-parity) $(-1)^N$ supplies a second minus sign. The resulting [fermionic path integral](../../../quantum-mechanics.md#fermionic-path-integral) therefore has

$$
\boxed{\eta(1)=\eta(0),\qquad\bar\eta(1)=\bar\eta(0)},
$$

and its time-sliced coherent-state action is precisely $S[\eta,\bar\eta]$. This proves the stated supertrace representation.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Diagonalize $T$ with eigenvalues $\lambda_a$ and use the periodic [Fourier series](../../../fourier-series.md)

$$
\eta^a(t)=\sum_{k\in\mathbb Z}\eta_k^ae^{2\pi ikt},
\qquad
\bar\eta^a(t)=\sum_{k\in\mathbb Z}\bar\eta_k^ae^{-2\pi ikt}.
$$

Each [Berezin integral](../../../quantum-mechanics.md#berezin-integral) contributes its quadratic coefficient, so

$$
Z=\prod_{a=1}^n\prod_{k\in\mathbb Z}(2\pi ik+\lambda_a).
$$

Pairing $k$ with $-k$ and using the infinite product for the hyperbolic sine gives, up to the local regularization factor,

$$
\prod_{k\in\mathbb Z}(2\pi ik+\lambda)
=2\sinh\frac\lambda2
=e^{\lambda/2}(1-e^{-\lambda}).
$$

The product of the prefactors is $e^{\operatorname{tr}T/2}=1$ because $T$ is traceless. Thus

$$
\boxed{Z=\prod_a(1-e^{-\lambda_a})=\det(1-e^{-T})}.
$$

This agrees with the direct identity that the [supertrace](../../../quantum-mechanics.md#supertrace) of an induced linear map on an exterior algebra is its characteristic determinant.

## 3

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Expand $X^a=x^a+\theta\psi^a$, $DX^a=\psi^a-i\theta\dot x^a$, and $g_{ab}(X)=g_{ab}(x)+\theta\psi^c\partial_cg_{ab}$. Performing the [Berezin integral](../../../quantum-mechanics.md#berezin-integral) gives

$$
S=\int dt\left[\frac12g_{ab}\dot x^a\dot x^b
+\frac i2g_{ab}\dot\psi^a\psi^b
+\frac i2(\partial_cg_{ab})\psi^c\dot x^a\psi^b\right].
$$

After a fermionic integration by parts, this is the manifestly covariant expression

$$
\boxed{S=\frac12\int dt\left[g_{ab}\dot x^a\dot x^b-i g_{ab}\psi^a\frac{D\psi^b}{dt}\right]},
\qquad
\frac{D\psi^a}{dt}=\dot\psi^a+\Gamma^a{}_{bc}\dot x^b\psi^c.
$$

Under a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism), $x$ is a point of $M$, $\psi\in T_xM$ is a tangent vector, $D_t\psi$ is its [covariant derivative along a curve](../../../fiber-bundle.md#covariant-derivative-along-a-curve), and every index is contracted with the [Riemannian metric](../../../differential-geometry.md#riemannian-metric); the action is therefore invariant.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Substitution of $\delta x^a=\epsilon\psi^a$ and $\delta\psi^a=-i\epsilon\dot x^a$ into the covariant component action leaves a total time derivative; the connection-dependent terms cancel by metric compatibility and the symmetry of the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection). The boundary term vanishes for the stated decay. The [Noether charge](../../../quantum-field-theory.md#noether-charge) is

$$
\boxed{Q=g_{ab}(x)\psi^a\dot x^b},
$$

up to the overall convention inherited from the supersymmetry parameter. Its graded square gives the Hamiltonian, $\{Q,Q\}=2H$ after canonical quantization.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The quantized fermions obey a [Clifford algebra](../../../algebra.md#clifford-algebra), $\{\widehat\psi^a,\widehat\psi^b\}=g^{ab}$. When $M$ is a [spin manifold](../../../riemannian-geometry.md#spin-manifold), they act on the spinor bundle and

$$
\boxed{\mathcal H=L^2(M,S)},
$$

the Hilbert space of square-integrable [spinor fields](../../../riemannian-geometry.md#spinor-field). The supercharge becomes the [Dirac operator](../../../riemannian-geometry.md#dirac-operator), the Hamiltonian is one half of its square, and because $M$ is even dimensional, $(-1)^F$ is the spinor chirality operator.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The insertion of $(-1)^F$ makes the fermions periodic, while the isometry $f$ twists both fields by its action on $M$ and its differential on the tangent bundle. Thus

$$
\boxed{x(\beta)=f(x(0)),\qquad
\psi(\beta)=df_{x(0)}\psi(0)}.
$$

The path integral with these boundary conditions represents the [equivariant supertrace](../../../quantum-mechanics.md#equivariant-supertrace) $\operatorname{Tr}_{\mathcal H}((-1)^Ff e^{-\beta H})$.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The equivariant supertrace is independent of $\beta$ because positive-energy bosonic and fermionic states pair under the supercharge. Take the [short-time limit](../../../quantum-mechanics.md#short-time-limit-of-a-supersymmetric-path-integral) $\beta\to0$. A finite-action path becomes constant, but the twisted boundary condition then requires $x=f(x)$; its constant saddles are exactly the [fixed-point set](../../../riemannian-geometry.md#fixed-point-set) $M^f$. Supersymmetry cancels the nonzero bosonic and fermionic fluctuations away from their zero modes. Consequently the path integral localizes to a tubular neighborhood of $M^f$, with the remaining Gaussian determinants giving the local fixed-point contribution to the [equivariant index theorem](../../../riemannian-geometry.md#equivariant-index-theorem).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
