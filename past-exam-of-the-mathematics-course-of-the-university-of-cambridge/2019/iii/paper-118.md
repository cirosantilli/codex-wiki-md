# Paper 118

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_118.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_118.pdf)

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
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
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
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)

## 1

↑ **Parent:** [Paper 118](paper-118.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [complex manifold](../../../complex-geometry.md#complex-manifold) of complex dimension $n$ is a Hausdorff, second-countable [topological manifold](../../../topology.md#topological-manifold) with charts to open subsets of $\mathbb C^n$ whose transition maps are [biholomorphic](../../../complex-analysis.md#biholomorphism). A rank-$r$ [holomorphic vector bundle](../../../complex-geometry.md#holomorphic-vector-bundle) is a complex [vector bundle](../../../fiber-bundle.md#vector-bundle) with local trivializations $E|_U\cong U\times\mathbb C^r$ whose transition matrices are holomorphic maps to $\operatorname{GL}_r(\mathbb C)$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

In a [holomorphic coordinate](../../../complex-geometry.md#holomorphic-coordinate) chart, $T^{1,0}X$ has frame $\partial/\partial z^1,\ldots,\partial/\partial z^n$. Under a holomorphic coordinate change $w=w(z)$, the [chain rule](../../../calculus.md#chain-rule) gives

$$
\frac{\partial}{\partial z^j}=\sum_k\frac{\partial w^k}{\partial z^j}\frac{\partial}{\partial w^k}.
$$

The Jacobian is an invertible matrix of [holomorphic functions](../../../complex-analysis.md#holomorphic-function). These frames therefore make $T^{1,0}X$ the [holomorphic tangent bundle](../../../complex-geometry.md#holomorphic-tangent-bundle).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

On each member of a cover, choose a reduced [local defining function of a complex analytic hypersurface](../../../complex-geometry.md#local-defining-function-of-a-complex-analytic-hypersurface) $f_i$ for $Y$. On overlaps $f_i=g_{ij}f_j$ for $g_{ij}\in\mathcal O_X^*$. Since $f_j|_Y=0$,

$$
df_i|_Y=g_{ij}df_j|_Y.
$$

Each $df_i$ annihilates $TY$ and is nonzero in the normal direction because $Y$ is smooth. If $e_i=g_{ij}^{-1}e_j$ are the frames of the [holomorphic line bundle associated to a divisor](../../../complex-geometry.md#holomorphic-line-bundle-associated-to-a-divisor) $\mathcal O(Y)$, then

$$
[v]\longmapsto df_i(v)e_i
$$

is a well-defined nowhere-zero holomorphic map of line bundles. Thus the [normal bundle of a smooth analytic hypersurface](../../../complex-geometry.md#normal-bundle-of-a-smooth-analytic-hypersurface) is

$$
\boxed{N_{Y/X}\cong\mathcal O(Y)|_Y.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The tangent-normal [short exact sequence](../../../module-theory.md#short-exact-sequence)

$$
0\longrightarrow TY\longrightarrow TX|_Y\longrightarrow N_{Y/X}\longrightarrow0
$$

gives $\det(TX|_Y)\cong\det(TY)\otimes N_{Y/X}$. Dualizing and using the [canonical bundle](../../../complex-geometry.md#canonical-bundle),

$$
K_X|_Y\cong K_Y\otimes N_{Y/X}^*.
$$

Since $N_{Y/X}\cong\mathcal O(Y)|_Y$, rearrangement proves the [adjunction formula](../../../complex-geometry.md#adjunction-formula)

$$
\boxed{K_Y\cong(K_X\otimes\mathcal O(Y))|_Y.}
$$

## 2

↑ **Parent:** [Paper 118](paper-118.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For an ordered [open cover](../../../topology.md#open-cover) $\mathcal U=(U_i)$ and a [sheaf of sets](../../../algebraic-geometry.md#sheaf-mathematics) $\mathcal F$, the [Čech cochain group](../../../ringed-space.md#cech-cochain-group) is

$$
\check C^p(\mathcal U,\mathcal F)=\prod_{i_0<\cdots<i_p}\mathcal F(U_{i_0}\cap\cdots\cap U_{i_p}).
$$

Its [Čech coboundary](../../../ringed-space.md#cech-coboundary) is

$$
(\delta c)_{i_0\ldots i_{p+1}}=\sum_{r=0}^{p+1}(-1)^r
c_{i_0\ldots\widehat{i_r}\ldots i_{p+1}}|.
$$

Terms in $\delta^2$ cancel in pairs. Hence

$$
\boxed{\check H^j(\mathcal U,\mathcal F)=\ker(\delta:\check C^j\to\check C^{j+1})/
\operatorname{im}(\delta:\check C^{j-1}\to\check C^j).}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Take pairwise disjoint coordinate discs $U_m$ around $x_m$ and put $U_0=S\setminus\{x_1,\ldots,x_N\}$. A prescribed [principal part of a meromorphic function](../../../complex-geometry.md#principal-part-of-a-meromorphic-function) $P_m$ is holomorphic on $U_0\cap U_m$. Define

$$
P_{0m}=P_m,\qquad P_{m0}=-P_m,
$$

with all other components zero. No three distinct cover members meet, so the [Čech cocycle condition](../../../ringed-space.md#cech-cocycle-condition) is automatic. Thus $(P_{ij})$ is a Čech one-cocycle for $\mathcal O$.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

If $\check H^1(S,\mathcal O)=0$, that cocycle is a [Čech coboundary](../../../ringed-space.md#cech-coboundary): there are $f_i\in\mathcal O(U_i)$ with

$$
P_m=f_m-f_0\quad\text{on }U_0\cap U_m.
$$

Set $F=-f_0$ on $U_0$ and $F=P_m-f_m$ on $U_m$. These formulas agree on overlaps, so the [sheaf gluing axiom](../../../algebraic-geometry.md#sheaf-gluing-axiom) gives a global [meromorphic function](../../../isolated-singularity.md#meromorphic-function). Moreover $F-P_m=-f_m$ is holomorphic near $x_m$. Thus $F$ solves the [Mittag-Leffler problem on a Riemann surface](../../../complex-geometry.md#mittag-leffler-problem-on-a-riemann-surface) with precisely the prescribed principal parts.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $\Omega^p$ be the sheaf of holomorphic $p$-forms and $\mathcal A^{p,q}$ the sheaf of smooth $(p,q)$-forms. The [Dolbeault-Poincaré lemma](../../../complex-geometry.md#dolbeault-poincare-lemma) makes

$$
0\longrightarrow\Omega^p\longrightarrow\mathcal A^{p,0}\xrightarrow{\bar\partial}\mathcal A^{p,1}\xrightarrow{\bar\partial}\cdots
$$

an exact resolution by [fine sheaves](../../../ringed-space.md#fine-sheaf), which are acyclic for [global sections](../../../ringed-space.md#global-section). Its global cochain complex computes [Dolbeault cohomology](../../../complex-geometry.md#dolbeault-cohomology), proving the [Dolbeault theorem](../../../complex-geometry.md#dolbeault-theorem)

$$
\boxed{H^q(X,\Omega^p)\cong H_{\bar\partial}^{p,q}(X).}
$$

## 3

↑ **Parent:** [Paper 118](paper-118.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $\mathcal K_X^*$ be the sheaf of nonzero meromorphic functions. A local equation for a [divisor on a complex manifold](../../../complex-geometry.md#divisor-on-a-complex-manifold) is determined modulo a nowhere-zero holomorphic factor and hence defines a section of the [divisor sheaf on a complex manifold](../../../complex-geometry.md#divisor-sheaf-on-a-complex-manifold) $\mathcal K_X^*/\mathcal O_X^*$. Conversely, local representatives of such a section have quotients in $\mathcal O_X^*$, so their zero and pole orders agree on overlaps and define a divisor. The constructions are inverse:

$$
\boxed{\operatorname{Div}(X)\cong H^0(X,\mathcal K_X^*/\mathcal O_X^*).}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The exact sequence

$$
0\longrightarrow\mathcal O_X^*\longrightarrow\mathcal K_X^*
\longrightarrow\mathcal K_X^*/\mathcal O_X^*\longrightarrow0
$$

induces a [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology). Under $H^0(\mathcal K_X^*/\mathcal O_X^*)=\operatorname{Div}(X)$ and $H^1(\mathcal O_X^*)=\operatorname{Pic}(X)$, its [connecting homomorphism](../../../homology.md#connecting-homomorphism) is the [divisor-to-Picard map](../../../complex-geometry.md#divisor-to-picard-map) $D\mapsto\mathcal O(D)$. Exactness identifies its kernel with divisors of global nonzero [meromorphic functions](../../../isolated-singularity.md#meromorphic-function), namely [principal divisors](../../../algebraic-geometry.md#principal-divisor-on-an-algebraic-curve):

$$
\boxed{\ker(\operatorname{Div}(X)\to\operatorname{Pic}(X))=\operatorname{Prin}(X).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

A [holomorphic line bundle](../../../complex-geometry.md#holomorphic-line-bundle) is [ample](../../../ringed-space.md#ample-line-bundle) when some positive [tensor power](../../../linear-algebra.md#tensor-power) is [very ample](../../../ringed-space.md#very-ample-line-bundle), so its sections define an embedding into [Complex projective space](../../../algebraic-topology.md#complex-projective-space). It is a [positive holomorphic line bundle](../../../complex-geometry.md#positive-holomorphic-line-bundle) when it has a [Hermitian metric](../../../complex-geometry.md#hermitian-metric-on-a-holomorphic-vector-bundle) with positive Chern curvature $iF_\nabla$. The [Kodaira embedding theorem](../../../complex-geometry.md#kodaira-embedding-theorem) says that a compact [complex manifold](../../../complex-geometry.md#complex-manifold) carrying a positive holomorphic line bundle is projective; sufficiently high tensor powers give a [holomorphic embedding](../../../complex-geometry.md#holomorphic-embedding) into projective space.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Choose a [very ample line bundle](../../../ringed-space.md#very-ample-line-bundle) $A$ on $X$. By the theorem that a [high ample twist is very ample](../../../ringed-space.md#high-ample-twist-is-very-ample), for sufficiently large $m$ both

$$
H_1=A^{\otimes m}\otimes L,\qquad H_2=A^{\otimes m}
$$

are very ample. The [dual bundle](../../../fiber-bundle.md#dual-bundle) cancels the power of $A$, giving

$$
\boxed{L\cong H_1\otimes H_2^*.}
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Write $L\cong H_1\otimes H_2^*$ as in part (d). Each [very ample line bundle](../../../ringed-space.md#very-ample-line-bundle) is the pullback of $\mathcal O(1)$ under a projective embedding. A [hyperplane section](../../../cartier-divisor.md#hyperplane-section) therefore supplies an effective [divisor on a complex manifold](../../../complex-geometry.md#divisor-on-a-complex-manifold) $D_i$ with $H_i\cong\mathcal O(D_i)$. Hence

$$
L\cong\mathcal O(D_1-D_2).
$$

Every [Picard group](../../../ringed-space.md#picard-group) class is therefore in the image of the [divisor-to-Picard map](../../../complex-geometry.md#divisor-to-picard-map):

$$
\boxed{\operatorname{Div}(X)\longrightarrow\operatorname{Pic}(X)\text{ is surjective}.}
$$

## 4

↑ **Parent:** [Paper 118](paper-118.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle) is a complex-linear map $D:\Omega^0(E)\to\Omega^1(E)$ satisfying the [Leibniz rule](../../../calculus.md#leibniz-rule) $D(fs)=df\otimes s+fDs$. It is compatible with the [Hermitian metric on a holomorphic vector bundle](../../../complex-geometry.md#hermitian-metric-on-a-holomorphic-vector-bundle) $h$ when

$$
d\,h(s,t)=h(Ds,t)+h(s,Dt),
$$

and compatible with the holomorphic structure when its type-$(0,1)$ part is the [Dolbeault partial connection](../../../complex-geometry.md#dolbeault-partial-connection):

$$
\boxed{D^{0,1}=\bar\partial_E.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

In a unitary frame the metric matrix is $I$. If $A$ is the [connection one-form](../../../fiber-bundle.md#connection-one-form), [metric compatibility](../../../fiber-bundle.md#metric-compatibility) gives $0=dI=A^*+A$, so

$$
\boxed{A^*=-A;}
$$

the matrix is [Skew-Hermitian](../../../linear-operator-theory.md#skew-hermitian-matrix). In a [holomorphic local frame](../../../complex-geometry.md#holomorphic-local-trivialization), every frame vector is annihilated by $\bar\partial_E$, and compatibility with the holomorphic structure gives

$$
\boxed{A^{0,1}=0.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

In a [holomorphic local frame](../../../complex-geometry.md#holomorphic-local-trivialization) $e$, let $H=(h(e_i,e_j))$ and write $De=eA$. Holomorphic compatibility forces $A^{0,1}=0$, while [metric compatibility](../../../fiber-bundle.md#metric-compatibility) forces the [local formula for the Chern connection on a vector bundle](../../../complex-geometry.md#local-formula-for-the-chern-connection-on-a-vector-bundle)

$$
\boxed{A=H^{-1}\partial H.}
$$

This proves uniqueness. The formula transforms by the [connection one-form](../../../fiber-bundle.md#connection-one-form) law under a holomorphic frame change, so the local definitions glue and satisfy both conditions. This proves existence of the unique [Chern connection](../../../complex-geometry.md#chern-connection).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Let $D_1$ and $D_2$ each be a [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle). Their difference is tensorial, so $D_1=D_2+a$ with $a\in\Omega^1(\operatorname{End}E)$. Extend $D_2$ to the [endomorphism bundle connection](../../../fiber-bundle.md#endomorphism-bundle-connection). Expanding $(D_2+a)^2$ with the supplied graded [Leibniz rule](../../../calculus.md#leibniz-rule) gives the [curvature difference formula](../../../fiber-bundle.md#curvature-difference-formula)

$$
\boxed{F_{D_1}=F_{D_2}+D_2(a)+a\wedge a.}
$$

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Because the two [Chern connections](../../../complex-geometry.md#chern-connection) have the same $(0,1)$ part, $a=D_1-D_2$ has type $(1,0)$. The [curvature difference formula](../../../fiber-bundle.md#curvature-difference-formula) has only $(2,0)$ and $(1,1)$ parts. Both Chern curvatures have type $(1,1)$, so the total $(2,0)$ part vanishes. The remaining part is obtained from $D_2^{0,1}=\bar\partial_{\operatorname{End}E}$, proving the [curvature difference of two Chern connections](../../../complex-geometry.md#curvature-difference-of-two-chern-connections)

$$
\boxed{F_{D_1}-F_{D_2}=\bar\partial_{\operatorname{End}E}a.}
$$

## 5

↑ **Parent:** [Paper 118](paper-118.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For the [formal adjoints](../../../hilbert-space.md#formal-adjoint) $d^*$, $\partial^*$ and $\bar\partial^*$ defined by the [Kähler metric](../../../complex-geometry.md#kahler-metric),

$$
\boxed{\Delta_d=dd^*+d^*d,}
$$

and

$$
\boxed{\Delta_{\bar\partial}=\bar\partial\bar\partial^*+\bar\partial^*\bar\partial,\qquad
\Delta_\partial=\partial\partial^*+\partial^*\partial.}
$$

These are respectively the [Hodge Laplacian](../../../differential-form.md#hodge-laplacian) and the two Dolbeault Laplacians.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For the [Lefschetz operator of a Kähler manifold](../../../complex-geometry.md#lefschetz-operator-of-a-kahler-manifold) and its adjoint $\Lambda$, the [Kähler identities](../../../complex-geometry.md#kahler-identities) include

$$
[\Lambda,\partial]=i\bar\partial^*,\qquad [\Lambda,\bar\partial]=-i\partial^*.
$$

They make the mixed anticommutators in the expansion of $\Delta_d$ vanish and imply $\Delta_\partial=\Delta_{\bar\partial}$. Expanding $d=\partial+\bar\partial$ therefore proves the [Kähler Laplacian identity](../../../complex-geometry.md#kahler-laplacian-identity)

$$
\boxed{\Delta_d=2\Delta_{\bar\partial}=2\Delta_\partial.}
$$

Thus $\Delta_d\alpha=0$ exactly when $\Delta_{\bar\partial}\alpha=0$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The [Hodge decomposition theorem for compact Kähler manifolds](../../../complex-geometry.md#hodge-decomposition-theorem-for-compact-kahler-manifolds) gives a unique [harmonic differential form](../../../differential-form.md#harmonic-differential-form) representative of every complex [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) class, with a decomposition into harmonic pure-type components. Consequently

$$
\boxed{H^k_{dR}(X;\mathbb C)=\bigoplus_{p+q=k}H_{\bar\partial}^{p,q}(X).}
$$

Equivalently, the [Dolbeault Hodge decomposition on a compact Hermitian manifold](../../../complex-geometry.md#dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold) is

$$
\Omega^{p,q}=\mathcal H^{p,q}\oplus\bar\partial\Omega^{p,q-1}\oplus\bar\partial^*\Omega^{p,q+1}.
$$

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

If $\alpha=\partial\bar\partial\beta$ and $h\in\mathcal H^{p,q}$, the [Kähler Laplacian identity](../../../complex-geometry.md#kahler-laplacian-identity) makes $h$ both $\partial$- and $\bar\partial$-harmonic. Hence $\partial^*h=\bar\partial^*h=0$, and integration by parts gives $\langle\alpha,h\rangle=0$.

Conversely, let $d\alpha=0$ and $\alpha\perp\mathcal H^{p,q}$. Pure type gives $\partial\alpha=\bar\partial\alpha=0$. [Dolbeault Hodge decomposition](../../../complex-geometry.md#dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold) removes the harmonic and coexact components, so

$$
\alpha=\bar\partial\theta,\qquad\theta=\bar\partial^*\gamma.
$$

Now $\bar\partial(\partial\theta)=-\partial\alpha=0$, and the Kähler anticommutation identity gives $\bar\partial^*(\partial\theta)=-\partial(\bar\partial^*\theta)=0$. Thus $\partial\theta$ is $\bar\partial$-harmonic and therefore $\partial$-harmonic; being $\partial$-exact, it vanishes. Moreover $\theta\in\operatorname{im}\bar\partial^*$ is orthogonal to the common $\bar\partial$- and $\partial$-harmonic space. Its $\partial$-Hodge decomposition therefore gives $\theta=\partial\phi$. Hence

$$
\alpha=\bar\partial\partial\phi=-\partial\bar\partial\phi.
$$

Taking $\beta=-\phi$ proves the [harmonic orthogonality criterion for ddbar exactness](../../../complex-geometry.md#harmonic-orthogonality-criterion-for-ddbar-exactness)

$$
\boxed{\alpha=\partial\bar\partial\beta\Longleftrightarrow\alpha\perp\mathcal H^{p,q}(X).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
