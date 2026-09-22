# Paper 304

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_304.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_304.pdf)

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
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [i](#4/d/i)
      - [Solution](#4/d/i/solution)
    - [ii](#4/d/ii)
      - [Solution](#4/d/ii/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a [scalar field](../../../quantum-field-theory.md#scalar-field) with classical [action](../../../classical-mechanics.md#action) $S[\phi]$, the Euclidean source convention used throughout this question gives

$$
Z[J]=\int\mathcal D\phi\,
\exp\left[-\frac1\hbar\left(S[\phi]+\int d^dx\,J(x)\phi(x)\right)\right].
$$

The [generating functional](../../../perturbative-quantum-field-theory.md#generating-functional) produces [correlation functions](../../../critical-phenomenon.md#correlation-function) through [functional derivatives](../../../calculus-of-variations.md#functional-derivative). For example,

$$
\boxed{\langle\phi(x)\phi(y)\rangle
=\left.\frac{\hbar^2}{Z[0]}
\frac{\delta^2Z[J]}{\delta J(x)\delta J(y)}\right|_{J=0}.}
$$

More generally, each derivative brings down $-\phi/\hbar$, so an $n$-point function carries $(-\hbar)^n/Z[0]$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The classical [action](../../../classical-mechanics.md#action) $S[\phi]$ supplies the vertices and quadratic [quantum field theory propagator](../../../quantum-field-theory.md#propagator) in the [path integral](../../../quantum-field-theory.md#path-integral). The [connected generating functional](../../../perturbative-quantum-field-theory.md#connected-generating-functional) is

$$
W[J]=-\hbar\log Z[J],
$$

and its first derivative is the source-dependent mean field

$$
\Phi(x)=\frac{\delta W}{\delta J(x)}=\langle\phi(x)\rangle_J.
$$

The [quantum effective action](../../../perturbative-quantum-field-theory.md#effective-action) is the [Legendre transform](../../../convex-optimization.md#convex-conjugate)

$$
\boxed{\Gamma[\Phi]=W[J]-\int d^dx\,J(x)\Phi(x),
\qquad \frac{\delta\Gamma}{\delta\Phi(x)}=-J(x),}
$$

where $J$ is eliminated in favor of $\Phi$. At vanishing source, stationary points of $\Gamma$ are the quantum equations of motion. This $W[J]$ is the connected, or Schwinger, functional; a [Wilsonian effective action](../../../perturbative-quantum-field-theory.md#wilsonian-effective-action) instead integrates out modes above a momentum scale.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The perturbative expansion of $Z[J]$ contains arbitrary [Feynman diagrams](../../../perturbative-quantum-field-theory.md#feynman-diagram), including disconnected products. The [linked-cluster theorem](../../../perturbative-quantum-field-theory.md#linked-cluster-theorem) gives

$$
Z[J]=Z[0]\exp\left(\sum_{C\ \text{connected}}C[J]\right),
$$

because the factorials from repeated connected components reproduce the exponential series. Therefore $W[J]=-\hbar\log Z[J]$ is the sum of [connected Feynman diagrams](../../../perturbative-quantum-field-theory.md#connected-feynman-diagram).

The Legendre transform removes diagrams that disconnect upon cutting one internal line. Equivalently, every connected diagram is a tree whose vertices are exact one-particle-irreducible vertices and whose edges are exact propagators. Thus

$$
\boxed{\Gamma[\Phi]=S[\Phi]+\text{the sum of loop-level one-particle-irreducible diagrams},}
$$

and its functional derivatives are the [one-particle-irreducible correlation functions](../../../perturbative-quantum-field-theory.md#one-particle-irreducible-correlation-function). Algebraically, differentiating the Legendre relations gives

$$
\int d^dz\,
\frac{\delta^2\Gamma}{\delta\Phi(x)\delta\Phi(z)}
\frac{\delta^2W}{\delta J(z)\delta J(y)}
=-\delta^{(d)}(x-y),
$$

so an exact [quantum field theory propagator](../../../quantum-field-theory.md#propagator) joining two proper vertices is precisely the inverse [Hessian matrix](../../../calculus.md#hessian-matrix) needed to reconstruct connected diagrams.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Change variables in the defining integral from the fluctuation to the total field, $\varphi=\phi_0+\eta$. Then

$$
\begin{aligned}
e^{-W(J;\phi_0)/\hbar}
&=\int d\varphi\,
e^{-[S(\varphi)+J(\varphi-\phi_0)]/\hbar}\\
&=e^{J\phi_0/\hbar}e^{-W(J;0)/\hbar},
\end{aligned}
$$

and hence

$$
W(J;\phi_0)=W(J;0)-J\phi_0.
$$

It follows nonperturbatively that

$$
\chi=\partial_JW(J;\phi_0)
=\partial_JW(J;0)-\phi_0.
$$

Thus the same source $J_\chi$ corresponds at zero background to the mean field $\Phi=\chi+\phi_0$. Using the source-sign-compatible Legendre transform $\Gamma(\chi;\phi_0)=W(J_\chi;\phi_0)-J_\chi\chi$,

$$
\Gamma(\chi;\phi_0)
=W(J_\chi;0)-J_\chi(\chi+\phi_0)
=\Gamma(\chi+\phi_0;0).
$$

Renaming $\chi$ as $\eta$ gives the requested identity

$$
\boxed{\Gamma(\eta;\phi_0)=\Gamma(\phi_0+\eta;0).}
$$

## 2

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

Split the field into disjoint ranges of [Fourier modes](../../../fourier-analysis.md#fourier-mode),

$$
\phi_{\rm tot}=\phi+\phi^+,
\qquad
\widetilde\phi(p)=0\ (p^2>\Lambda^2),
\qquad
\widetilde{\phi^+}(p)=0\ \text{unless }\Lambda^2<p^2\leq\Lambda_0^2.
$$

The [Wilsonian effective action](../../../perturbative-quantum-field-theory.md#wilsonian-effective-action) is defined by

$$
e^{-S_\Lambda^{\rm eff}[\phi]}
=\int_\Lambda^{\Lambda_0}\mathcal D\phi^+\,
e^{-S_{\Lambda_0}[\phi+\phi^+]}.
$$

Writing $\Delta S[\phi,\phi^+]=S_{\Lambda_0}[\phi+\phi^+]-S_{\Lambda_0}[\phi]$ immediately gives

$$
\boxed{S_\Lambda^{\rm eff}[\phi]=S_{\Lambda_0}[\phi]
-\log\int_\Lambda^{\Lambda_0}\mathcal D\phi^+e^{-\Delta S[\phi,\phi^+]}.}
$$

Quadratic cross terms vanish because the momentum supports do not overlap. For $h_0\ne0$,

$$
\begin{aligned}
\Delta S={}&S_{0,>}[\phi^+]
+\int d^4x\left\{
\frac{h_0}{3!}\left[3\phi^2\phi^++3\phi(\phi^+)^2+(\phi^+)^3\right]\right.\\
&\left.\hspace{31mm}
+\frac{g_0}{4!}\left[4\phi^3\phi^++6\phi^2(\phi^+)^2
+4\phi(\phi^+)^3+(\phi^+)^4\right]\right\},
\end{aligned}
$$

where

$$
S_{0,>}[\phi^+]=\frac12\int d^4x\,
\left[(\partial\phi^+)^2+m_0^2(\phi^+)^2\right].
$$

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

When $h_0=0$, the cubic contribution is absent and

$$
\boxed{\Delta S=S_{0,>}[\phi^+]
+\frac{g_0}{4!}\int d^4x\,
\left[4\phi^3\phi^++6\phi^2(\phi^+)^2
+4\phi(\phi^+)^3+(\phi^+)^4\right].}
$$

Although terms odd in $\phi^+$ occur for a fixed low field, the simultaneous transformation $(\phi,\phi^+)\mapsto(-\phi,-\phi^+)$ shows that integrating out the shell preserves the original $\mathbb Z_2$ [discrete symmetry](../../../physics.md#discrete-symmetry) of the effective action.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Introduce the [renormalization-group beta functions](../../../perturbative-quantum-field-theory.md#beta-function-physics) and field anomalous dimension

$$
\beta_i=\Lambda\frac{dg_i}{d\Lambda},
\qquad
\beta_{m^2}=\Lambda\frac{dm^2}{d\Lambda},
\qquad
\gamma_\phi=\frac12\Lambda\frac{d\log Z_\Lambda}{d\Lambda}.
$$

Independence of physics from the arbitrary sliding scale gives the functional [Callan-Symanzik equation](../../../perturbative-quantum-field-theory.md#callan-symanzik-equation)

$$
\boxed{\left[
\Lambda\partial_\Lambda+\beta_{m^2}\partial_{m^2}
+\sum_i\beta_i\partial_{g_i}
-\gamma_\phi\int d^4x\,\phi(x)\frac{\delta}{\delta\phi(x)}
\right]S_\Lambda^{\rm eff}=0,}
$$

up to the equivalent sign convention obtained by defining $\gamma_\phi$ with a minus sign. For an operator $O_i$ of dimension $d_i$ containing $n_i$ fields, differentiating its coefficient shows the canonical and wave-function pieces

$$
\beta_i=(d_i-4+n_i\gamma_\phi)g_i+\beta_i^{\rm vertex},
$$

where $\beta_i^{\rm vertex}$ contains mixing among [local field operators](../../../quantum-field-theory.md#local-operator-physics) and genuine corrections at higher [loop order](../../../perturbative-quantum-field-theory.md#loop-order). Thus $d_i<4$, $d_i=4$, and $d_i>4$ canonically produce [relevant operators](../../../critical-phenomenon.md#relevant-operator), [marginal operators](../../../critical-phenomenon.md#marginal-operator), and [irrelevant operators](../../../critical-phenomenon.md#irrelevant-operator), respectively, before anomalous corrections.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Applying four functional derivatives to the functional equation gives the homogeneous equation for the renormalized [four-point one-particle-irreducible correlation function](../../../perturbative-quantum-field-theory.md#four-point-one-particle-irreducible-correlation-function):

$$
\boxed{\left[
\Lambda\partial_\Lambda+\beta_{m^2}\partial_{m^2}
+\sum_i\beta_i\partial_{g_i}-4\gamma_\phi
\right]
\Gamma_\Lambda^{(4)}(x_1,x_2,x_3,x_4;m^2,g_i)=0.}
$$

If the opposite convention for $\gamma_\phi$ is used, the last sign changes. The factor four counts the four external renormalized fields.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

A [continuum limit of a quantum field theory](../../../perturbative-quantum-field-theory.md#continuum-limit-of-a-quantum-field-theory) sends the [ultraviolet cutoff](../../../quantum-field-theory.md#ultraviolet-cutoff) $\Lambda_0$ to infinity while holding chosen physical masses and amplitudes fixed. In cutoff units this requires a diverging [correlation length](../../../critical-phenomenon.md#correlation-length), so the bare couplings must be tuned onto the [critical surface](../../../critical-phenomenon.md#critical-surface) of an ultraviolet [renormalization-group fixed point](../../../critical-phenomenon.md#renormalization-group-fixed-point). Each [relevant direction of a fixed point](../../../critical-phenomenon.md#relevant-direction-of-a-fixed-point) requires one coordinate fixed by measurement; predictivity requires only finitely many such directions, and irrelevant microscopic details disappear.

Several behaviors are possible. In an [asymptotically free](../../../perturbative-quantum-field-theory.md#asymptotic-freedom) theory the trajectory approaches a [Gaussian fixed point](../../../critical-phenomenon.md#gaussian-fixed-point) in the ultraviolet and interactions vanish logarithmically. In an [asymptotically safe quantum field theory](../../../perturbative-quantum-field-theory.md#asymptotic-safety) it approaches a non-Gaussian fixed point with finitely many relevant directions. A theory with a [Landau pole](../../../perturbative-quantum-field-theory.md#landau-pole) may possess only a [trivial quantum field theory](../../../perturbative-quantum-field-theory.md#quantum-triviality) as its continuum limit; retaining a nonzero interaction then requires a finite cutoff. Finally, if no ultraviolet-complete trajectory exists, the model remains an [effective field theory](../../../quantum-field-theory.md#effective-field-theory) valid only below a physical cutoff.

## 3

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Repeated insertions of the [fermion self-energy](../../../perturbative-quantum-field-theory.md#fermion-self-energy) form a geometric [Dyson resummation](../../../perturbative-quantum-field-theory.md#dyson-resummation):

$$
\begin{aligned}
G&=S_F+S_F\Sigma S_F+S_F\Sigma S_F\Sigma S_F+\cdots,\\
G(\not p)&=\boxed{\left[S_F(\not p)^{-1}-\Sigma(\not p)\right]^{-1}
=\left[i\not p+m-\Sigma(\not p)\right]^{-1}.}
\end{aligned}
$$

The physical fermion mass is the [pole mass](../../../perturbative-quantum-field-theory.md#pole-mass): after analytic continuation, $m_{\rm phys}$ is determined by the zero of the exact inverse propagator at $p^2=-m_{\rm phys}^2$. If

$$
\Sigma(\not p)=i\not p\,\Sigma_V(p^2)+m\Sigma_S(p^2),
$$

then to all orders the pole obeys

$$
m_{\rm phys}=m\,
\frac{1-\Sigma_S(-m_{\rm phys}^2)}
{1-\Sigma_V(-m_{\rm phys}^2)}
$$

with the signs fixed by the displayed Dyson convention.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The one-loop graph is a fermion line that emits and reabsorbs one internal photon:

<a id="3/b/image-one-loop-qed-fermion-self-energy"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-304-qed-self-energy.png)

**[Figure 1](#3/b/image-one-loop-qed-fermion-self-energy). One-loop QED fermion self-energy**. An external fermion of momentum p emits an internal photon of momentum p minus k, propagates with loop momentum k, and reabsorbs the photon.

The [QED Feynman rules](../../../perturbative-quantum-field-theory.md#qed-feynman-rules) assign $(-ie\gamma^\mu)(-ie\gamma^\nu)$ to the two vertices, the [Feynman-gauge photon propagator](../../../relativistic-quantum-field.md#feynman-gauge-photon-propagator) contracts $\mu$ and $\nu$ and contributes $\delta_{\mu\nu}/(p-k)^2$, and the internal [Dirac propagator](../../../quantum-field-theory.md#dirac-propagator) is $(-i\not k+m)/(k^2+m^2)$. Hence

$$
\boxed{\Sigma(\not p)=(-ie)^2\int\frac{d^4k}{(2\pi)^4}
\gamma^\mu\frac{-i\not k+m}{k^2+m^2}\gamma_\mu
\frac1{(p-k)^2}.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [kinetic terms](../../../quantum-field-theory.md#kinetic-term) determine the [engineering dimensions](../../../critical-phenomenon.md#engineering-dimension) in $d$ dimensions:

$$
[A_\mu]=\frac{d-2}{2},
\qquad [\psi]=\frac{d-1}{2}.
$$

Requiring $e\bar\psi\gamma^\mu A_\mu\psi$ to have dimension $d$ gives

$$
\boxed{[e]=\frac{4-d}{2}=\frac\epsilon2.}
$$

Thus the electric charge is dimensionless only in four dimensions. In [dimensional regularization](../../../perturbative-quantum-field-theory.md#dimensional-regularization) one writes the bare interaction with $e_0=\mu^{\epsilon/2}Z_e e$, where $e$ is dimensionless and the [renormalization scale](../../../perturbative-quantum-field-theory.md#renormalization-scale) $\mu$ supplies the missing dimension.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Use a [Feynman parameter](../../../perturbative-quantum-field-theory.md#feynman-parameter) with $A=k^2+m^2$ and $B=(p-k)^2$. Then

$$
xA+(1-x)B=[k-(1-x)p]^2+\Delta,
\qquad
\Delta=xm^2+x(1-x)p^2.
$$

The identities for [gamma matrices](../../../algebra.md#gamma-matrices) give

$$
\gamma^\mu(-i\not k+m)\gamma_\mu
=i(d-2)\not k+dm.
$$

After the shift $\ell=k-(1-x)p$, the term odd in $\ell$ integrates to zero. The rotationally symmetric loop integral is

$$
\int\frac{d^d\ell}{(2\pi)^d}\frac1{(\ell^2+\Delta)^2}
=\frac1{(4\pi)^{d/2}}\Gamma\left(\frac\epsilon2\right)
\Delta^{-\epsilon/2}.
$$

Consequently

$$
\boxed{\Sigma(\not p)=-\frac{e^2}{(4\pi)^{d/2}}
\Gamma\left(\frac\epsilon2\right)
\int_0^1dx\,
\frac{i(2-\epsilon)(1-x)\not p+(4-\epsilon)m}
{[xm^2+x(1-x)p^2]^{\epsilon/2}}.}
$$

Thus

$$
\boxed{C=i(2-\epsilon)(1-x),\qquad F=4-\epsilon,
\qquad\Delta=xm^2+x(1-x)p^2.}
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Restore the dimensional-regularization factor $\mu^\epsilon$ and define

$$
N_0=2i(1-x)\not p+4m,
\qquad N_1=i(1-x)\not p+m.
$$

Using $\Gamma(\epsilon/2)=2/\epsilon-\gamma+O(\epsilon)$ gives

$$
\boxed{\Sigma(\not p)=-\frac{e^2}{16\pi^2}\int_0^1dx
\left\{
\frac{2N_0}{\epsilon}
+N_0\left[\log\frac{4\pi\mu^2}{\Delta}-\gamma\right]
-2N_1
\right\}+O(\epsilon).}
$$

The first term is the [ultraviolet divergence](../../../perturbative-quantum-field-theory.md#ultraviolet-divergence). In the [modified minimal subtraction scheme](../../../perturbative-quantum-field-theory.md#modified-minimal-subtraction-scheme), subtraction of $2/\epsilon-\gamma+\log4\pi$ leaves

$$
\Sigma_{\overline{\rm MS}}(\not p)
=-\frac{e^2}{16\pi^2}\int_0^1dx
\left[N_0\log\frac{\mu^2}{\Delta}-2N_1\right].
$$

On the tree-level mass shell, $p^2=-m^2$ and $i\not p=-m$, so $\Delta=x^2m^2$. The [mass counterterm](../../../perturbative-quantum-field-theory.md#mass-counterterm) is

$$
\boxed{\delta m_{\overline{\rm MS}}
=-\frac{3e^2m}{16\pi^2}
\left(\frac2\epsilon-\gamma+\log4\pi\right).}
$$

The pole condition $m_{\rm phys}=m-\Sigma_{\overline{\rm MS}}|_{i\not p=-m}+O(e^4)$ therefore gives

$$
\boxed{m_{\rm phys}=m(\mu)\left[
1+\frac{e^2}{8\pi^2}\int_0^1dx
\left((1+x)\log\frac{\mu^2}{x^2m^2}-x\right)
\right]+O(e^4).}
$$

Evaluating the elementary parameter integral yields the equivalent expression

$$
m_{\rm phys}=m(\mu)\left[1+\frac{e^2}{4\pi^2}
\left(1+\frac34\log\frac{\mu^2}{m^2}\right)\right]+O(e^4).
$$

## 4

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For a short [Wilson line](../../../relativistic-quantum-field.md#wilson-line), a [gauge transformation](../../../electromagnetism.md#gauge-transformation) gives

$$
U'(x+an,x)=V(x+an)U(x+an,x)V^\dagger(x).
$$

Use $V(x+an)=1+i\alpha(x)+ia n^\mu\partial_\mu\alpha(x)+O(a^2,\alpha^2)$ and $U=1+iga n^\mu A_\mu+O(a^2)$. Keeping terms of order $a$, including $a\alpha$, gives

$$
U'=1+iga n^\mu
\left(A_\mu+\frac1g\partial_\mu\alpha+i[\alpha,A_\mu]\right)+O(a^2,\alpha^2).
$$

Since the [Lie bracket](../../../lie-algebra.md#lie-bracket) is encoded by the [Lie algebra structure constants](../../../lie-algebra.md#structure-constant-of-a-lie-algebra), $i[\alpha,A_\mu]^a=f^{abc}A_\mu^b\alpha^c$, and therefore

$$
\boxed{(A^\alpha)_\mu^a=A_\mu^a
+\frac1g\partial_\mu\alpha^a
+f^{abc}A_\mu^b\alpha^c.}
$$

This is the infinitesimal form of the [Wilson-line gauge transformation](../../../relativistic-quantum-field.md#wilson-line-gauge-transformation).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The variation found above uses the [adjoint covariant derivative](../../../relativistic-quantum-field.md#adjoint-covariant-derivative):

$$
\delta A_\mu^a=\frac1g(D_\mu\alpha)^a,
\qquad
(D_\mu c)^a=\partial_\mu c^a+g f^{abc}A_\mu^b c^c.
$$

For the [Lorenz gauge](../../../electromagnetism.md#lorenz-gauge-condition) functional $G^a[A]=\partial^\mu A_\mu^a$,

$$
\frac{\delta G^a[A^\alpha](x)}{\delta\alpha^b(y)}
=\frac1g\partial^\mu D_\mu^{ab}\delta(x-y).
$$

The field-independent factor $1/g$ may be absorbed into normalization. The [Grassmann Gaussian integral](../../../quantum-field-theory.md#grassmann-gaussian-integral) exponentiates the [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) with anticommuting [Faddeev-Popov ghost fields](../../../relativistic-quantum-field.md#faddeev-popov-ghost):

$$
\det(\partial^\mu D_\mu)
=\int\mathcal D\bar c\,\mathcal Dc\,
e^{-\int d^4x\,\bar c^a\partial^\mu(D_\mu c)^a}.
$$

A Gaussian average over the gauge condition supplies the covariant gauge-fixing term, so

$$
\boxed{S=S_g+\int d^4x\left[
\frac1{2\xi}(\partial^\mu A_\mu^a)^2
+\bar c^a\partial^\mu(D_\mu c)^a
\right],
\qquad
D_\mu^{ac}=\delta^{ac}\partial_\mu+g f^{abc}A_\mu^b.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The quadratic gauge-field action in momentum space is

$$
S^{(2)}=\frac12\int\frac{d^4k}{(2\pi)^4}
A_\mu^a(-k)\left[k^2\delta^{\mu\nu}
+\left(\frac1\xi-1\right)k^\mu k^\nu\right]A_\nu^a(k).
$$

In terms of the [transverse projector of a vector field](../../../relativistic-quantum-field.md#transverse-projector-of-a-vector-field) and [longitudinal projector of a vector field](../../../relativistic-quantum-field.md#longitudinal-projector-of-a-vector-field),

$$
P_T^{\mu\nu}=\delta^{\mu\nu}-\frac{k^\mu k^\nu}{k^2},
\qquad P_L^{\mu\nu}=\frac{k^\mu k^\nu}{k^2},
$$

the operator is $k^2(P_T+\xi^{-1}P_L)$. Its inverse, the [gauge-boson propagator](../../../relativistic-quantum-field.md#gauge-boson-propagator), is

$$
\boxed{D^{ab}_{\mu\nu}(k)=\frac{\delta^{ab}}{k^2}
\left(\delta_{\mu\nu}+(\xi-1)\frac{k_\mu k_\nu}{k^2}\right).}
$$

Therefore **$X=1$ and $Y=\xi-1$**.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/i">i</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/i/solution">Solution</h5>

↑ **Parent:** [I](#4/d/i)

Without [gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing), every [gauge orbit](../../../relativistic-quantum-field.md#gauge-orbit) is integrated infinitely many times and the quadratic gauge-field operator has a [zero mode in field theory](../../../relativistic-quantum-field.md#zero-mode-in-field-theory) for every pure-gauge direction. It therefore has no inverse and no propagator. A gauge condition selects one representative per orbit, up to global transformations and the possible nonperturbative [Gribov ambiguity](../../../relativistic-quantum-field.md#gribov-ambiguity), and makes perturbative Gaussian integration well defined.

<h4 id="4/d/ii">ii</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/d/ii)

The anticommuting fields $c$ and $\bar c$ represent the field-dependent [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant). They are Lorentz-scalar [Grassmann fields](../../../quantum-field-theory.md#grassmann-field), appear only on internal lines, and contribute a minus sign for each closed [ghost loop](../../../relativistic-quantum-field.md#ghost-loop). Their diagrams cancel unphysical gauge-polarization contributions and are required for gauge-independent, unitary amplitudes in a non-Abelian covariant gauge.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

For [axial gauge](../../../relativistic-quantum-field.md#axial-gauge), $G^a[A]=n^\mu A_\mu^a$. Its Faddeev-Popov operator is

$$
\frac{\delta G^a[A^\alpha]}{\delta\alpha^b}
=\frac1g n^\mu D_\mu^{ab}
=\frac1g n\mathbin\cdot\partial\,\delta^{ab}
+n^\mu f^{acb}A_\mu^c.
$$

On the gauge slice $n\mathbin\cdot A^c=0$, the second term vanishes. Hence

$$
\boxed{\Delta_{\rm FP}[A]\big|_{n\cdot A=0}
=\det\left(\frac1g n\mathbin\cdot\partial\right),}
$$

This [functional determinant](../../../quantum-field-theory.md#functional-determinant) is independent of the gauge field and may be absorbed into the normalization of the [path integral](../../../quantum-field-theory.md#path-integral). Any introduced ghosts are free and decouple, so **no ghost fields are needed in axial gauge**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
