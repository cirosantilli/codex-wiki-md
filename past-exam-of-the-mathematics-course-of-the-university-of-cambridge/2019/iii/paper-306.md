# Paper 306

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_306.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_306.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The holomorphic part of the [free-boson worldsheet propagator](../../../string-theory.md#free-boson-worldsheet-propagator) gives

$$
\partial X^\mu(z)\partial X^\nu(w)\sim-\frac{\alpha'}2\frac{\eta^{\mu\nu}}{(z-w)^2}.
$$

Apply [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem) to $T(z)T(w)$. The two double contractions give $D/[2(z-w)^4]$, while the single contractions reconstruct $T$ and its derivative. Thus the [stress-tensor operator-product expansion](../../../string-theory.md#stress-tensor-operator-product-expansion) is

$$
\boxed{
T(z)T(w)\sim\frac{D/2}{(z-w)^4}+\frac{2T(w)}{(z-w)^2}+\frac{\partial T(w)}{z-w}
}
$$

and the $D$ embedding coordinates have [central charge](../../../string-theory.md#central-charge) $\boxed{c=D}$.

The [holomorphic stress-energy tensor](../../../string-theory.md#holomorphic-stress-energy-tensor) generates an infinitesimal conformal transformation through

$$
\delta_vT(z)=\frac1{2\pi i}\oint_zdw\,v(w)T(w)T(z).
$$

Taking the three residues gives

$$
\boxed{\delta_vT=\frac{c}{12}\partial^3v+2(\partial v)T+v\partial T}.
$$

The third derivative is the anomalous term that prevents $T$ from transforming as an ordinary weight-two [Virasoro primary operator](../../../string-theory.md#primary-field).

With [Virasoro algebra](../../../string-theory.md#virasoro-algebra) modes $L_n=(2\pi i)^{-1}\oint dz\,z^{n+1}T(z)$, a second contour calculation gives

$$
\boxed{[L_m,L_n]=(m-n)L_{m+n}+\frac{c}{12}m(m^2-1)\delta_{m+n,0}},
$$

so $A(m)=c(m^3-m)/12=D(m^3-m)/12$. This [Virasoro central extension](../../../string-theory.md#virasoro-central-extension) is the quantum conformal anomaly. In string theory the matter and ghost contributions must cancel; $c_{\rm matter}+c_{\rm ghost}=D-26=0$ gives the [critical dimension of string theory](../../../string-theory.md#critical-dimension-of-string-theory) $D=26$ and makes the [BRST operator](../../../string-theory.md#brst-operator) nilpotent.

## 2

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Split the [string embedding map](../../../string-theory.md#string-embedding-map) into its constant [worldsheet zero mode](../../../string-theory.md#worldsheet-zero-mode) and orthogonal fluctuations, $X^\mu=x^\mu+X'^\mu$. The kinetic operator has no inverse on the constant mode, while its inverse on $X'$ is the [worldsheet Green function](../../../string-theory.md#worldsheet-green-function) $G$. Completing the square in the [Gaussian functional integral](../../../quantum-field-theory.md#gaussian-functional-integral) gives

$$
\int\mathcal DX'\,e^{-S[X']-\int J\cdot X'}
\propto\exp\left(\frac12\int_{\Sigma\times\Sigma}d^2z\,d^2w\,J(z)G(z,w)J(w)\right).
$$

The remaining ordinary integral is

$$
\int d^Dx\,e^{-x^\mu\int_\Sigma d^2zJ_\mu(z)},
$$

which proves (1), up to a source-independent [functional determinant](../../../quantum-field-theory.md#functional-determinant).

To insert $n$ [tachyon vertex operators](../../../string-theory.md#tachyon-vertex-operator), choose

$$
J_\mu(z,\bar z)=-i\sum_{j=1}^nk_{j\mu}\delta^{(2)}(z-z_j).
$$

The zero-mode integral produces target-space momentum conservation,

$$
(2\pi)^D\delta^{(D)}\left(\sum_jk_j\right).
$$

In the nonzero-mode integral, discard the coincident self-contractions by [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering). With $G(z,w)=-(\alpha'/2)\log|z-w|^2$, the remaining pairwise contractions produce the [Koba-Nielsen factor](../../../string-theory.md#koba-nielsen-factor), so

$$
\boxed{
\left\langle\prod_{j=1}^ne^{ik_j\cdot X(z_j,\bar z_j)}\right\rangle
\propto(2\pi)^D\delta^{(D)}\left(\sum_jk_j\right)
\prod_{i<j}|z_i-z_j|^{\alpha'k_i\cdot k_j}
}.
$$

For three closed-string tachyons on the sphere, $k_i^2=4/\alpha'$ and $\sum_i k_i=0$, hence $\alpha'k_i\cdot k_j=-2$ for $i\ne j$. The matter correlator is therefore $|z_{12}z_{13}z_{23}|^{-2}$. Gauge fixing the sphere's [Möbius transformation](../../../group-theory.md#mobius-transformation) group fixes three insertion points and supplies the [bc ghost system](../../../string-theory.md#bc-system) correlator $|z_{12}z_{13}z_{23}|^2$, exactly cancelling this position dependence. Thus

$$
\boxed{\mathcal A_3=C_{S^2}g_c^3(2\pi)^D\delta^{(D)}(k_1+k_2+k_3)}.
$$

Here each vertex contributes one closed-string coupling $g_c$, $C_{S^2}$ contains the sphere vacuum normalization and conventions, the [worldsheet zero mode](../../../string-theory.md#worldsheet-zero-mode) gives the momentum delta function, the nonzero modes give the [Koba-Nielsen factor](../../../string-theory.md#koba-nielsen-factor), and the ghost determinant divides by the conformal Killing group. Since $C_{S^2}\propto g_s^{-2}$ and $g_c\propto g_s$, the net [string genus expansion](../../../string-theory.md#string-genus-expansion) dependence is $g_s$.

## 3

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [BRST operator](../../../string-theory.md#brst-operator) $Q_B$ is Grassmann odd and represents the gauge symmetry on the gauge-fixed state space. Requiring two successive BRST transformations to vanish means

$$
Q_B^2=\frac12\{Q_B,Q_B\}=0.
$$

This nilpotence makes physical states a [BRST cohomology](../../../relativistic-quantum-field.md#brst-cohomology). If $[Q_B,S_0]=0$ and $\Psi$ is the [gauge-fixing fermion](../../../relativistic-quantum-field.md#gauge-fixing-fermion), the graded Jacobi identity gives

$$
[Q_B,S]=[Q_B,S_0]+[Q_B,\{Q_B,\Psi\}]
=\frac12[\{Q_B,Q_B\},\Psi]=0,
$$

so $S=S_0+\{Q_B,\Psi\}$ is BRST invariant.

A holomorphic field of [conformal weight](../../../string-theory.md#conformal-weight) $h$ has the Laurent expansion

$$
\phi(z)=\sum_{n\in\mathbb Z}\phi_nz^{-n-h}.
$$

Under the [state–operator correspondence](../../../string-theory.md#state-operator-correspondence), $\phi(z)|0\rangle$ must be regular at the origin. Terms with $n>-h$ have negative powers, so

$$
\boxed{\phi_n|0\rangle=0\quad(n>-h)}.
$$

For the anticommuting [bc system](../../../string-theory.md#bc-system),

$$
b(z)=\sum_nb_nz^{-n-2},\qquad c(z)=\sum_nc_nz^{-n+1},
\qquad\{b_m,c_n\}=\delta_{m+n,0}.
$$

Separating creation and annihilation modes and summing the geometric series for $|z|>|w|$ gives the [bc ghost operator-product expansion](../../../string-theory.md#bc-ghost-operator-product-expansion)

$$
\boxed{b(z)c(w)\sim\frac1{z-w}}.
$$

The [BRST current](../../../string-theory.md#brst-current) built from the matter and ghost stress tensors has an operator-product expansion with $c$ whose residue gives

$$
\boxed{\{Q_B,c(z)\}=c(z)\partial c(z)}.
$$

For a matter [Virasoro primary operator](../../../string-theory.md#primary-field) $\Phi(z,\bar z)$ of weights $(1,1)$, the two standard [string vertex operators](../../../string-theory.md#string-vertex-operator) are

$$
\boxed{U(z,\bar z)=c(z)\bar c(\bar z)\Phi(z,\bar z)},
\qquad
\boxed{V=\int_\Sigma d^2z\,\Phi(z,\bar z)}.
$$

The first is the local, unintegrated vertex. Using $Q_Bc=c\partial c$, $Q_B\bar c=\bar c\bar\partial\bar c$, and the weight-$(1,1)$ transformation of $\Phi$, the terms cancel pairwise and $Q_BU=0$. For the integrated vertex,

$$
\{Q_B,\Phi\}=\partial(c\Phi)+\bar\partial(\bar c\Phi),
$$

so $\{Q_B,V\}=0$ on a closed worldsheet because the variation is a total derivative. Both vertices therefore represent the same [BRST cohomology](../../../relativistic-quantum-field.md#brst-cohomology) class.

## 4

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Insert the given [closed-string mode expansion](../../../string-theory.md#closed-string-mode-expansion) into the stress tensor and compare $T(z)=\sum_nL_nz^{-n-2}$. [Normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering) gives

$$
\boxed{L_n=\frac12\sum_{m\in\mathbb Z}:\alpha_{n-m}\cdot\alpha_m:}.
$$

The inverse of the worldsheet Laplacian gives the free-field operator-product expansion

$$
\boxed{X^\mu(z,\bar z)X^\nu(w,\bar w)\sim-\frac{\alpha'}2\eta^{\mu\nu}\log|z-w|^2}.
$$

Hence

$$
\partial X^\mu(z)\partial X^\nu(w)\sim-\frac{\alpha'}2\frac{\eta^{\mu\nu}}{(z-w)^2}.
$$

Extracting the Laurent modes by contour integration yields the [string oscillator](../../../string-theory.md#string-oscillator) algebra

$$
\boxed{[\alpha_m^\mu,\alpha_n^\nu]=m\eta^{\mu\nu}\delta_{m+n,0}}.
$$

The vanishing of the worldsheet stress tensor becomes the [Virasoro constraints](../../../string-theory.md#virasoro-constraint)

$$
L_n|\text{phys}\rangle=\bar L_n|\text{phys}\rangle=0\quad(n>0),
\qquad (L_0-a)|\text{phys}\rangle=(\bar L_0-a)|\text{phys}\rangle=0.
$$

Since $L_0=\alpha'k^2/4+N$ and the bosonic-string normal-ordering constant is $a=1$, these zero-mode constraints are the target-space [string mass-shell condition](../../../string-theory.md#string-mass-shell-condition)

$$
M^2=\frac4{\alpha'}(N-1)=\frac4{\alpha'}(\bar N-1),
\qquad N=\bar N.
$$

Therefore

$$
\boxed{M_T^2=-\frac4{\alpha'},\qquad M_g^2=0.}
$$

The positive-mode constraints further require

$$
\boxed{k^\mu\epsilon_{\mu\nu}=0,\qquad k^\nu\epsilon_{\mu\nu}=0},
$$

and [null string states](../../../string-theory.md#null-string-state) identify polarizations that differ by momentum-longitudinal terms. The symmetric trace-free, antisymmetric, and trace sectors of $\epsilon_{\mu\nu}$ describe the graviton, [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field), and [dilaton](../../../string-theory.md#dilaton), respectively.

Finally, the [state–operator correspondence](../../../string-theory.md#state-operator-correspondence) maps $\alpha_{-1}^\mu\bar\alpha_{-1}^\nu|k\rangle$ to

$$
\partial X^\mu\bar\partial X^\nu e^{ik\cdot X}.
$$

Adding its integrated [massless closed-string vertex operator](../../../string-theory.md#massless-closed-string-vertex-operator) to the [string nonlinear sigma model](../../../string-theory.md#string-nonlinear-sigma-model) changes the background coupling by

$$
\delta S\propto\int d^2z\,\delta G_{\mu\nu}(X)\partial X^\mu\bar\partial X^\nu.
$$

Thus a Fourier mode $\delta G_{\mu\nu}(X)=\epsilon_{(\mu\nu)}e^{ik\cdot X}$ is precisely a linearized deformation of the target-space metric. Its transversality, mass-shell condition, and polarization gauge redundancy are the worldsheet statements that the deformation is marginal and is defined up to a linearized spacetime diffeomorphism.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
