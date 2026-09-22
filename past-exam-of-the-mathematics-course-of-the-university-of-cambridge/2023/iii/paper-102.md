# Paper 102

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_102.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_102.pdf)

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
  - [v](#1/v)
    - [Solution](#1/v/solution)
  - [vi](#1/vi)
    - [Solution](#1/vi/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For an [affine algebraic group](../../../lie-theory.md#linear-algebraic-group) $G$, its [Lie algebra](../../../lie-algebra.md) is the [tangent space](../../../differential-geometry.md#tangent-space) at the identity,

$$
\mathfrak g=T_eG.
$$

Equivalently, it is the space of left-invariant derivations of the [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) $\mathbb C[G]$. The [Lie bracket](../../../lie-algebra.md#lie-bracket) is the commutator of derivations,

$$
[X,Y]=XY-YX.
$$

It is antisymmetric because $[Y,X]=-[X,Y]$. Associativity of composition gives

$$
[X,[Y,Z]]+[Y,[Z,X]]+[Z,[X,Y]]=0
$$

after all six triple products cancel in pairs, proving the [Jacobi identity](../../../lie-algebra.md#jacobi-identity). This construction is the [Lie algebra of an affine algebraic group](../../../lie-theory.md#lie-algebra-of-an-affine-algebraic-group).

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The distinct affine algebraic groups

$$
SL_2(\mathbb C)
\quad\text{and}\quad
PGL_2(\mathbb C)=SL_2(\mathbb C)/\{\pm I\}
$$

both have the [special linear Lie algebra](../../../semisimple-lie-algebra.md#special-linear-lie-algebra) $\mathfrak{sl}_2(\mathbb C)$. Quotienting a [Lie group](../../../lie-theory.md#lie-group) by a discrete central subgroup does not change its tangent Lie algebra.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

The finite-dimensional irreducible rational representations of $SL_2(\mathbb C)$ are

$$
V_n=\operatorname{Sym}^n(\mathbb C^2),\qquad n\geq0,
$$

of dimension $n+1$. The central element $-I$ acts on $V_n$ by $(-1)^n$. Therefore precisely the even-indexed representations

$$
V_{2m},\qquad m\geq0,
$$

descend to irreducible representations of $PGL_2(\mathbb C)$. This is the [Descent of an irreducible SL2 representation to PGL2](../../../lie-theory.md#descent-of-an-irreducible-sl2-representation-to-pgl2).

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

A bilinear form $B$ on a [Lie algebra](../../../lie-algebra.md) is [invariant](../../../lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra) when

$$
B([x,y],z)=B(x,[y,z]),
$$

equivalently $B([x,y],z)+B(y,[x,z])=0$.

Choose a basis $(x_i)$ of $\mathfrak g$ and its $B$-dual basis $(x^i)$. The [Casimir element](../../../semisimple-lie-algebra.md#casimir-element) is

$$
\Omega=\sum_i x_ix^i\in U(\mathfrak g),
$$

where $U(\mathfrak g)$ is the [universal enveloping algebra](../../../lie-algebra.md#universal-enveloping-algebra). The tensor $\sum_i x_i\otimes x^i$ corresponds under $B:\mathfrak g\cong\mathfrak g^*$ to the identity endomorphism, so invariance of $B$ makes it fixed by the diagonal adjoint action. Applying multiplication $U(\mathfrak g)\otimes U(\mathfrak g)\to U(\mathfrak g)$ gives

$$
[x,\Omega]=0
$$

for every $x\in\mathfrak g$. Thus $\Omega$ lies in the [center of an associative algebra](../../../associative-algebra.md#center-of-an-associative-algebra) of $U(\mathfrak g)$.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

Use the standard basis

$$
e=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad
f=\begin{pmatrix}0&0\\1&0\end{pmatrix},\qquad
h=\begin{pmatrix}1&0\\0&-1\end{pmatrix}
$$

of $\mathfrak{sl}_2$. For the invariant [trace form](../../../lie-algebra.md#trace-form-of-a-lie-algebra-representation) $B(x,y)=\operatorname{tr}(xy)$, the dual basis is $(f,e,h/2)$, so

$$
\Omega=ef+fe+\frac12h^2.
$$

On a highest-weight vector $v$ in the $(n+1)$-dimensional irreducible module, $ev=0$ and $hv=nv$. Since $efv=[e,f]v=n v$ and $fev=0$,

$$
\Omega v=\left(n+\frac{n^2}{2}\right)v
=\frac{n(n+2)}2v.
$$

Centrality and [Schur lemma](../../../representation-theory.md#schur-s-lemma) make this the eigenvalue on the whole module. Thus $\lambda=n(n+2)/2$, the [Casimir eigenvalue for sl2](../../../semisimple-lie-algebra.md#casimir-eigenvalue-for-sl2). If the form is instead the [Killing form](../../../lie-algebra.md#killing-form), which is four times the trace form on $\mathfrak{sl}_2$, the corresponding Casimir and eigenvalue are divided by four.

<h3 id="1/vi">vi</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#1/vi)

**No.** Let $\mathfrak g=\mathfrak{sl}_2$, let $\mathfrak s=\mathbb Ce$ be the one-dimensional subalgebra generated by the standard raising operator, and let $L=\mathbb C^2$ be the irreducible defining representation. On restriction to $\mathfrak s$, the element $e$ acts by a nonzero [Nilpotent Jordan block](../../../linear-operator-theory.md#nilpotent-jordan-block). A direct sum of irreducible representations of the one-dimensional abelian Lie algebra would make $e$ diagonalizable, so this restriction is not completely reducible. The [complete reducibility of semisimple Lie algebra representations](../../../semisimple-lie-algebra.md#weyl-s-theorem-on-complete-reducibility) applies when the restricting algebra is semisimple, which $\mathfrak s$ is not.

## 2

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The [Cartan solvability criterion](../../../lie-algebra.md#cartan-solvability-criterion) states that a finite-dimensional complex Lie algebra $\mathfrak g$ is solvable exactly when

$$
\kappa(\mathfrak g,[\mathfrak g,\mathfrak g])=0,
$$

where $\kappa$ is the [Killing form](../../../lie-algebra.md#killing-form). In the matrix form of the criterion, a Lie subalgebra $\mathfrak g\subseteq\mathfrak{gl}(V)$ is solvable if

$$
\operatorname{tr}(xy)=0
$$

for all $x\in[\mathfrak g,\mathfrak g]$ and $y\in\mathfrak g$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

A torus $\mathfrak t$ in a Lie algebra is an abelian subalgebra whose elements act semisimply in the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra). Its [weight-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) is

$$
\mathfrak g=\bigoplus_{\gamma\in\mathfrak t^*}\mathfrak g_\gamma,\qquad
\mathfrak g_\gamma=\{x:[t,x]=\gamma(t)x\text{ for every }t\in\mathfrak t\}.
$$

Invariance of the nondegenerate [Trace form of a Lie algebra representation](../../../lie-algebra.md#trace-form-of-a-lie-algebra-representation) gives

$$
(\mathfrak g_\gamma,\mathfrak g_\delta)_V=0
\quad\text{unless}\quad \gamma+\delta=0.
$$

Nondegeneracy therefore forces $\beta=-\alpha$. The standard [sl2 subalgebra associated with a root](../../../semisimple-lie-algebra.md#sl2-subalgebra-associated-with-a-root) argument gives one-dimensional opposite root spaces with vectors $e\in\mathfrak g_\alpha$, $f\in\mathfrak g_{-\alpha}$ and $h_\alpha\in\mathfrak t$ satisfying

$$
[h_\alpha,e]=2e,\qquad [h_\alpha,f]=-2f,\qquad[e,f]=h_\alpha.
$$

Their span is a copy of $\mathfrak{sl}_2$.

Set

$$
\mathfrak h=\ker(\alpha:\mathfrak t\to\mathbb C).
$$

Then $\dim\mathfrak h=\dim\mathfrak t-1$, $\mathfrak t=\mathbb Ch_\alpha\oplus\mathfrak h$, and every element of $\mathfrak h$ commutes with $e$, $f$, and $\mathfrak t$. Hence $\mathfrak h$ is abelian and

$$
\mathfrak g=\mathfrak{sl}_2\oplus\mathfrak h
$$

as a direct sum of commuting Lie algebras. This is the [two-root decomposition with a nondegenerate trace form](../../../semisimple-lie-algebra.md#two-root-decomposition-with-a-nondegenerate-trace-form).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Let $r=\dim\mathfrak h$ and choose a dual basis of weights $\varepsilon_1,\ldots,\varepsilon_r\in\mathfrak h^*$. Take

$$
V=\mathbb C^2\oplus\bigoplus_{i=1}^r(\mathbb C_{\varepsilon_i}\oplus\mathbb C_{-\varepsilon_i}).
$$

The $\mathfrak{sl}_2$ factor acts in its defining representation on $\mathbb C^2$ and trivially on the other summands; $\mathfrak h$ acts trivially on $\mathbb C^2$ and by the displayed characters on the one-dimensional summands. The resulting trace form is the nondegenerate trace form on $\mathfrak{sl}_2$, is

$$
2\sum_i\varepsilon_i(x)\varepsilon_i(y)
$$

on $\mathfrak h$, and has zero cross terms. It is therefore nondegenerate on $\mathfrak{sl}_2\oplus\mathfrak h$.

## 3

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Write an element of the diagonal torus as

$$
\operatorname{diag}(t_1,\ldots,t_n,-t_n,\ldots,-t_1)
$$

and let $\varepsilon_i$ extract $t_i$. The [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) is

$$
\mathfrak{so}_{2n}
=\mathfrak t\oplus
\bigoplus_{1\leq i<j\leq n}
\left(
\mathfrak g_{\varepsilon_i-\varepsilon_j}\oplus
\mathfrak g_{\varepsilon_i+\varepsilon_j}\oplus
\mathfrak g_{-\varepsilon_i+\varepsilon_j}\oplus
\mathfrak g_{-\varepsilon_i-\varepsilon_j}
\right),
$$

with one-dimensional root spaces. Thus the $D_n$ [root system](../../../semisimple-lie-algebra.md#root-system) is

$$
R=\{\pm\varepsilon_i\pm\varepsilon_j:i<j\}.
$$

The upper-triangular choice gives

$$
R^+=\{\varepsilon_i-\varepsilon_j,\ \varepsilon_i+\varepsilon_j:i<j\}.
$$

A compatible simple system is

$$
\alpha_i=\varepsilon_i-\varepsilon_{i+1}\quad(1\leq i<n),\qquad
\alpha_n=\varepsilon_{n-1}+\varepsilon_n.
$$

The [highest root](../../../semisimple-lie-algebra.md#highest-root) and [Weyl vector](../../../semisimple-lie-algebra.md#half-sum-of-positive-roots) are

$$
\theta=\varepsilon_1+\varepsilon_2
=\alpha_1+2\alpha_2+\cdots+2\alpha_{n-2}+\alpha_{n-1}+\alpha_n,
\qquad
\rho=\sum_{i=1}^n(n-i)\varepsilon_i.
$$

The [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight) are

$$
\omega_k=\varepsilon_1+\cdots+\varepsilon_k\quad(1\leq k\leq n-2),
$$



$$
\omega_{n-1}=\frac12(\varepsilon_1+\cdots+\varepsilon_{n-1}-\varepsilon_n),
\qquad
\omega_n=\frac12(\varepsilon_1+\cdots+\varepsilon_n).
$$

Using the paper's letters, the root lattice and weight lattice are respectively

$$
P=\left\{(a_i)\in\mathbb Z^n:\sum_i a_i\ \text{is even}\right\},
\qquad
Q=\mathbb Z^n\cup\left(\mathbb Z+\frac12\right)^n.
$$

Their quotient is

$$
Q/P\cong
\begin{cases}
\mathbb Z/2\mathbb Z\times\mathbb Z/2\mathbb Z,&n\text{ even},\\
\mathbb Z/4\mathbb Z,&n\text{ odd}.
\end{cases}
$$

The [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) is the $D_n$ diagram: a chain $\alpha_1-\cdots-\alpha_{n-2}$ whose last node is joined to both $\alpha_{n-1}$ and $\alpha_n$. The [Extended Dynkin diagram](../../../semisimple-lie-algebra.md#extended-dynkin-diagram) adds $\alpha_0=-\theta$ joined to $\alpha_2$. For $D_4$, the central node $\alpha_2$ consequently has the four leaves $\alpha_0,\alpha_1,\alpha_3,\alpha_4$.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Let $V=\mathbb C^4$. The [special linear Lie algebra](../../../semisimple-lie-algebra.md#special-linear-lie-algebra) $\mathfrak{sl}(V)$ acts on $\Lambda^2V$. The wedge product

$$
\Lambda^2V\times\Lambda^2V\longrightarrow\Lambda^4V\cong\mathbb C
$$

is a nondegenerate symmetric bilinear form, and the action preserves it because $\mathfrak{sl}(V)$ acts trivially on $\Lambda^4V$. This gives an injective homomorphism

$$
\mathfrak{sl}_4\longrightarrow\mathfrak{so}(\Lambda^2V)\cong\mathfrak{so}_6.
$$

Both Lie algebras have dimension $15$, so the map is an isomorphism. This realizes the [Isomorphism between so6 and sl4](../../../semisimple-lie-algebra.md#isomorphism-between-so6-and-sl4).

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

For every root, the [Weyl reflection](../../../semisimple-lie-algebra.md#weyl-reflection) is

$$
s_\alpha(x)=x-\frac{2(x,\alpha)}{(\alpha,\alpha)}\alpha.
$$

For $\alpha=\varepsilon_i-\varepsilon_j$, it swaps the $i$th and $j$th coordinates. For $\alpha=\varepsilon_i+\varepsilon_j$, it sends

$$
(x_i,x_j)\longmapsto(-x_j,-x_i)
$$

and fixes all other coordinates. The [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) of $D_n$ is therefore the group of signed permutations with an even number of sign changes,

$$
\boxed{W(D_n)\cong(\mathbb Z/2\mathbb Z)^{n-1}\rtimes S_n.}
$$

## 4

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

For a dominant integral weight $\lambda$, the [Weyl character formula](../../../semisimple-lie-algebra.md#weyl-character-formula) is

$$
\operatorname{ch}L_\lambda=
\frac{\sum_{w\in W}(-1)^{\ell(w)}e^{w(\lambda+\rho)}}
{\sum_{w\in W}(-1)^{\ell(w)}e^{w\rho}}.
$$

Here $W$ is the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group), $\ell(w)$ its [Coxeter length](../../../semisimple-lie-algebra.md#coxeter-length), $\rho$ the [Weyl vector](../../../semisimple-lie-algebra.md#half-sum-of-positive-roots), and $\operatorname{ch}$ the [formal character of a weight module](../../../semisimple-lie-algebra.md#formal-character-of-a-weight-module). Taking the limit at the identity gives the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula)

$$
\boxed{\dim L_\lambda=
\prod_{\alpha\in R^+}
\frac{\langle\lambda+\rho,\alpha^\vee\rangle}
{\langle\rho,\alpha^\vee\rangle}.}
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Choose a short simple root $\alpha_1$ and a long simple root $\alpha_2$. The [G2 root system](../../../semisimple-lie-algebra.md#g2-root-system) has positive roots

$$
\alpha_1,\ \alpha_2,\ \alpha_1+\alpha_2,\ 2\alpha_1+\alpha_2,\ 3\alpha_1+\alpha_2,\ 3\alpha_1+2\alpha_2.
$$

The two hexagons formed by the short and long roots give the usual twelve-root diagram. The fundamental weights are

$$
\omega_1=2\alpha_1+\alpha_2,\qquad
\omega_2=3\alpha_1+2\alpha_2.
$$

The second is the highest root, so the irreducible module $L(\omega_2)$ is the [Adjoint representation of a Lie algebra](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra).

The seven weights of $L(\omega_1)$ are zero and the six short roots, each with multiplicity one. Its [crystal](../../../semisimple-lie-algebra.md#crystal-basis), with arrows denoting the lowering operators $\widetilde f_i$, is the chain

$$
\omega_1
\xrightarrow{1}\alpha_1+\alpha_2
\xrightarrow{2}\alpha_1
\xrightarrow{1}0
\xrightarrow{1}-\alpha_1
\xrightarrow{2}-(\alpha_1+\alpha_2)
\xrightarrow{1}-\omega_1.
$$

Applying the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) to $\lambda=n_1\omega_1+n_2\omega_2$ gives

$$
\boxed{\dim L(\lambda)=\frac1{120}
(n_1+1)(n_2+1)(n_1+n_2+2)(n_1+2n_2+3)
(n_1+3n_2+4)(2n_1+3n_2+5).}
$$

## 5

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

For type $B_n$, the [spinor representation](../../../semisimple-lie-algebra.md#spin-representation) has highest weight

$$
\omega_n=\frac12(\varepsilon_1+\cdots+\varepsilon_n)
$$

and its weights are the $2^n$ sign vectors

$$
\frac12\sum_{j=1}^n i_j\varepsilon_j,\qquad i_j\in\{\pm1\}.
$$

Each weight has multiplicity one. Along the simple root $\alpha_j=\varepsilon_j-\varepsilon_{j+1}$, the [Kashiwara operator](../../../semisimple-lie-algebra.md#kashiwara-operator) $\widetilde e_j$ can raise a weight exactly when $(i_j,i_{j+1})=(-1,+1)$, when it replaces that pair by $(+1,-1)$. For the short root $\alpha_n=\varepsilon_n$, $\widetilde e_n$ replaces a final $-1$ by $+1$. This proves the stated crystal by the [root-string property of a crystal](../../../semisimple-lie-algebra.md#root-string-property-of-a-crystal).

For $n=3$, the complete list of raising edges is

$$
\begin{gathered}
(-,-,-)\xrightarrow{3}(-,-,+)
\xrightarrow{2}(-,+,-),\\
(-,+,-)\xrightarrow{1}(+,-,-),\qquad
(-,+,-)\xrightarrow{3}(-,+,+),\\
(+,-,-)\xrightarrow{3}(+,-,+),\qquad
(-,+,+)\xrightarrow{1}(+,-,+),\\
(+,-,+)\xrightarrow{2}(+,+,-)
\xrightarrow{3}(+,+,+).
\end{gathered}
$$

The [tensor product of crystals](../../../semisimple-lie-algebra.md#tensor-product-of-crystals) has four highest-weight connected components, of highest weights

$$
0,\qquad\omega_1,\qquad\omega_2,\qquad2\omega_3.
$$

Consequently, for the eight-dimensional spin representation $S$ of $\mathfrak{so}_7$,

$$
S\otimes S
\cong
\mathbb C\oplus V(\omega_1)\oplus V(\omega_2)\oplus V(2\omega_3),
$$

with dimensions

$$
64=1+7+21+35.
$$

Equivalently these summands are $\Lambda^k(\mathbb C^7)$ for $0\leq k\leq3$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
