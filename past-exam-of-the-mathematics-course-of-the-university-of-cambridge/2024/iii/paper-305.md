# Paper 305

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_305.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_305.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
  - [v](#2/v)
    - [Solution](#2/v/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
  - [v](#3/v)
    - [Solution](#3/v/solution)
  - [vi](#3/vi)
    - [Solution](#3/vi/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 305](paper-305.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Write $m=|m|e^{i\theta}$. [Parity](../../../quantum-mechanics.md#parity) reverses the spatial coordinates and must exchange the two chiral [Weyl spinors](../../../relativistic-quantum-field.md#weyl-spinor). One convenient choice is

$$
\boxed{
P:\quad
\psi_L(t,\mathbf x)\mapsto e^{-i\theta}\psi_R(t,-\mathbf x),
\qquad
\psi_R(t,\mathbf x)\mapsto e^{i\theta}\psi_L(t,-\mathbf x)}.
$$

The identities $\sigma^0=\bar\sigma^0$ and $\sigma^i=-\bar\sigma^i$ exchange the two kinetic terms after $\mathbf x\mapsto-\mathbf x$. The mass bilinear $m\bar\psi_R\psi_L$ maps to its [complex conjugate](../../../complex-analysis.md#complex-conjugate) $m^*\bar\psi_L\psi_R$, so the two mass terms are exchanged and the action is invariant. More generally, independent unit phases $a,b$ may multiply the two transformations provided $b^*a=m^*/m$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

[Charge conjugation](../../../quantum-field-theory.md#charge-conjugation) reverses the gauge charge, so

$$
\boxed{A_\mu\mapsto-A_\mu}.
$$

Using the antisymmetric spinor metric $\epsilon=i\sigma^2$, a compatible action on the two Weyl fields is

$$
\boxed{
\psi_L\mapsto i\sigma^2\psi_R^*,
\qquad
\psi_R\mapsto-i\sigma^2\psi_L^*}.
$$

Complex conjugation reverses the sign of $i$ and of the gauge representation, while $A_\mu\mapsto-A_\mu$ restores the original [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative). The identities $\sigma^2(\sigma^\mu)^*\sigma^2=\bar\sigma^\mu$ and $\sigma^2(\bar\sigma^\mu)^*\sigma^2=\sigma^\mu$ then exchange the two equations of motion. Unit phases can be inserted in the two spinor transformations without changing the conclusion, subject to the mass-term relation.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Take the most general parity action compatible with the kinetic and mass terms as $\psi_L\mapsto a\psi_R$, $\psi_R\mapsto b\psi_L$, where $|a|=|b|=1$ and $b^*a=m^*/m$, and let $\phi\mapsto c_P\phi$ with $|c_P|=1$. The two holomorphic [Yukawa interactions](../../../standard-model.md#yukawa-interaction) are exchanged when

$$
\lambda_2=\lambda_1c_Pa^2,
\qquad
\lambda_1=\lambda_2c_Pb^2,
$$

up to the common sign convention for antisymmetric spinor contraction. The freely chosen intrinsic phases satisfy these equations exactly when

$$
\boxed{|\lambda_1|=|\lambda_2|}.
$$

For charge conjugation, write $\psi_L\mapsto a_Ci\sigma^2\psi_R^*$, $\psi_R\mapsto b_Ci\sigma^2\psi_L^*$ and $\phi\mapsto c_C\phi^*$. It exchanges each Yukawa term with the Hermitian conjugate of the opposite-chirality term. The coefficient equations have the form $\lambda_2^*=\lambda_1c_Ca_C^2$ and $\lambda_1^*=\lambda_2c_Cb_C^2$; the available intrinsic phases again solve them exactly when

$$
\boxed{|\lambda_1|=|\lambda_2|}.
$$

For conventional choices of all intrinsic phases these statements reduce to phase-sensitive relations such as $\lambda_2=\lambda_1$ under parity and $\lambda_2=\lambda_1^*$ under charge conjugation; those phases are conventions, while equality of magnitudes is invariant.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

In four spacetime dimensions a [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor) has [mass dimension](../../../perturbative-quantum-field-theory.md#mass-dimension) $3/2$, so each chiral current $J_L^\mu=\bar\psi_L\bar\sigma^\mu\psi_L$ or $J_R^\mu=\bar\psi_R\sigma^\mu\psi_R$ has dimension three. Since the interaction is $(gJ_L+g'J_R)^2$, dimensional homogeneity of the Lagrangian gives

$$
\boxed{[g]=[g']=-1}.
$$

Equivalently, the expanded [four-fermion interaction](../../../quantum-field-theory.md#four-fermion-interaction) has coefficients $g^2,gg',g'^2$ of mass dimension minus two.

Parity exchanges $J_L$ and $J_R$. The square is invariant precisely when the two same-chirality coefficients agree, $g^2=g'^2$, while the mixed coefficient is already symmetric. Therefore

$$
\boxed{g'=g\quad\text{or}\quad g'=-g}.
$$

## 2

↑ **Parent:** [Paper 305](paper-305.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

[Asymptotic freedom](../../../perturbative-quantum-field-theory.md#asymptotic-freedom) means that the gauge [running coupling](../../../perturbative-quantum-field-theory.md#running-coupling) tends to zero as the renormalization scale tends to infinity. In the stated convention this occurs when $b_0>0$, namely

$$
\boxed{11N_c-N_f-\frac12N_s>0}.
$$

The high-energy theory then approaches the [Gaussian fixed point](../../../critical-phenomenon.md#gaussian-fixed-point) and perturbation theory becomes increasingly accurate.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [strong-coupling scale](../../../perturbative-quantum-field-theory.md#strong-coupling-scale) $\Lambda$ is defined as the scale at which the one-loop inverse coupling vanishes. Setting $g^{-2}(\Lambda)=0$ gives

$$
\boxed{\Lambda=\Lambda_{UV}
\exp\!\left[-\frac{3(4\pi)^2}{2b_0g_0^2}\right]}.
$$

Equivalently, in terms of the coupling measured at any scale $\mu$,

$$
\boxed{\Lambda=\mu
\exp\!\left[-\frac{3(4\pi)^2}{2b_0g^2(\mu)}\right]}.
$$

This [dimensional transmutation](../../../perturbative-quantum-field-theory.md#dimensional-transmutation) defines $\Lambda_{\rm QCD}$ for [Quantum chromodynamics](../../../standard-model.md#quantum-chromodynamics).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

For $SU(3)_c$, one generation contains two color triplets in the quark doublet and the two right-handed color triplets, so $N_f=4N_g$ and there is no colored scalar. Thus

$$
b_s=33-4N_g>0,
$$

which permits at most

$$
\boxed{N_g=8}.
$$

For $SU(2)_L$, each generation contains three colored copies of the quark doublet and one lepton doublet, again giving $N_f=4N_g$. The one complex [Higgs doublet](../../../standard-model.md#higgs-field) gives $N_s=1$, so

$$
b_w=22-4N_g-\frac12>0.
$$

Hence the maximum is

$$
\boxed{N_g=5}.
$$

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Let $K=3(4\pi)^2$ and $L=\log(M^2/\mu^2)$. Running from $M$ down to $\mu$ gives

$$
\frac1{g_i^2(\mu)}=\frac1{g_i^2(M)}-\frac{b_i}{K}L.
$$

The assumed unified boundary condition implies

$$
\frac1{g_s^2(M)}=\frac1{g_w^2(M)}=\frac3{5g_Y^2(M)}.
$$

Subtracting the weak equation from the strong and normalized-hypercharge equations therefore gives

$$
\frac1{g_s^2(\mu)}-\frac1{g_w^2(\mu)}
=-\frac{b_s-b_w}{K}L,
$$



$$
\frac3{5g_Y^2(\mu)}-\frac1{g_w^2(\mu)}
=-\frac{\frac35b_Y-b_w}{K}L.
$$

Eliminating $L$ proves

$$
\boxed{
\frac1{g_s^2(\mu)}-\frac1{g_w^2(\mu)}
=\frac{b_s-b_w}{\frac35b_Y-b_w}
\left(\frac3{5g_Y^2(\mu)}-\frac1{g_w^2(\mu)}\right)}.
$$

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

The block-diagonal subgroup

$$
S(U(3)\times U(2))
=\{\operatorname{diag}(U_3,U_2):\det U_3\det U_2=1\}
\subset SU(5)
$$

is locally $SU(3)\times SU(2)\times U(1)$, with only a finite central quotient distinguishing the global groups. The hypercharge direction in the fundamental representation is

$$
Y=\operatorname{diag}\!\left(-\frac13,-\frac13,-\frac13,
\frac12,\frac12\right),
$$

which is traceless and commutes with the $SU(3)$ and $SU(2)$ blocks.

The canonically normalized $SU(5)$ generator must satisfy $\operatorname{Tr}(T_Y^2)=1/2$. Since $\operatorname{Tr}(Y^2)=5/6$,

$$
T_Y=\sqrt{\frac35}\,Y.
$$

The unified [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative) contains $g_5T_YB_\mu$, whereas the Standard Model convention contains $g_YYB_\mu$. Hence $g_Y=\sqrt{3/5}\,g_5$. The non-Abelian generators already have the canonical normalization, so [gauge coupling unification](../../../perturbative-quantum-field-theory.md#gauge-coupling-unification) in the [SU(5) grand unified theory](../../../perturbative-quantum-field-theory.md#su-5-grand-unified-theory) predicts

$$
\boxed{g_s^2=g_w^2=g_5^2=\frac53g_Y^2}.
$$

## 3

↑ **Parent:** [Paper 305](paper-305.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [gauge anomaly](../../../relativistic-quantum-field.md#gauge-anomaly) breaks a redundancy required to remove unphysical polarizations. It violates the Ward identities and makes the quantum gauge theory inconsistent, so all gauge anomalies must cancel. A [chiral anomaly](../../../relativistic-quantum-field.md#chiral-anomaly), or [Adler-Bell-Jackiw anomaly](../../../relativistic-quantum-field.md#chiral-anomaly), instead breaks a classically conserved global axial symmetry; it is physically allowed and explains effects such as anomalous pseudoscalar decays and instanton-induced charge violation. A ['t Hooft anomaly](../../../relativistic-quantum-field.md#t-hooft-anomaly) is an obstruction to gauging a global symmetry. It is invariant under [renormalization-group flow](../../../critical-phenomenon.md#renormalization-group-flow), so ['t Hooft anomaly matching](../../../relativistic-quantum-field.md#t-hooft-anomaly-matching) constrains the infrared theory to reproduce it through massless fields, symmetry breaking, or a topological sector.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Count every right-handed field as a left-handed conjugate, which reverses its $U(1)$ charge and conjugates its non-Abelian representation. The nontrivial local anomaly-cancellation conditions are

$$
[SU(3)]^2U(1):\qquad \boxed{2q-u-d=0},
$$



$$
[SU(2)]^2U(1):\qquad \boxed{3q+l=0},
$$



$$
[U(1)]^3:\qquad
\boxed{6q^3+2l^3-3u^3-3d^3-x^3=0}.
$$

The pure $SU(3)^3$ anomaly cancels because the two triplets in $Q_L$ balance the conjugates of $u_R$ and $d_R$. There is no perturbative $SU(2)^3$ anomaly, and the [Witten SU(2) anomaly](../../../relativistic-quantum-field.md#witten-su-2-anomaly) also vanishes because the three colored quark doublets plus one lepton doublet make four. The [mixed gauge-gravitational anomaly](../../../relativistic-quantum-field.md#mixed-gauge-gravitational-anomaly) is excluded at this stage as requested.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The $[SU(3)]^2U(1)$ condition gives $u+d=2q$, which is even because all hypercharges are [integers](../../../number-theory.md#integer). The sum $u+d$ and difference $u-d$ have the same parity, so $u-d$ is even. Therefore

$$
\boxed{u-d=2y\quad\text{for some }y\in\mathbb Z}.
$$

Solving the sum and difference equations gives

$$
\boxed{u=q+y,\qquad d=q-y}.
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The $[SU(2)]^2U(1)$ condition gives $l=-3q$. Substituting this and $u=q+y$, $d=q-y$ into the cubic anomaly gives

$$
0=6q^3+2(-3q)^3-3(q+y)^3-3(q-y)^3-x^3.
$$

Using $(q+y)^3+(q-y)^3=2q^3+6qy^2$ and multiplying by minus one yields

$$
\boxed{54q^3+18y^2q+x^3=0}.
$$

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

If $q\ne0$, divide the cubic equation by $q^3$ and define the [rational numbers](../../../number-theory.md#rational-number)

$$
\widetilde y=\frac yq,
\qquad
\widetilde x=\frac xq.
$$

Then every integer anomaly-free assignment supplies a rational solution of

$$
\boxed{54+18\widetilde y^{,2}+\widetilde x^{,3}=0,
\qquad \widetilde x,\widetilde y\in\mathbb Q}.
$$

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

Use the stated rational change of variables

$$
\widetilde x=-\frac6{v+w},
\qquad
\widetilde y=\frac{3(v-w)}{v+w}.
$$

Direct substitution turns the anomaly equation into

$$
\frac{216(v^3+w^3-1)}{(v+w)^3}=0,
\qquad\text{so}\qquad v^3+w^3=1.
$$

Writing $v=a/c$ and $w=b/c$ in lowest common denominator gives the integer equation $a^3+b^3=c^3$. The supplied special case of Fermat's Last Theorem says that one of $a,b$ must vanish. Thus $(v,w)=(1,0)$ or $(0,1)$, which gives

$$
\widetilde x=-6,
\qquad
\widetilde y=\pm3.
$$

The two signs merely exchange the names of the up- and down-type singlets. Choosing $q=1$ and the conventional sign $y=3$ gives the unique assignment up to overall scaling and that exchange:

$$
\boxed{l=-3,\qquad u=4,\qquad d=-2,\qquad x=-6}.
$$

These are six times the conventional Standard Model [hypercharges](../../../standard-model.md#hypercharge).

<h3 id="3/vi">vi</h3>

↑ **Parent:** [3](#3)

<h4 id="3/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#3/vi)

The coefficient of the [mixed gauge-gravitational anomaly](../../../relativistic-quantum-field.md#mixed-gauge-gravitational-anomaly) is the sum of all left-handed $U(1)$ charges, with right-handed fields counted as conjugates:

$$
\mathcal A_{\mathrm{grav}^2U(1)}=6q+2l-3u-3d-x.
$$

For the solution above,

$$
6+2(-3)-3(4)-3(-2)-(-6)=0.
$$

More invariantly, $l=-3q$, $u+d=2q$, and $x=-6q$ make the expression vanish identically. Thus the unique cubic-anomaly solution automatically cancels the mixed gauge-gravitational anomaly.

## 4

↑ **Parent:** [Paper 305](paper-305.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

In the convention $(SU(3)_c,SU(2)_L)_Y$, one [Standard Model fermion](../../../standard-model.md#standard-model-fermion) generation including a [right-handed neutrino](../../../standard-model.md#right-handed-neutrino) is

$$
Q_L:(\mathbf3,\mathbf2)_{1/6},\quad
u_R:(\mathbf3,\mathbf1)_{2/3},\quad
d_R:(\mathbf3,\mathbf1)_{-1/3},
$$



$$
L_L:(\mathbf1,\mathbf2)_{-1/2},\quad
e_R:(\mathbf1,\mathbf1)_{-1},\quad
\nu_R:(\mathbf1,\mathbf1)_0.
$$

A bare [Dirac mass term](../../../relativistic-quantum-field.md#dirac-mass-term) pairs left- and right-handed fields in the same gauge representation, but every charged left-handed Standard Model fermion is an $SU(2)_L$ doublet while its right-handed partner is a singlet. The [Higgs field](../../../standard-model.md#higgs-field) $H:(\mathbf1,\mathbf2)_{1/2}$ and $\widetilde H=i\sigma^2H^*:(\mathbf1,\mathbf2)_{-1/2}$ permit the gauge-invariant [Yukawa interactions](../../../standard-model.md#yukawa-interaction)

$$
y_d\bar Q_LHd_R+y_u\bar Q_L\widetilde Hu_R
+y_e\bar L_LHe_R+y_\nu\bar L_L\widetilde H\nu_R+\text{h.c.}
$$

The neutral Higgs vacuum expectation value turns them into masses after [electroweak symmetry breaking](../../../standard-model.md#electroweak-symmetry-breaking).

Because $\nu_R$ is a gauge singlet, it may also have a large [Majorana mass term](../../../relativistic-quantum-field.md#majorana-mass-term) $M$. Together with its Dirac mass $m_D$, the [seesaw mechanism](../../../standard-model.md#seesaw-mechanism) gives a light neutrino mass $m_\nu\simeq m_D^2/M$. If no right-handed neutrino is retained, the same low-energy physics is encoded by the dimension-five [Weinberg operator](../../../standard-model.md#weinberg-operator) $(L_LH)(L_LH)/\Lambda$.

Now let $\phi$ be an [electroweak scalar triplet](../../../standard-model.md#electroweak-scalar-triplet) with $Y=1$. Its $T^3$ weights are $1,0,-1$, and electric charge is $Q=T^3+Y$, so its components have charges

$$
\boxed{\phi^{++}:Q=2,\qquad\phi^+:Q=1,\qquad\phi^0:Q=0}.
$$

In the given matrix convention,

$$
\phi^{++}=\frac{\phi_1-i\phi_2}{2},
\qquad
\phi^+=\frac{\phi_3}{2},
\qquad
\boxed{\phi^0=\frac{\phi_1+i\phi_2}{2}}.
$$

Thus the electromagnetic-neutral direction satisfies $\phi_3=0$ and $\phi_1-i\phi_2=0$.

The gauge-invariant [type-II seesaw mechanism](../../../standard-model.md#type-ii-seesaw-mechanism) Yukawa interaction is

$$
\boxed{\mathcal L_Y=-\frac12y_\phi
L_L^TC\,i\sigma^2\phi L_L+\text{h.c.}}.
$$

The two lepton doublets have total hypercharge $-1$, which is cancelled by $Y(\phi)=1$, and the displayed $SU(2)$ contraction is a singlet. Expanding it contains

$$
-\frac{y_\phi}{4}(\phi_1+i\phi_2)\nu_L^TC\nu_L+\cdots.
$$

**Therefore a neutral condensate $\langle\phi^0\rangle\ne0$ preserves electromagnetism and generates a left-handed-neutrino [Majorana mass term](../../../relativistic-quantum-field.md#majorana-mass-term) proportional to $y_\phi\langle\phi^0\rangle$.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
