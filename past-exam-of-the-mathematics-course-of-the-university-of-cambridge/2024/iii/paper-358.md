# Paper 358

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_358.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_358.pdf)

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
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 358](paper-358.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [computational problem in the SCI hierarchy](../../../functional-analysis.md#computational-problem-in-the-sci-hierarchy) is a quadruple

$$
(\Xi,\Omega,\mathcal M,\Lambda).
$$

Here $\Omega$ is the primary set of inputs, $\Lambda$ is the set of permitted evaluation functions, $(\mathcal M,d)$ is the output [metric space](../../../topological-analysis.md#metric-space), and $\Xi:\Omega\to\mathcal M$ is the problem function. The [Solvability complexity index](../../../functional-analysis.md#solvability-complexity-index) is defined from the minimum height of a [tower of algorithms](../../../functional-analysis.md#tower-of-algorithms) that computes $\Xi$ from finite subsets of $\Lambda$.

For the [classical computational spectral problem](../../../functional-analysis.md#classical-computational-spectral-problem), take

$$
\Omega=\mathcal B(\ell^2(\mathbb N)),\qquad
\lambda_{ij}(A)=\langle Ae_j,e_i\rangle,\qquad
\Lambda=\{\lambda_{ij}:i,j\in\mathbb N\},
$$

and

$$
\Xi(A)=\operatorname{Sp}(A).
$$

Since the [spectrum of a bounded operator](../../../linear-operator-theory.md#spectrum-of-a-bounded-operator) is a nonempty [compact subset](../../../topology.md#compact-space) of the [complex numbers](../../../complex-analysis.md#complex-number), one may take $\mathcal M$ to be the nonempty compact subsets of $\mathbb C$ with the [Hausdorff distance](../../../topological-analysis.md#hausdorff-distance). The [Attouch--Wets topology](../../../functional-analysis.md#attouch-wets-topology) gives an equivalent convenient formulation on bounded spectral sets and also extends naturally to unbounded closed sets. This choice of $\mathcal M$ makes convergence mean convergence of the whole spectrum as a set, including both the absence of persistent [spectral pollution](../../../functional-analysis.md#spectral-pollution) and the approximation of every genuine spectral point.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A [general algorithm in the SCI hierarchy](../../../functional-analysis.md#general-algorithm-in-the-sci-hierarchy) $\Gamma:\Omega\to\mathcal M$ reads a finite set $\Lambda_\Gamma(A)\subset\Lambda$ on each input $A$. Its output depends only on those values, and whenever another input $B$ has the same values on $\Lambda_\Gamma(A)$, the algorithm requests the same finite set and gives the same output. A [tower of algorithms](../../../functional-analysis.md#tower-of-algorithms) of height $k$ satisfies

$$
\Xi(A)=\lim_{n_k\to\infty}\cdots\lim_{n_1\to\infty}
\Gamma_{n_k,\ldots,n_1}(A)
$$

for every $A\in\Omega$. The [Solvability complexity index](../../../functional-analysis.md#solvability-complexity-index) is the least such $k$, with value zero when one finite algorithm computes $\Xi$ exactly.

We reduce a known height-three [finite-column decision problem](../../../functional-analysis.md#finite-column-decision-problem) to spectral computation. Let $(a_{ij})_{i,j\in\mathbb Z}$ be a bi-infinite zero-one matrix and let $\Xi_{\rm col}$ ask whether there is a number $D$ such that every column either contains fewer than $D$ ones or has infinitely many ones in both directions. The lecture lower-bound theorem states

$$
\operatorname{SCI}(\Xi_{\rm col})_G=3,
$$

even for unrestricted general algorithms.

For a zero-one sequence $a=(a_i)_{i\in\mathbb Z}$, define $B_a$ on $\ell^2(\mathbb Z)$ to be the identity on coordinates where $a_i=0$ and the shift from each coordinate with $a_i=1$ to the next coordinate carrying a one. It is a direct sum of identity pieces and one shift chain. Consequently:

- finitely many ones give $\operatorname{Sp}(B_a)\subset\{0,1\}$;
- infinitely many ones in both directions give the unit circle $\mathbb T$;
- a one-sided infinite sequence gives the closed unit disk $\overline{\mathbb D}$.

For the columns $a^{(j)}=(a_{ij})_i$, form the bounded direct-sum operator

$$
C(a)=\bigoplus_{j\in\mathbb Z}B_{a^{(j)}}.
$$

Every finite set of matrix entries of $C(a)$ is determined by finitely many entries of $a$, so this construction respects the finite-information condition for a [general algorithm in the SCI hierarchy](../../../functional-analysis.md#general-algorithm-in-the-sci-hierarchy). The preceding trichotomy implies

$$
\Xi_{\rm col}(a)=\mathrm{No}
\quad\Longrightarrow\quad
\operatorname{Sp}(C(a))=\overline{\mathbb D},
$$

whereas

$$
\Xi_{\rm col}(a)=\mathrm{Yes}
\quad\Longrightarrow\quad
\operatorname{Sp}(C(a))\subset\{0\}\cup\mathbb T.
$$

The two cases are separated by the point $1/2$: its distance from the spectrum is respectively zero and $1/2$.

If a height-two tower $\Gamma_{n_2,n_1}$ computed the spectrum of every bounded operator, apply it to $C(a)$ and inspect

$$
\alpha_{n_2,n_1}
=\operatorname{dist}\!\left(\frac12,\Gamma_{n_2,n_1}(C(a))\right).
$$

Use the disjoint intervals $[0,1/8]$ and $[3/8,\infty)$ to turn each finite output into Yes or No, retaining the latest inner-stage value that lies in either interval. Convergence in the [Hausdorff distance](../../../topological-analysis.md#hausdorff-distance) ensures that the inner limit stabilizes; the outer limit answers $\Xi_{\rm col}$ correctly. This would give a height-two tower for a problem whose [Solvability complexity index](../../../functional-analysis.md#solvability-complexity-index) is three, a contradiction. Therefore

$$
\boxed{\operatorname{SCI}(\operatorname{Sp},
\mathcal B(\ell^2(\mathbb N)))\geq3.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $L_n=\operatorname{span}\{e_1,\ldots,e_n\}$ and let $P_n$ be its [orthogonal projection](../../../hilbert-space.md#orthogonal-projection). For $z\in\mathbb C$, define

$$
\gamma_n(z)^2
=\lambda_{\min}\!\left(
(1+|z|^2)I_n-\bar z\,P_nAP_n-z\,P_nA^*P_n
\right).
$$

Because $A$ is [unitary](../../../vector-space.md#unitary-operator),

$$
\gamma_n(z)
=\inf_{\substack{x\in L_n\\\|x\|=1}}\|(A-zI)x\|.
$$

The displayed finite [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) uses only finitely many matrix entries of $A$, and its least eigenvalue can be approximated by an [arithmetic algorithm in the SCI hierarchy](../../../functional-analysis.md#arithmetic-algorithm-in-the-sci-hierarchy).

As $L_n$ increases densely,

$$
\gamma_n(z)\downarrow
\inf_{\|x\|=1}\|(A-zI)x\|.
$$

A [unitary operator](../../../vector-space.md#unitary-operator) is [normal](../../../hilbert-space.md#normal-operator), so the [spectral theorem for normal operators on a separable Hilbert space](../../../hilbert-space.md#spectral-theorem-for-normal-operators-on-a-separable-hilbert-space) identifies the limit as

$$
\operatorname{dist}(z,\operatorname{Sp}(A)).
$$

The functions $\gamma_n$ are continuous and decrease to a continuous function on the compact unit circle. The [Dini theorem](../../../real-analysis.md#dini-s-theorem) therefore gives uniform convergence there.

Take successively finer rational meshes $G_n$ around $\mathbb T$. From the finitely computed values of $\gamma_n$, retain the mesh minima in the comparison neighborhoods whose radii are $\gamma_n(z)$; equivalently, use the standard local-minimum construction for a decreasing approximation to a distance function. Call the resulting finite set $\Gamma_n(A)$. Uniform convergence and the shrinking mesh imply

$$
\boxed{\Gamma_n(A)\longrightarrow\operatorname{Sp}(A)}
$$

in [Hausdorff distance](../../../topological-analysis.md#hausdorff-distance). Every operation at stage $n$ is finite and arithmetic, so $(\Gamma_n)$ is the required one-limit sequence.

There is no finite-stage certificate that the whole output has the correct Hausdorff error: the convergence of $\gamma_n$ has no uniform computable rate over all unitary operators, and unseen matrix entries can still reveal a missing spectral component. A small computed residual can certify that an individual output point lies near the spectrum, but it cannot verify that $\Gamma_n(A)$ covers all of $\operatorname{Sp}(A)$. Thus the full finite-stage output is not verifiable without additional information.

## 2

↑ **Parent:** [Paper 358](paper-358.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [projection-valued measure](../../../hilbert-space.md#projection-valued-measure) on the [Borel sets](../../../measure-theory.md#borel-set) of $\mathbb C$ is a map $E$ into the [orthogonal projections](../../../hilbert-space.md#orthogonal-projection) on a [separable Hilbert space](../../../hilbert-space.md#separable-hilbert-space) $\mathcal H$ such that

$$
E(\varnothing)=0,\qquad E(\mathbb C)=I,\qquad
E(B\cap C)=E(B)E(C),
$$

and for pairwise disjoint $B_j$,

$$
E\!\left(\bigcup_jB_j\right)v=\sum_jE(B_j)v
$$

for every $v\in\mathcal H$, with convergence in norm.

The [spectral theorem for normal operators on a separable Hilbert space](../../../hilbert-space.md#spectral-theorem-for-normal-operators-on-a-separable-hilbert-space) states that a bounded [normal operator](../../../hilbert-space.md#normal-operator) $A$ has a unique projection-valued measure supported on $\operatorname{Sp}(A)$ for which

$$
\boxed{A=\int_{\operatorname{Sp}(A)}z\,dE(z).}
$$

More generally, the [Borel functional calculus for a normal operator](../../../banach-algebra.md#borel-functional-calculus-for-a-normal-operator) is

$$
f(A)=\int f(z)\,dE(z).
$$

For $v,w\in\mathcal H$, the [scalar spectral measures](../../../hilbert-space.md#scalar-spectral-measure) are

$$
\mu_{v,w}(B)=\langle E(B)v,w\rangle,
\qquad
\mu_v=\mu_{v,v}.
$$

If $A$ is [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator), its spectrum and hence the support of $E$ lie in $\mathbb R$. Moreover,

$$
\mu_v(B)=\langle E(B)v,v\rangle=\|E(B)v\|^2\geq0,
$$

so $\mu_v$ is a [positive measure](../../../measure-theory.md#positive-measure), and

$$
\boxed{\mu_v(\mathbb R)=\langle Iv,v\rangle=\|v\|^2.}
$$

The paper prints total mass $\|v\|$; with the standard definition it is $\|v\|^2$, so the unsquared norm is a typographical error.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $E_n$ and $E$ be the [projection-valued measures](../../../hilbert-space.md#projection-valued-measure) of $A_n$ and $A$. Using the projection $P_n:\mathcal H\to\mathcal H_n$, define

$$
\mu^{(n)}_{v,w}(B)
=\langle E_n(B)P_nv,P_nw\rangle.
$$

The [scalar spectral measures](../../../hilbert-space.md#scalar-spectral-measure) converge weakly when

$$
\boxed{
\int_{\mathbb R}f\,d\mu^{(n)}_{v,w}
\longrightarrow
\int_{\mathbb R}f\,d\mu_{v,w}}
$$

for every bounded [continuous function](../../../calculus.md#continuous-function) $f$ and every $v,w\in\mathcal H$. By the [spectral theorem for normal operators on a separable Hilbert space](../../../hilbert-space.md#spectral-theorem-for-normal-operators-on-a-separable-hilbert-space), this is equivalent to

$$
\langle f(A_n)P_nv,P_nw\rangle
\longrightarrow
\langle f(A)v,w\rangle.
$$

The assumed moment identities say precisely that this convergence holds for every monomial $f(x)=x^m$. It follows by [linearity](../../../vector-space.md#linearity) for every [polynomial](../../../polynomial.md). For $v=w$, the $m=2$ identity gives

$$
\int x^2\,d\mu^{(n)}_v(x)\longrightarrow
\int x^2\,d\mu_v(x),
$$

so [Markov inequality](../../../probability-inequality.md#markov-inequality) makes the positive measures $(\mu^{(n)}_v)$ tight. Higher even moments similarly control the tails of any fixed polynomial.

Given a bounded continuous $f$ and $\epsilon>0$, choose $R$ so that the measure tails are uniformly small. The [Weierstrass approximation theorem](../../../functional-analysis.md#weierstrass-approximation-theorem) supplies a polynomial $p$ with

$$
\sup_{|x|\leq R}|f(x)-p(x)|<\epsilon.
$$

Moment convergence handles $p$; tightness and a sufficiently high even moment handle the two tails. Hence $\int f\,d\mu_v^{(n)}\to\int f\,d\mu_v$. The [polarization identity](../../../linear-algebra.md#polarization-identity) then gives the same conclusion for $\mu_{v,w}^{(n)}$. This proves [weak convergence of scalar spectral measures](../../../hilbert-space.md#weak-convergence-of-scalar-spectral-measures).

The assertion fails if only $m=1$ is assumed. Let $\mathcal H=\ell^2(\mathbb N)$, let $\mathcal H_n=\operatorname{span}\{e_1,\ldots,e_n\}$, take $A=0$, and let

$$
A_ne_j=e_{n+1-j}
\qquad(1\leq j\leq n).
$$

The reversal matrices are self-adjoint unitaries. For fixed $v,w\in\ell^2$,

$$
\langle A_nP_nv,P_nw\rangle\longrightarrow0,
$$

because the finite head of one vector is paired with the vanishing tail of the other. Thus the $m=1$ condition holds. However, $A_n^2=I_{\mathcal H_n}$, so

$$
\langle A_n^2P_nv,P_nw\rangle
\longrightarrow\langle v,w\rangle
\ne0=\langle A^2v,w\rangle
$$

in general. Taking $f(x)=x^2$ shows that the spectral measures do not converge weakly.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Here [functional calculus convergence](../../../banach-algebra.md#functional-calculus-convergence) means that for every $f\in C(\mathbb T)$,

$$
\boxed{
\langle f(A_n)P_nv,P_nw\rangle
\longrightarrow
\langle f(A)v,w\rangle
\qquad(v,w\in\mathcal H).}
$$

Embed $\mathcal H_n$ in $\mathcal H$ and write $\widetilde A_n=P_n^*A_nP_n$. The hypothesis gives $\widetilde A_n\rightharpoonup A$ in the [weak operator topology](../../../functional-analysis.md#weak-operator-topology). Since $A_n$ and $A$ are [unitary operators](../../../vector-space.md#unitary-operator),

$$
\|\widetilde A_nv-Av\|^2
=\|P_nv\|^2+\|v\|^2
-2\operatorname{Re}\langle\widetilde A_nv,Av\rangle
\longrightarrow0.
$$

Thus $\widetilde A_n\to A$ in the [strong operator topology](../../../functional-analysis.md#strong-operator-topology). Applying the same argument to the adjoints gives $\widetilde A_n^*\to A^*$ strongly.

Products of uniformly bounded strongly convergent operators converge strongly, so for every integer $k$,

$$
P_n^*A_n^kP_n\longrightarrow A^k
$$

strongly, with negative $k$ interpreted through adjoints. Therefore convergence holds for every [Laurent polynomial](../../../polynomial.md#laurent-polynomial). The [Stone-Weierstrass theorem](../../../functional-analysis.md#stone-weierstrass-theorem) says that Laurent polynomials are uniformly dense in $C(\mathbb T)$. Since the continuous functional calculus is contractive, uniform approximation finishes the proof for every $f\in C(\mathbb T)$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let $P_n:\ell^2(\mathbb N)\to\mathbb C^n$ be coordinate projection and set

$$
T_n=P_nAP_n^*.
$$

This finite matrix is computable from the matrix entries of $A$. Compute its [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition)

$$
T_n=V_n\Sigma_nW_n^*
$$

and define the [unitary polar factor of a finite compression](../../../banach-algebra.md#unitary-polar-factor-of-a-finite-compression)

$$
\boxed{A_n=V_nW_n^*.}
$$

This is a unitary operator on $\mathbb C^n$, including when $T_n$ is singular.

Put $Q_n=P_n^*P_n$. Since $Q_n\to I$ strongly and $A$ is unitary,

$$
P_n^*T_n^*T_nP_nv
=Q_nA^*Q_nAQ_nv\longrightarrow v.
$$

The continuous functional calculus for positive matrices therefore gives

$$
P_n^*|T_n|P_nv\longrightarrow v.
$$

The polar identity $T_n=A_n|T_n|$ now yields

$$
\|P_n^*(A_n-T_n)P_nv\|
=\|(I-|T_n|)P_nv\|\longrightarrow0.
$$

Also $P_n^*T_nP_n=Q_nAQ_n\to A$ strongly, and hence

$$
\boxed{P_n^*A_nP_n\longrightarrow A\quad\text{strongly}.}
$$

In particular the weak convergence required in part (c) holds. The construction uses only a finite block of the given matrix and a finite [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition), so it is an algorithm realizing all the assumptions of part (c).

## 3

↑ **Parent:** [Paper 358](paper-358.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

The map $F$ is a [nonsingular transformation](../../../measure-theory.md#nonsingular-transformation) with respect to $\omega$ when

$$
\omega(N)=0\quad\Longrightarrow\quad
\omega(F^{-1}(N))=0.
$$

Equivalently, the [pushforward measure](../../../measure-theory.md#pushforward-measure) $F_*\omega(B)=\omega(F^{-1}(B))$ satisfies $F_*\omega\ll\omega$.

For an essentially bounded observable $g$, define the [Koopman operator](../../../measure-theory.md#koopman-operator)

$$
\boxed{K_Fg=g\circ F.}
$$

Nonsingularity makes this well defined on almost-everywhere equivalence classes. By the [Radon-Nikodym theorem](../../../measure-theory.md#radon-nikodym-theorem),

$$
\|K_Fg\|_2^2
=\int|g|^2\,d(F_*\omega)
=\int|g|^2\frac{d(F_*\omega)}{d\omega}\,d\omega.
$$

Consequently the [bounded Koopman operator criterion](../../../measure-theory.md#bounded-koopman-operator-criterion) is

$$
\boxed{
K_F:L^2(\omega)\to L^2(\omega)\text{ is bounded}
\iff
\frac{d(F_*\omega)}{d\omega}\in L^\infty(\omega).}
$$

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

The map $F$ is a [measure-preserving transformation](../../../measure-theory.md#measure-preserving-transformation) when

$$
\boxed{\omega(F^{-1}(B))=\omega(B)}
$$

for every [Borel set](../../../measure-theory.md#borel-set) $B$, equivalently $F_*\omega=\omega$. In this case its [Koopman operator](../../../measure-theory.md#koopman-operator) is an [isometry](../../../riemannian-geometry.md#isometry) on $L^2(\omega)$.

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

The map is invertible with respect to $\omega$ when there is a measurable $G:X\to X$ such that

$$
G\circ F=\operatorname{id},
\qquad
F\circ G=\operatorname{id}
$$

almost everywhere. For an [invertible measure-preserving system](../../../measure-theory.md#invertible-measure-preserving-system), $K_G=K_F^{-1}=K_F^*$, so its [Koopman operator](../../../measure-theory.md#koopman-operator) is unitary.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Suppose first that the system is [ergodic](../../../measure-theory.md#ergodicity) and $K_Fg=g$. For each real $t$, the level set

$$
E_t=\{x:\operatorname{Re}g(x)>t\}
$$

is invariant modulo a null set, so $\omega(E_t)\in\{0,1\}$. The distribution function of $\operatorname{Re}g$ can therefore jump only once, which makes $\operatorname{Re}g$ constant almost everywhere. The same argument applies to $\operatorname{Im}g$.

Conversely, if $E$ is invariant, then $K_F\mathbf1_E=\mathbf1_E$. If every invariant $L^2$ function is constant, the [indicator function](../../../measure-theory.md#indicator-function) $\mathbf1_E$ is almost everywhere zero or one, and hence $\omega(E)=0$ or $1$. This proves the [invariant-function characterization of ergodicity](../../../measure-theory.md#invariant-function-characterization-of-ergodicity).

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Use the [Fourier basis](../../../fourier-series.md#fourier-basis)

$$
e_k(x)=e^{ikx},\qquad k\in\mathbb Z,
$$

of $L^2([-\pi,\pi]_{\rm per})$. For the rotation $F(x)=x+a$,

$$
K_Fe_k=e^{ika}e_k.
$$

If $a/\pi$ is irrational, $e^{ika}=1$ implies $k=0$. Hence every fixed $L^2$ function has only its constant Fourier coefficient, and part (i) proves ergodicity.

If $a/\pi=p/q$ is rational, then

$$
e_{2q}(x)=e^{i2qx}
$$

is a nonconstant fixed function because $e^{i2qa}=e^{i2\pi p}=1$. Part (i) now shows that the system is not ergodic. Therefore the [ergodicity criterion for a circle rotation](../../../measure-theory.md#ergodicity-criterion-for-a-circle-rotation) is

$$
\boxed{F\text{ is ergodic}\iff a/\pi\notin\mathbb Q.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For [inexact information in the SCI hierarchy](../../../functional-analysis.md#inexact-information-in-the-sci-hierarchy), replace every exact evaluation $\lambda\in\Lambda$ by a family of admissible approximations $\lambda_m$ satisfying

$$
d(\lambda_m(A),\lambda(A))\leq2^{-m}.
$$

An algorithm must converge for every admissible choice of approximations, not merely for one favored encoding.

For continuous nonsingular maps $F:X\to X$, take the evaluations to be arbitrary point queries. At precision $m$, a query at $x\in X$ returns any $y$ satisfying

$$
\boxed{d_X(y,F(x))\leq2^{-m}.}
$$

Thus the information set contains all triples $(x,m,y)$ satisfying this inequality. This is a [perfect measurement device for a dynamical system](../../../functional-analysis.md#perfect-measurement-device-for-a-dynamical-system): it can sample any state, at any requested accuracy, with no fixed noise floor. The finite-information rule still requires each terminating computation to make only finitely many such measurements.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Assume for contradiction that a sequence of general algorithms $\Gamma_n$ decides ergodicity from the perfect measurement data, so that $\Gamma_n(F)$ eventually equals $\Xi_{\rm erg}(F)$ for every $F\in\Omega$.

Restrict the input class to the circle rotations

$$
F_a(x)=x+a\pmod{2\pi}.
$$

From [inexact information in the SCI hierarchy](../../../functional-analysis.md#inexact-information-in-the-sci-hierarchy) for the real number $a$, one can answer every requested measurement of $F_a(x)$ to the same precision. The supposed algorithms would therefore give a one-limit decision procedure for

$$
a\longmapsto\mathbf1_{\mathbb R\setminus\mathbb Q}(a/\pi),
$$

because part (b)(ii) identifies ergodicity with irrationality.

Every finite-information general algorithm is locally constant on a sufficiently small cylinder of the inexact data. A pointwise limit of a sequence of such functions is a [Baire class one function](../../../topological-analysis.md#baire-class-one-function). But the rationality indicator is discontinuous at every real number: every interval contains both rational and irrational numbers. The theorem that the discontinuity set of a Baire class one function is meagre, or directly [rationality indicator is not Baire class one](../../../topological-analysis.md#rationality-indicator-is-not-baire-class-one), gives a contradiction.

Hence no one-limit tower of general algorithms can decide ergodicity, even with the perfect measurement device:

$$
\boxed{
\{\Xi_{\rm erg},\Omega,\{0,1\},\Lambda\}^{\Delta_1}
\notin\Delta_2^G.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
