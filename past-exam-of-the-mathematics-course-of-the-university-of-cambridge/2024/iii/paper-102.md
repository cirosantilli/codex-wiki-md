# Paper 102

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_102.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_102.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
    - [iii](#2/c/iii)
      - [Solution](#2/c/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
    - [iv](#3/b/iv)
      - [Solution](#3/b/iv/solution)
    - [v](#3/b/v)
      - [Solution](#3/b/v/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [i](#5/c/i)
      - [Solution](#5/c/i/solution)
    - [ii](#5/c/ii)
      - [Solution](#5/c/ii/solution)

## 1

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Write $e,h,f$ for the standard generators of the [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra). For the representation $\phi$, use the normalization

$$
\Omega=\phi(e)\phi(f)+\phi(f)\phi(e)+\frac12\phi(h)^2.
$$

This is the quadratic [Casimir element](../../../semisimple-lie-algebra.md#casimir-element), and by assumption it commutes with every $\phi(x)$.

[Schur lemma](../../../representation-theory.md#schur-s-lemma) says that an endomorphism of a finite-dimensional irreducible complex representation which commutes with the representation is a scalar. Hence $\Omega=cI_V$ when $V$ is irreducible.

Let $v$ be a [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-representation) of highest weight $m$, so $ev=0$ and $hv=mv$. Since $[e,f]=h$,

$$
efv=(fe+h)v=mv,
\qquad fev=0.
$$

Therefore

$$
\Omega v=\left(m+\frac12m^2\right)v
=\frac12m(m+2)v.
$$

It follows from scalarity that

$$
\boxed{\Omega=\frac12m(m+2)I_V}.
$$

This is the [Casimir eigenvalue for sl2](../../../semisimple-lie-algebra.md#casimir-eigenvalue-for-sl2) in the chosen normalization.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

The one-dimensional quotient $V/W$ is trivial because every one-dimensional representation vanishes on the [derived algebra](../../../lie-algebra.md#derived-series-of-a-lie-algebra) $[\mathfrak{sl}_2,\mathfrak{sl}_2]=\mathfrak{sl}_2$. Choose $v\in V$ mapping to $1\in V/W$. Then

$$
c(x)=xv\in W
$$

is a $1$-cocycle:

$$
c([x,y])=x,c(y)-y,c(x).
$$

We show that it is a coboundary.

Decompose $W$ into generalized eigenspaces of its [Casimir element](../../../semisimple-lie-algebra.md#casimir-element) $\Omega$. These are subrepresentations because $\Omega$ is central. On a generalized eigenspace with nonzero eigenvalue, $\Omega$ is invertible. If $(x_i)$ and $(x^i)$ are dual bases of $\mathfrak{sl}_2$ for the [Killing form](../../../lie-algebra.md#killing-form), put

$$
u=\sum_i x_i c(x^i).
$$

Invariance of the Killing form and the cocycle identity give the standard Casimir calculation

$$
x u=\Omega c(x).
$$

Thus on every nonzero generalized eigenspace, $c(x)=x(\Omega^{-1}u)$.

On the zero generalized eigenspace, every irreducible composition factor has zero Casimir eigenvalue. By part i and the [classification of finite-dimensional sl2 representations](../../../semisimple-lie-algebra.md#classification-of-finite-dimensional-sl2-representations), each such factor is trivial. In a basis adapted to a composition series, the image of $\mathfrak{sl}_2$ is therefore strictly upper triangular and hence solvable. Since $\mathfrak{sl}_2$ is simple and non-solvable, that image is zero. The cocycle then vanishes because it kills $[\mathfrak{sl}_2,\mathfrak{sl}_2]$.

Combining the generalized eigenspaces gives $w\in W$ such that $c(x)=xw$ for every $x$. Hence $v-w$ is invariant, and

$$
V=W\oplus\mathbb C(v-w)
$$

is a decomposition into subrepresentations. This proves the codimension-one case of the [Weyl complete reducibility theorem](../../../semisimple-lie-algebra.md#weyl-complete-reducibility-theorem).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The relation $[h,e]=2e$ forces $ew_i$ to have weight $a+2(i+1)$, so

$$
ew_i=c_iw_{i+1}
$$

for scalars $c_i$. The relation $[e,f]=h$ becomes

$$
(c_{i-1}-c_i)w_i=(a+2i)w_i.
$$

With $c_0=b$, this recurrence has the unique solution

$$
\boxed{c_i=b-ia-i(i+1)}
$$

for every $i\in\mathbb Z$. Direct substitution also verifies $[h,f]=-2f$ and $[h,e]=2e$, so these formulas define the unique required [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra) action. They form an [Intermediate-series sl2 module](../../../semisimple-lie-algebra.md#intermediate-series-sl2-module).

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Let $0\ne U\subseteq W$ be a subrepresentation and choose

$$
0\ne u=\sum_{r=p}^q a_rw_r\in U
$$

with finite support. The $h$-eigenvalues $a+2r$ are pairwise distinct. By [Lagrange interpolation](../../../numerical-analysis.md#lagrange-polynomial), there is a polynomial $P$ which is one at one chosen eigenvalue appearing in $u$ and zero at all the others. Then $P(h)u$ is a nonzero scalar multiple of one basis vector $w_i$. Since $U$ is invariant under $h$, it contains $w_i$.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

If

$$
b=ja+j(j+1),
$$

then the coefficient $c_j=b-ja-j(j+1)$ vanishes. Consequently

$$
U_j=\operatorname{span}\{w_i:i\leq j\}
$$

is stable under $h$, $f$, and $e$: the only raising operation that could leave it is $ew_j$, and that is zero. Thus $W$ is reducible.

Conversely, let $U$ be a nonzero subrepresentation. By part ii it contains some $w_i$, and repeated application of $f$ gives every $w_r$ with $r\leq i$. If every $c_r$ is nonzero, repeated application of $e$ also gives every $w_r$ with $r>i$, so $U=W$. Hence a proper nonzero subrepresentation exists exactly when some $c_j=0$, or

$$
\boxed{b=ja+j(j+1)\quad\text{for some }j\in\mathbb Z}.
$$

## 2

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a finite-dimensional [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) $\phi:\mathfrak g\to\mathfrak{gl}(V)$, the [Trace form of a Lie algebra representation](../../../lie-algebra.md#trace-form-of-a-lie-algebra-representation) is

$$
B_V(x,y)=\operatorname{tr}(\phi(x)\phi(y)).
$$

The [Killing form](../../../lie-algebra.md#killing-form) is the trace form of the [Adjoint representation of a Lie algebra](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra):

$$
\kappa(x,y)=\operatorname{tr}(\operatorname{ad}_x\operatorname{ad}_y).
$$

A bilinear form $B$ is $\mathfrak g$-invariant when

$$
B([z,x],y)+B(x,[z,y])=0,
$$

equivalently $B([x,y],z)=B(x,[y,z])$. For a trace form this follows from cyclicity of trace:

$$
\boxed{\operatorname{tr}([\phi(z),\phi(x)]\phi(y))
+\operatorname{tr}(\phi(x)[\phi(z),\phi(y)])=0.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use the nondegenerate restriction of the [Killing form](../../../lie-algebra.md#killing-form) to $\mathfrak t$ to define $t_\alpha\in\mathfrak t$ by

$$
\kappa(t_\alpha,t)=\alpha(t)
\qquad(t\in\mathfrak t).
$$

Killing-form invariance and the [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) show that $\mathfrak g_\alpha$ pairs nondegenerately with $\mathfrak g_{-\alpha}$ and orthogonally with every other root space. Choose nonzero $e\in\mathfrak g_\alpha$ and $f\in\mathfrak g_{-\alpha}$ with $\kappa(e,f)\ne0$. For $t\in\mathfrak t$,

$$
\kappa([e,f],t)=\kappa(e,[f,t])
=\alpha(t)\kappa(e,f),
$$

so

$$
[e,f]=\kappa(e,f)t_\alpha\ne0.
$$

We need $\alpha(t_\alpha)\ne0$. If it were zero, the span of $e,f,t_\alpha$ would be a solvable Heisenberg-type Lie algebra with central commutator $[e,f]$. By [Lie theorem](../../../lie-algebra.md#lie-s-theorem), its adjoint action on $\mathfrak g$ can be upper triangularized, so $\operatorname{ad}[e,f]$ is nilpotent. But $[e,f]\in\mathfrak t$, and elements of the [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) act semisimply; hence $\operatorname{ad}[e,f]=0$. A semisimple Lie algebra has zero center, contradicting $[e,f]\ne0$.

Set

$$
h_\alpha=\frac{2t_\alpha}{\alpha(t_\alpha)}.
$$

Rescale $f$ so that $[e_\alpha,f_\alpha]=h_\alpha$. Since $e_\alpha$ and $f_\alpha$ lie in the $\alpha$ and $-\alpha$ root spaces,

$$
[h_\alpha,e_\alpha]=2e_\alpha,
\qquad
[h_\alpha,f_\alpha]=-2f_\alpha.
$$

**Thus $\mathfrak m_\alpha=\langle e_\alpha,h_\alpha,f_\alpha\rangle$ is the [sl2 subalgebra associated with a root](../../../semisimple-lie-algebra.md#sl2-subalgebra-associated-with-a-root).**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

Bilinearity and alternatingness of

$$
[(x,v),(y,w)]=([x,y],xw-yv)
$$

are immediate. For three elements, the $\mathfrak g$ component of the Jacobi sum vanishes by the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) in $\mathfrak g$. In the $V$ component, the coefficient of a vector such as $u$ is

$$
[x,y]u-x(yu)+y(xu)=0
$$

because the action is a [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation); the other terms cancel cyclically in the same way. Hence the bracket satisfies Jacobi and defines the [semidirect product of a Lie algebra and a module](../../../lie-algebra.md#semidirect-product-of-a-lie-algebra-and-a-module) $\mathfrak g\ltimes V$.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

Let $\mathfrak g=\mathfrak{sl}_2(\mathbb C)$ and let $V=\mathbb C^2$ be its defining irreducible representation. Set

$$
\mathfrak h=\mathfrak g\ltimes V.
$$

Since $[\mathfrak g,\mathfrak g]=\mathfrak g$ and $\mathfrak gV=V$,

$$
[\mathfrak h,\mathfrak h]=\mathfrak g\oplus V=\mathfrak h.
$$

If $(x,v)$ is central, commuting with every $(0,w)$ gives $xw=0$ for all $w$, so faithfulness of the defining representation gives $x=0$. Commuting with every $(y,0)$ then gives $yv=0$ for all $y$; irreducibility and nontriviality give $v=0$. Thus $Z(\mathfrak h)=0$.

The nonzero abelian subspace $V$ is a proper [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra), so $\mathfrak h$ is not simple. It is not a direct product of simple Lie algebras either, because such a product is semisimple and has no nonzero solvable ideal, whereas $V$ is one.

<h4 id="2/c/iii">iii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/c/iii)

Relative to $\mathfrak g\oplus V$, the adjoint action has block form

$$
\operatorname{ad}_{(x,v)}=
\begin{pmatrix}
\operatorname{ad}_x&0\\
(y\mapsto-yv)&\phi(x)
\end{pmatrix}.
$$

Multiplying two such block-triangular matrices and taking the trace gives

$$
\boxed{
K((x,v),(y,w))
=\kappa(x,y)+\operatorname{tr}(\phi(x)\phi(y))},
$$

the [Killing form of a semidirect product with a module](../../../lie-algebra.md#killing-form-of-a-semidirect-product-with-a-module). It does not depend on $v$ or $w$, so $V$ lies in its radical. Therefore $K$ can be nondegenerate only if $V=0$. In that case $K=\kappa$, which is nondegenerate exactly when $\mathfrak g$ is semisimple by the [Cartan criterion for semisimplicity](../../../lie-algebra.md#cartan-criterion-for-semisimplicity). Thus

$$
\boxed{K\text{ is nondegenerate iff }V=0\text{ and }\mathfrak g\text{ is semisimple}.}
$$

## 3

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

A [Weyl chamber](../../../semisimple-lie-algebra.md#fundamental-chamber-of-a-root-system) is a connected component of

$$
E\setminus\bigcup_{\alpha\in\Phi}\alpha^\perp.
$$

A [root basis](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system) $\Delta\subseteq\Phi$ is a vector-space basis of $E$ such that every root is an integer combination of elements of $\Delta$ with all nonzero coefficients of one sign.

To construct one, choose a regular vector $\gamma\in E$, meaning $(\gamma,\alpha)\ne0$ for every root. Declare

$$
\Phi_\gamma^+=\{\alpha\in\Phi:(\gamma,\alpha)>0\}.
$$

The positive roots in $\Phi_\gamma^+$ which cannot be written as sums of two positive roots form a root basis $\Delta_\gamma$. Vectors $\gamma$ in the same Weyl chamber give the same basis.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Write a positive nonsimple root as

$$
\alpha=\sum_{\beta\in\Delta}n_\beta\beta,
\qquad n_\beta\geq0.
$$

If $(\alpha,\beta)\leq0$ for every simple root with $n_\beta>0$, then

$$
(\alpha,\alpha)=\sum_\beta n_\beta(\alpha,\beta)\leq0,
$$

which is impossible. Hence $(\alpha,\beta)>0$ for some simple $\beta$. The root-string property then gives $\alpha-\beta\in\Phi$, and its simple-root coefficients remain nonnegative. This is the [simple-root subtraction lemma](../../../semisimple-lie-algebra.md#simple-root-subtraction-lemma).

Induct on the height $\sum n_\beta$. Applying the induction hypothesis to $\alpha-\beta$ and appending $\beta$ writes

$$
\alpha=\alpha_1+\cdots+\alpha_k
$$

so that every partial sum is a root.

Finally let $\alpha$ be simple and let $\gamma\ne\alpha$ be positive. In the simple-root expansion of

$$
s_\alpha(\gamma)=\gamma-
\langle\gamma,\alpha^\vee\rangle\alpha,
$$

all coefficients except possibly that of $\alpha$ are unchanged, and at least one of those unchanged coefficients is positive. Since a root has coefficients all of one sign, the image cannot be negative. Thus $s_\alpha$ permutes $\Phi^+\setminus\{\alpha\}$, as stated by [action of a simple reflection on positive roots](../../../semisimple-lie-algebra.md#action-of-a-simple-reflection-on-positive-roots).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

The diagonal [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) consists of

$$
\operatorname{diag}(t_1,t_2,t_3,-t_1,-t_2,-t_3).
$$

Let $\varepsilon_i\in\mathfrak t^*$ read off $t_i$. The roots are

$$
\boxed{
\Phi=\{\pm\varepsilon_i\pm\varepsilon_j:
1\leq i<j\leq3\}},
$$

the [D3 root system](../../../semisimple-lie-algebra.md#d3-root-system).

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

One root basis is

$$
\alpha_1=\varepsilon_1-\varepsilon_2,
\qquad
\alpha_2=\varepsilon_2-\varepsilon_3,
\qquad
\alpha_3=\varepsilon_2+\varepsilon_3.
$$

All roots have the same length. The nonzero inner products are $(\alpha_1,\alpha_2)=(\alpha_1,\alpha_3)=-1$, so the labeled [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) is

$$
\alpha_2\;\text{---}\;\alpha_1\;\text{---}\;\alpha_3.
$$

It is the three-node $A_3$ diagram.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

The simple reflections act on the root basis by

$$
\begin{array}{c|ccc}
&\alpha_1&\alpha_2&\alpha_3\\ \hline
s_{\alpha_1}&-\alpha_1&\alpha_2+\alpha_1&\alpha_3+\alpha_1\\
s_{\alpha_2}&\alpha_1+\alpha_2&-\alpha_2&\alpha_3\\
s_{\alpha_3}&\alpha_1+\alpha_3&\alpha_2&-\alpha_3
\end{array}
$$

by the [Weyl reflection](../../../semisimple-lie-algebra.md#weyl-reflection) formula $s_\alpha(\beta)=\beta-\langle\beta,\alpha^\vee\rangle\alpha$.

<h4 id="3/b/iv">iv</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/b/iv)

The linear map

$$
\varepsilon_1\mapsto\varepsilon_1,
\qquad
\varepsilon_2\mapsto\varepsilon_2,
\qquad
\varepsilon_3\mapsto-\varepsilon_3
$$

preserves $\Phi$ and exchanges $\alpha_2$ with $\alpha_3$ while fixing $\alpha_1$. It is not in the $D_3$ [Weyl group](../../../semisimple-lie-algebra.md#weyl-group), whose signed permutations change an even number of signs. Thus it is an outer automorphism of the root system.

<h4 id="3/b/v">v</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/v/solution">Solution</h5>

↑ **Parent:** [V](#3/b/v)

The preceding [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) identifies the root system $D_3$ with $A_3$. The classification of finite-dimensional complex [simple Lie algebras](../../../semisimple-lie-algebra.md#simple-lie-algebra) by connected Dynkin diagrams therefore gives

$$
\boxed{\mathfrak{so}_6(\mathbb C)\cong\mathfrak{sl}_4(\mathbb C)}.
$$

This is the [Isomorphism between so6 and sl4](../../../semisimple-lie-algebra.md#isomorphism-between-so6-and-sl4). Both algebras have dimension $15$, consistently with the classification.

## 4

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The crystallographic axiom makes

$$
m=\langle\alpha,\beta^\vee\rangle,
\qquad
n=\langle\beta,\alpha^\vee\rangle
$$

integers. If $\theta$ is the angle between the roots, then

$$
mn=
\frac{2(\alpha,\beta)}{(\beta,\beta)}
\frac{2(\beta,\alpha)}{(\alpha,\alpha)}
=4\cos^2\theta.
$$

This is a nonnegative integer. Since $\beta\ne\pm\alpha$, the roots are not parallel, so $\cos^2\theta<1$. Therefore

$$
\boxed{mn\in\{0,1,2,3\}},
$$

which is the [root-system finiteness lemma](../../../semisimple-lie-algebra.md#root-system-finiteness-lemma).

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Choose simple roots $\alpha,\beta$. Their inner product is nonpositive, so their angle lies in $[\pi/2,\pi)$. Part i leaves four possibilities for $mn$:

- $mn=0$: angle $\pi/2$, giving $A_1\times A_1$.
- $mn=1$: angle $2\pi/3$ and equal root lengths, giving $A_2$.
- $mn=2$: angle $3\pi/4$ and squared-length ratio $2$, giving $B_2$.
- $mn=3$: angle $5\pi/6$ and squared-length ratio $3$, giving $G_2$.

The root strings generated by the two simple reflections produce exactly the roots in those four standard systems. Hence these are all possibilities, proving the [classification of rank-two root systems](../../../semisimple-lie-algebra.md#classification-of-rank-two-root-systems).

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

An irreducible root system is [simply laced](../../../semisimple-lie-algebra.md#simply-laced-root-system) when every root has the same length, equivalently when its [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) has no multiple edge.

If all roots have the same length, the two Cartan integers for $\alpha$ and $\beta$ are equal. The [root-system finiteness lemma](../../../semisimple-lie-algebra.md#root-system-finiteness-lemma) then makes their product either zero or one, so

$$
\langle\alpha,\beta^\vee\rangle\in\{0,\pm1\}
$$

for $\alpha\ne\pm\beta$.

Conversely, when all such Cartan integers lie in $\{0,\pm1\}$, any two nonorthogonal roots have Cartan integers of absolute value one in both directions. Their squared lengths are therefore equal. Irreducibility makes the graph joining nonorthogonal roots connected, so all roots have the same length. Thus the system is simply laced.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

On $P=\operatorname{span}\{\alpha,\beta\}$, each $s_\alpha$ is reflection in the line $\alpha^\perp\cap P$. The product of two plane reflections is a rotation. If $\theta$ is the oriented angle from $\beta$ to $\alpha$, then

$$
s_\alpha s_\beta
$$

rotates through $2\theta$ modulo $2\pi$.

If this rotation has order $m$, conjugation by either reflection inverts it. Hence

$$
\langle s_\alpha,s_\beta\rangle
=\langle r,s:r^m=s^2=1, srs=r^{-1}\rangle
$$

is a [dihedral group](../../../finite-group-theory.md#dihedral-group), with rotational subgroup $\langle r\rangle=\langle s_\alpha s_\beta\rangle$.

For the simple-root angles from part ii, the rotation orders and Weyl groups are

$$
\begin{array}{c|c|c}
\text{type}&m&|W|\\ \hline
A_1\times A_1&2&4\\
A_2&3&6\\
B_2&4&8\\
G_2&6&12.
\end{array}
$$

These are the [rank-two Weyl groups](../../../semisimple-lie-algebra.md#weyl-group-of-a-rank-two-root-system).

## 5

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

Choose a [Borel subalgebra](../../../semisimple-lie-algebra.md#borel-subalgebra) $\mathfrak b=\mathfrak t\oplus\mathfrak n^+$. For $\lambda\in\mathfrak t^*$, let $\mathbb C_\lambda$ be the one-dimensional $\mathfrak b$-module on which $\mathfrak n^+$ acts by zero and $h\in\mathfrak t$ acts by $\lambda(h)$. The [Verma module](../../../semisimple-lie-algebra.md#verma-module) is

$$
M(\lambda)=U(\mathfrak g)\otimes_{U(\mathfrak b)}\mathbb C_\lambda.
$$

Its [universal property of a Verma module](../../../semisimple-lie-algebra.md#universal-property-of-a-verma-module) says that any vector of weight $\lambda$ annihilated by $\mathfrak n^+$ receives the canonical highest-weight vector under one unique module homomorphism from $M(\lambda)$.

The sum of the proper submodules of $M(\lambda)$ is its unique maximal proper submodule, because no proper submodule contains the highest-weight vector. Its quotient $V(\lambda)$ is therefore the unique [irreducible quotient of a Verma module](../../../semisimple-lie-algebra.md#irreducible-quotient-of-a-verma-module), and hence the unique irreducible highest-weight module of weight $\lambda$.

The module $V(\lambda)$ is finite-dimensional exactly when $\lambda$ is a [dominant integral weight](../../../semisimple-lie-algebra.md#dominant-integral-weight):

$$
\langle\lambda,\alpha_i^\vee\rangle\in\mathbb Z_{\geq0}
$$

for every simple root $\alpha_i$.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

For $\mathfrak{sl}_2$, the Verma module has basis

$$
v,,fv,,f^2v,\ldots
$$

by the [Poincaré-Birkhoff-Witt theorem](../../../lie-algebra.md#poincare-birkhoff-witt-theorem). If $hv=\lambda v$, then

$$
e f^rv=r(\lambda-r+1)f^{r-1}v.
$$

For $\lambda=-d$ with $d>0$, the coefficient is

$$
r(-d-r+1)\ne0
$$

for every $r\geq1$. Thus no $f^rv$ with $r>0$ is a [singular vector](../../../semisimple-lie-algebra.md#singular-vector).

Any nonzero submodule contains a weight vector $f^rv$ because the $h$-weights are distinct. Applying $e^r$ gives a nonzero multiple of $v$, after which applying powers of $f$ generates all of $M(-d)$. Hence

$$
\boxed{M(-d)\text{ is irreducible and infinite-dimensional}.}
$$

This is also the negative-highest-weight case of [Reducibility of an sl2 Verma module](../../../semisimple-lie-algebra.md#reducibility-of-an-sl2-verma-module).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For a dominant integral weight $\lambda$, the [Weyl character formula](../../../semisimple-lie-algebra.md#weyl-character-formula) is

$$
\operatorname{ch}V(\lambda)=
\frac{\sum_{w\in W}(-1)^{\ell(w)}e^{w(\lambda+\rho)}}
{\sum_{w\in W}(-1)^{\ell(w)}e^{w\rho}},
$$

where $W$ is the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group), $\ell$ is [Coxeter length](../../../semisimple-lie-algebra.md#coxeter-length), and $\rho$ is the [half-sum of positive roots](../../../semisimple-lie-algebra.md#half-sum-of-positive-roots). The [Weyl denominator formula](../../../semisimple-lie-algebra.md#weyl-denominator-formula) is

$$
\sum_{w\in W}(-1)^{\ell(w)}e^{w\rho}
=e^\rho\prod_{\alpha\in\Phi^+}(1-e^{-\alpha}).
$$

Set $\lambda=k\rho$. Apply the denominator identity after replacing every formal exponential $e^\mu$ by $e^{(k+1)\mu}$:

$$
\sum_w(-1)^{\ell(w)}e^{w((k+1)\rho)}
=e^{(k+1)\rho}
\prod_{\alpha\in\Phi^+}(1-e^{-(k+1)\alpha}).
$$

Dividing this by the ordinary denominator gives

$$
\begin{aligned}
\operatorname{ch}V(k\rho)
&=e^{k\rho}\prod_{\alpha\in\Phi^+}
\frac{1-e^{-(k+1)\alpha}}{1-e^{-\alpha}}\\
&=\boxed{e^{k\rho}\prod_{\alpha\in\Phi^+}
(1+e^{-\alpha}+\cdots+e^{-k\alpha})}.
\end{aligned}
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/i">i</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/i/solution">Solution</h5>

↑ **Parent:** [I](#5/c/i)

Realize the [B2 root system](../../../semisimple-lie-algebra.md#b2-root-system) in $\mathbb R^2$ as

$$
\{\pm\varepsilon_1,\pm\varepsilon_2,
\pm\varepsilon_1\pm\varepsilon_2\}.
$$

Choose the short simple root and long simple root

$$
\alpha_1=\varepsilon_2,
\qquad
\alpha_2=\varepsilon_1-\varepsilon_2.
$$

Then

$$
\omega_1=\frac12(\varepsilon_1+\varepsilon_2),
\qquad
\omega_2=\varepsilon_1,
$$

as follows from $\langle\omega_i,\alpha_j^\vee\rangle=\delta_{ij}$. The roots form a square from the long roots with the four short roots on the coordinate axes; the double edge in the Dynkin diagram points toward $\alpha_1$.

The positive roots are

$$
\alpha_1,quad\alpha_2,quad
\alpha_1+\alpha_2,quad2\alpha_1+\alpha_2.
$$

For $\lambda=a\omega_1+b\omega_2$, substituting their coroot pairings in the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) gives

$$
\boxed{
\dim V(\lambda)=
\frac{(a+1)(b+1)(a+b+2)(a+2b+3)}6}.
$$

This is the [Weyl dimension formula for B2](../../../semisimple-lie-algebra.md#weyl-dimension-formula-for-b2).

<h4 id="5/c/ii">ii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/c/ii)

The weights of the defining five-dimensional representation are

$$
\varepsilon_1,\ \varepsilon_2,\ 0,\ -\varepsilon_2,\ -\varepsilon_1.
$$

Its highest weight is $\varepsilon_1=\omega_2$, so irreducibility identifies it as

$$
V\cong V(\omega_2).
$$

If $v_+$ is a highest-weight vector, then $v_+\otimes v_+$ is a highest-weight vector of weight $2\omega_2$ in $V\otimes V$. The subrepresentation it generates is therefore $V(2\omega_2)$. Equivalently, it is the [Traceless symmetric square of the defining so5 representation](../../../semisimple-lie-algebra.md#traceless-symmetric-square-of-the-defining-so5-representation); the invariant quadratic form supplies the complementary trivial line in $S^2V$.

Putting $a=0$ and $b=2$ into the formula from part i gives

$$
\boxed{
\dim V(2\omega_2)
=\frac{(1)(3)(4)(7)}6=14}.
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
