# Paper 307

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_307.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_307.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
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
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)
  - [v](#4/v)
    - [Solution](#4/v/solution)
  - [vi](#4/vi)
    - [Solution](#4/vi/solution)
  - [vii](#4/vii)
    - [Solution](#4/vii/solution)
  - [viii](#4/viii)
    - [Solution](#4/viii/solution)

## 1

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Treating derivatives with respect to the [Grassmann variables](../../../linear-algebra.md#grassmann-variable) as graded derivatives and using $\{\partial_\alpha,\theta^\beta\}=\delta_\alpha{}^\beta$ gives

$$
\{\mathcal D_\alpha,\overline{\mathcal D}_{\dot\alpha}\}
=-2i\sigma^\mu_{\alpha\dot\alpha}\partial_\mu
=2\sigma^\mu_{\alpha\dot\alpha}\mathcal P_\mu,
\qquad \mathcal P_\mu=-i\partial_\mu.
$$

The terms in $\{\mathcal D_\alpha,\mathcal D_\beta\}$ and $\{\overline{\mathcal D}_{\dot\alpha},\overline{\mathcal D}_{\dot\beta}\}$ cancel pairwise, so both vanish.

A [chiral superfield](../../../supersymmetry.md#chiral-superfield) obeys $\overline{\mathcal D}_{\dot\alpha}\Phi=0$, while an [antichiral superfield](../../../supersymmetry.md#antichiral-superfield) obeys $\mathcal D_\alpha\Phi^\dagger=0$. Since $\overline{\mathcal D}_{\dot\alpha}y^\mu=0$ for $y^\mu=x^\mu+i\theta\sigma^\mu\bar\theta$, the general chiral expansion is

$$
\Phi(y,\theta)=\phi(y)+\sqrt2\theta\psi(y)+\theta^2F(y).
$$

In the original coordinates this is

$$
\Phi=\phi+\sqrt2\theta\psi+\theta^2F+i\theta\sigma^\mu\bar\theta\,\partial_\mu\phi
-\frac{i}{\sqrt2}\theta^2\partial_\mu\psi\sigma^\mu\bar\theta
-\frac14\theta^2\bar\theta^2\Box\phi,
$$

with signs following the conventions of the question.

A holomorphic function $W(\Phi)$ is chiral. Its highest component transforms into a spacetime divergence, so the [F-term](../../../supersymmetry.md#f-term) action

$$
S_W=\int d^4x\,d^2\theta\,W(\Phi)+\mathrm{h.c.}
$$

is supersymmetric even though it integrates over only chiral half of [superspace](../../../supersymmetry.md#superspace).

The [non-renormalization theorem](../../../supersymmetry.md#non-renormalization-theorem) says that perturbative loop corrections are full-superspace D-terms and cannot generate a new local superpotential. Holomorphy and spurion symmetries therefore preserve

$$
W_{\rm Wilsonian}=\frac12m\Phi^2+\frac13\lambda\Phi^3.
$$

The Kähler potential is renormalized, however. If its kinetic term is $Z\Phi^\dagger\Phi$, canonical normalization $\Phi_c=Z^{1/2}\Phi$ gives

$$
m_{\rm phys}=\frac mZ,
\qquad
\lambda_{\rm phys}=\frac\lambda{Z^{3/2}},
$$

up to scheme and scale conventions. Thus superpotential parameters are holomorphic invariants while physical masses and couplings still run through [wave-function renormalization](../../../perturbative-quantum-field-theory.md#wave-function-renormalization).

## 2

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Under the Abelian [supergauge transformation](../../../supersymmetry.md#supergauge-transformation) $V\mapsto V+i(\Omega-\Omega^\dagger)$, the real and imaginary components of $\omega$, together with $\psi$ and $F$, shift $C,\chi$ and $M$. They can be chosen to set

$$
C=\chi=M=0,
$$

leaving [Wess-Zumino gauge](../../../supersymmetry.md#wess-zumino-gauge)

$$
V_{\rm WZ}=\theta\sigma^\mu\bar\theta A_\mu
+\theta^2\bar\theta\bar\lambda+\bar\theta^2\theta\lambda
+\frac12\theta^2\bar\theta^2D.
$$

The remaining imaginary scalar gauge parameter acts as the ordinary transformation $A_\mu\mapsto A_\mu+\partial_\mu\alpha$.

The [chiral field-strength superfield](../../../supersymmetry.md#chiral-field-strength-superfield)

$$
W_\alpha=-\frac14\overline{\mathcal D}^{,2}\mathcal D_\alpha V
$$

is chiral and gauge invariant in the Abelian theory. Hence

$$
S=\frac1{4e^2}\int d^4x\,d^2\theta\,W^\alpha W_\alpha+\mathrm{h.c.}
$$

is supersymmetric. Its components are the Maxwell kinetic term, the gaugino kinetic term, and the auxiliary term $D^2/(2e^2)$.

For the component check, vary $F_{\mu\nu}$ using $\delta A_\mu=\epsilon\sigma_\mu\bar\lambda+\lambda\sigma_\mu\bar\epsilon$ and vary the gaugino term using $\delta\lambda=F_{\rho\sigma}\sigma^{\rho\sigma}\epsilon$ and its conjugate. After integration by parts, the terms proportional to $\partial_\mu F^{\mu\nu}$ cancel between the two variations. The remaining terms reduce, by the stated sigma-matrix identity, to a contraction of $\partial_{[\mu}F_{\nu\rho]}$, which vanishes by the [Bianchi identity](../../../fiber-bundle.md#bianchi-identity). Thus $\delta\mathcal L$ is a total divergence and the action is invariant. The auxiliary field would make this supersymmetry close off shell; setting $D=0$ gives the displayed on-shell transformations.

## 3

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [gauge anomaly](../../../relativistic-quantum-field.md#gauge-anomaly) breaks a redundancy needed to remove unphysical states and makes a quantum gauge theory inconsistent unless it cancels. A [chiral anomaly](../../../relativistic-quantum-field.md#chiral-anomaly) is instead the quantum violation of a classical global axial current; the theory remains consistent, but processes such as $\pi^0\to\gamma\gamma$ and instanton-induced charge violation become possible. A ['t Hooft anomaly](../../../relativistic-quantum-field.md#t-hooft-anomaly) is an obstruction to gauging a global symmetry. It is compatible with a consistent theory but is invariant under renormalization-group flow, so any infrared phase must reproduce it through massless fields, spontaneous symmetry breaking, or topological degrees of freedom.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Normalize the [cubic anomaly coefficient](../../../semisimple-lie-algebra.md#cubic-anomaly-coefficient) of the $SU(N)$ fundamental to $+1$. The [two-index antisymmetric representation](../../../semisimple-lie-algebra.md#two-index-antisymmetric-representation) has anomaly coefficient $N-4$, while an antifundamental contributes $-1$. Cancellation of the $SU(N)^3$ [gauge anomaly](../../../relativistic-quantum-field.md#gauge-anomaly) requires

$$
(N-4)-p=0,
\qquad
\boxed{p=N-4}.
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Classically the $p$ identical fields $\psi^i$ have $U(p)=SU(p)\times U(1)_\psi$, and $\lambda$ has an independent $U(1)_\lambda$. One linear combination has an $SU(N)^2U(1)$ anomaly. For the orthogonal combination choose

$$
q_\lambda=p=N-4,
\qquad
q_\psi=-(N-2).
$$

Indeed,

$$
I(\text{antisym})q_\lambda+pI(\overline\square)q_\psi
=(N-2)p-p(N-2)=0.
$$

The continuous quantum global symmetry is therefore

$$
\boxed{SU(p)\times U(1)},
$$

up to discrete identifications. The anomalous orthogonal axial rotation does not survive as a continuous quantum symmetry.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Only the $\psi$ fields transform under flavor $SU(p)$; their gauge-color index gives $N$ copies of its fundamental. With $p=N-4$, the ultraviolet ['t Hooft anomalies](../../../relativistic-quantum-field.md#t-hooft-anomaly) are

$$
\begin{aligned}
SU(p)^3 &: &&N,\\
SU(p)^2U(1)&:&&Nq_\psi=-N(N-2),\\
U(1)^3&:&&\frac{N(N-1)}2p^3+pN[-(N-2)]^3,\\
U(1)\text{-gravity}^2&:&&\frac{N(N-1)}2p+pN[-(N-2)].
\end{aligned}
$$

The last two expressions simplify to

$$
-\frac12p(p+1)N^3,
\qquad
-\frac12p(p+1)N,
$$

respectively.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

The composite $\chi^{ij}$ is in the [two-index symmetric representation](../../../semisimple-lie-algebra.md#two-index-symmetric-representation) of $SU(p)$ and has

$$
q_\chi=2q_\psi+q_\lambda=-N.
$$

For that representation,

$$
A(\mathrm{sym})=p+4=N,
\quad I(\mathrm{sym})=p+2=N-2,
\quad \dim(\mathrm{sym})=\frac{p(p+1)}2.
$$

Its anomalies are consequently

$$
N,qquad -N(N-2),qquad
-\frac12p(p+1)N^3,qquad
-\frac12p(p+1)N,
$$

in the same order as part iii. Every anomaly matches, so confinement to the proposed massless composite is consistent with ['t Hooft anomaly matching](../../../relativistic-quantum-field.md#t-hooft-anomaly-matching).

## 4

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The fermion in a chiral multiplet has [R-charge](../../../supersymmetry.md#r-charge) $R[\Phi]-1$, while the gluino has charge one. Cancellation of the $Sp(N_c)^2U(1)_R$ anomaly gives

$$
I(\mathrm{adj})+2N_fI(\square)(R[\Phi]-1)=0.
$$

Using $I(\mathrm{adj})=2(N_c+1)$ and $I(\square)=1$ yields

$$
\boxed{R[\Phi]=1-\frac{N_c+1}{N_f}
=\frac{N_f-N_c-1}{N_f}}.
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The one-loop coefficient is

$$
b_0=\frac32\,2(N_c+1)-\frac12(2N_f)=3(N_c+1)-N_f.
$$

Thus asymptotic freedom is lost at

$$
\boxed{N_f=3(N_c+1)},
$$

and the theory is infrared free for larger $N_f$.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

In a four-dimensional supersymmetric conformal field theory, a [chiral primary operator in four-dimensional N=1 supersymmetry](../../../supersymmetry.md#chiral-primary-operator-in-four-dimensional-n-1-supersymmetry) obeys $\Delta=3R/2$. The meson has [R-charge](../../../supersymmetry.md#r-charge) $R[M]=2R[\Phi]$, hence

$$
\Delta(M)=3R[\Phi]=3\left(1-\frac{N_c+1}{N_f}\right).
$$

At $N_f=3(N_c+1)$ this gives

$$
\boxed{\Delta(M)=2}.
$$

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

A free scalar has [scaling dimension](../../../string-theory.md#scaling-dimension) one. Setting the meson dimension to one gives

$$
3\left(1-\frac{N_c+1}{N_f}\right)=1,
\qquad
N_f=\frac32(N_c+1).
$$

The expected interacting [supersymmetric conformal window](../../../supersymmetry.md#supersymmetric-conformal-window) is therefore

$$
\boxed{\frac32(N_c+1)<N_f<3(N_c+1)}.
$$

<h3 id="4/v">v</h3>

↑ **Parent:** [4](#4)

<h4 id="4/v/solution">Solution</h4>

↑ **Parent:** [V](#4/v)

The magnetic gauge group is $Sp(\widetilde N_c)$ with $\widetilde N_c=N_f-N_c-2$. Repeating the gauge-anomaly cancellation gives

$$
R[q]=1-\frac{\widetilde N_c+1}{N_f}
=\boxed{\frac{N_c+1}{N_f}}.
$$

<h3 id="4/vi">vi</h3>

↑ **Parent:** [4](#4)

<h4 id="4/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#4/vi)

The magnetic superpotential $W\sim qMq$ must have [R-charge](../../../supersymmetry.md#r-charge) two, so

$$
R[M]=2-2R[q]=2\left(1-\frac{N_c+1}{N_f}\right).
$$

Therefore

$$
\boxed{\Delta(M)=\frac32R[M]
=3\left(1-\frac{N_c+1}{N_f}\right)},
$$

exactly matching the R-charge and dimension of the electric meson $\Phi^i\Phi^j$.

<h3 id="4/vii">vii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/vii/solution">Solution</h4>

↑ **Parent:** [Vii](#4/vii)

For the magnetic theory,

$$
b_0^{\rm mag}=3(\widetilde N_c+1)-N_f
=2N_f-3(N_c+1).
$$

It ceases to be asymptotically free when

$$
\boxed{N_f\le\frac32(N_c+1)}.
$$

This is precisely the lower edge of the electric conformal window. Inside the window both descriptions flow to the same interacting [infrared fixed point](../../../critical-phenomenon.md#infrared-fixed-point); below it the magnetic variables provide a weakly coupled infrared description.

<h3 id="4/viii">viii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/viii/solution">Solution</h4>

↑ **Parent:** [Viii](#4/viii)

The electric quarks give $2N_c$ copies of the $SU(2N_f)$ fundamental, so

$$
\mathcal A_{\rm el}[SU(2N_f)^3]=2N_c.
$$

In the magnetic theory the $2\widetilde N_c$ color components of $q$ transform as flavor antifundamentals and contribute $-2\widetilde N_c$. The singlet $M^{ij}$ is the [two-index antisymmetric representation](../../../semisimple-lie-algebra.md#two-index-antisymmetric-representation) of $SU(2N_f)$, whose [cubic anomaly coefficient](../../../semisimple-lie-algebra.md#cubic-anomaly-coefficient) is $2N_f-4$. Hence

$$
\begin{aligned}
\mathcal A_{\rm mag}[SU(2N_f)^3]
&=-2(N_f-N_c-2)+(2N_f-4)\\
&=\boxed{2N_c}
=\mathcal A_{\rm el}.
\end{aligned}
$$

This is a direct anomaly check of [Seiberg duality](../../../supersymmetry.md#seiberg-duality).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
