# Paper 102

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20102.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20102.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
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
  - [Solution](#5/solution)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Adjoint representation of a Lie algebra](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) is

$$
\operatorname{ad}:\mathfrak g\longrightarrow\mathfrak{gl}(\mathfrak g),
\qquad
\operatorname{ad}_x(y)=[x,y].
$$

The [Killing form](../../../lie-algebra.md#killing-form) is the symmetric invariant bilinear form

$$
\boxed{\kappa(x,y)=\operatorname{tr}(\operatorname{ad}_x\operatorname{ad}_y)}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A vector subspace $I\subseteq\mathfrak g$ is an [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) when $[\mathfrak g,I]\subseteq I$. A [nilpotent Lie algebra](../../../lie-algebra.md#nilpotent-lie-algebra) is one whose lower central series

$$
\mathfrak g=\gamma_1(\mathfrak g),\qquad
\gamma_{r+1}(\mathfrak g)=[\mathfrak g,\gamma_r(\mathfrak g)]
$$

eventually vanishes.

By the [Engel theorem](../../../lie-algebra.md#engel-s-theorem), the operators $\operatorname{ad}_x$ for a nilpotent complex Lie algebra can be represented simultaneously by strictly upper triangular matrices. Their products are strictly upper triangular and have zero trace. Hence

$$
\boxed{\kappa(x,y)=0\quad\text{for every }x,y\in\mathfrak g}.
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

A [solvable Lie algebra](../../../lie-algebra.md#solvable-lie-algebra) is one whose derived series

$$
\mathfrak g^{(0)}=\mathfrak g,\qquad
\mathfrak g^{(r+1)}=[\mathfrak g^{(r)},\mathfrak g^{(r)}]
$$

eventually vanishes. By the [Lie theorem](../../../lie-algebra.md#lie-s-theorem), the adjoint operators of a solvable complex Lie algebra are simultaneously upper triangular. If $x\in[\mathfrak g,\mathfrak g]$, then $\operatorname{ad}_x$ is a sum of commutators of upper triangular matrices and is therefore strictly upper triangular. For every $y\in\mathfrak g$, the product $\operatorname{ad}_x\operatorname{ad}_y$ is strictly upper triangular, so

$$
\kappa(x,y)=0.
$$

Thus

$$
\boxed{[\mathfrak g,\mathfrak g]\subseteq\mathfrak g^\perp}.
$$

For a nonzero example, let $\mathfrak g$ have basis $h,e$ with $[h,e]=e$. It is solvable because $[\mathfrak g,\mathfrak g]=\mathbb Ce$ is abelian, but in the ordered basis $(h,e)$,

$$
\operatorname{ad}_h=
\begin{pmatrix}0&0\\0&1\end{pmatrix},
\qquad
\kappa(h,h)=1.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Invariance of the [Killing form](../../../lie-algebra.md#killing-form) gives

$$
\kappa([a,x],y)=\kappa(x,[y,a]).
$$

If $x\in\mathfrak g^\perp$, the right-hand side vanishes for every $y$, so $[a,x]\in\mathfrak g^\perp$. Thus $\mathfrak g^\perp$ is an ideal.

Let $\mathfrak h=\operatorname{ad}(\mathfrak g^\perp)\subseteq\mathfrak{gl}(\mathfrak g)$. For $x\in[\mathfrak g^\perp,\mathfrak g^\perp]$ and $y\in\mathfrak g^\perp$,

$$
\operatorname{tr}(\operatorname{ad}_x\operatorname{ad}_y)
=\kappa(x,y)=0.
$$

The [Cartan solvability criterion](../../../lie-algebra.md#cartan-solvability-criterion) makes $\mathfrak h$ solvable. The kernel of the adjoint map on $\mathfrak g^\perp$ lies in its center and is abelian, so $\mathfrak g^\perp$ is itself solvable. This proves the [Solvability of the radical of the Killing form](../../../lie-algebra.md#solvability-of-the-radical-of-the-killing-form).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The Killing form of a complex [simple Lie algebra](../../../semisimple-lie-algebra.md#simple-lie-algebra) is nondegenerate. Since $B$ is also nondegenerate, there is a unique endomorphism $T$ of $\mathfrak g$ satisfying

$$
\kappa(x,y)=B(Tx,y).
$$

Invariance of both forms gives

$$
T([z,x])=[z,Tx],
$$

so $T$ intertwines the adjoint representation. That representation is irreducible because its invariant subspaces are ideals. The [Schur lemma](../../../representation-theory.md#schur-s-lemma) therefore gives $T=cI$. Since $\kappa$ is nondegenerate, $c\ne0$, and

$$
\boxed{\kappa=cB}.
$$

This is the [uniqueness of an invariant bilinear form on a simple Lie algebra](../../../lie-algebra.md#uniqueness-of-an-invariant-bilinear-form-on-a-simple-lie-algebra).

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

For $\mathfrak{sl}_3(\mathbb C)$, the [Killing form of the special linear Lie algebra](../../../lie-algebra.md#killing-form-of-the-special-linear-lie-algebra) is

$$
\kappa(X,Y)=6\operatorname{tr}(XY).
$$

For $H_1=E_{11}-E_{22}$ and $H_2=E_{22}-E_{33}$, its matrix on the Cartan part is

$$
\begin{pmatrix}12&-6\\-6&12\end{pmatrix},
$$

whose determinant is $108$. Each $E_{ij}$ pairs only with $E_{ji}$, with value $6$. In the stated ordering, the remaining block is

$$
\begin{pmatrix}0&6I_3\\6I_3&0\end{pmatrix},
$$

whose determinant is $-6^6$. Therefore

$$
\boxed{\det\kappa=-108\cdot6^6=-5\,038\,848}.
$$

## 2

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [Weyl chamber](../../../semisimple-lie-algebra.md#fundamental-chamber-of-a-root-system) is a connected component of

$$
E\setminus\bigcup_{\alpha\in\Phi}\alpha^\perp.
$$

A [root basis](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system) $\Delta$ is a basis of $E$ made of roots such that every root is an integer combination of $\Delta$ whose nonzero coefficients all have one sign.

Choose a regular vector $\gamma$, meaning $(\gamma,\alpha)\ne0$ for every root. Declare

$$
\Phi_\gamma^+=\{\alpha\in\Phi:(\gamma,\alpha)>0\}.
$$

The indecomposable roots in $\Phi_\gamma^+$ form a root basis $\Delta_\gamma$, and every root basis arises in this way. Its chamber is the component containing $\gamma$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Root bases correspond bijectively to Weyl chambers: the walls of a chamber determine its inward simple roots. The [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) acts transitively on the chambers. One proof joins interior points of two chambers by a generic line segment. Each time the segment crosses one reflecting hyperplane, reflect the remaining segment across that wall; the resulting product of root reflections sends the first chamber to the second. It consequently sends the first root basis to the second. Thus $W$ acts transitively on root bases.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

We induct on the [Coxeter length](../../../semisimple-lie-algebra.md#coxeter-length) $\ell(w)$. There is nothing to prove when $\ell(w)=0$. Otherwise choose a simple root $\alpha$ such that

$$
\ell(ws_\alpha)=\ell(w)-1;
$$

equivalently, $w\alpha$ is negative. Since $\lambda$ and $\mu=w\lambda$ lie in the [Closed dominant Weyl chamber](../../../semisimple-lie-algebra.md#closed-dominant-weyl-chamber),

$$
0\leq\langle\lambda,\alpha^\vee\rangle
=\langle\mu,(w\alpha)^\vee\rangle\leq0.
$$

Therefore $\langle\lambda,\alpha^\vee\rangle=0$, and the simple reflection $s_\alpha$ fixes $\lambda$. Moreover,

$$
(ws_\alpha)\lambda=w\lambda=\mu.
$$

The induction hypothesis writes $ws_\alpha$ as a product of simple reflections that fix $\lambda$. Multiplying on the right by $s_\alpha$ gives the required expression for $w$. This is the [Weyl stabilizer of a dominant point](../../../semisimple-lie-algebra.md#weyl-stabilizer-of-a-dominant-point) lemma.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For existence, choose $w\in W$ maximizing $(w\lambda,\rho)$, where $\rho$ lies in the interior of the dominant chamber. If $\langle w\lambda,\alpha^\vee\rangle<0$ for a simple root $\alpha$, then

$$
(s_\alpha w\lambda,\rho)-(w\lambda,\rho)
=-\langle w\lambda,\alpha^\vee\rangle(\alpha,\rho)>0,
$$

contradicting maximality. Hence $w\lambda$ is dominant.

For uniqueness, suppose $\lambda$ and $\mu$ are dominant and $\mu=w\lambda$. Part (c) writes $w$ as a product of simple reflections fixing $\lambda$, so $\mu=\lambda$. Every Weyl orbit therefore has exactly one representative in the closed dominant chamber.

## 3

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Every diagonal element of the stated Cartan subalgebra has the form

$$
\operatorname{diag}(0,t_1,t_2,-t_1,-t_2).
$$

Let $\varepsilon_i$ extract $t_i$. The roots are the [B2 root system](../../../semisimple-lie-algebra.md#b2-root-system)

$$
\boxed{\Phi=\{\pm\varepsilon_1,\pm\varepsilon_2,
\pm\varepsilon_1\pm\varepsilon_2\}}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Choose

$$
\boxed{\alpha_1=\varepsilon_1-\varepsilon_2,\qquad
\alpha_2=\varepsilon_2}.
$$

Here $\alpha_1$ is long and $\alpha_2$ is short. The [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) consists of two vertices joined by a double edge, with its arrow pointing from $\alpha_1$ toward the shorter root $\alpha_2$:

$$
\boxed{\alpha_1\Longrightarrow\alpha_2.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [Weyl reflection](../../../semisimple-lie-algebra.md#weyl-reflection) $s_{\alpha_1}$ swaps $\varepsilon_1$ and $\varepsilon_2$, whereas $s_{\alpha_2}$ changes the sign of $\varepsilon_2$. Hence

$$
\boxed{
\begin{aligned}
s_{\alpha_1}(\alpha_1)&=-\alpha_1,
&s_{\alpha_1}(\alpha_2)&=\alpha_1+\alpha_2,\\
s_{\alpha_2}(\alpha_1)&=\alpha_1+2\alpha_2,
&s_{\alpha_2}(\alpha_2)&=-\alpha_2.
\end{aligned}}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The [highest root](../../../semisimple-lie-algebra.md#highest-root) is

$$
\boxed{\beta=\varepsilon_1+\varepsilon_2
=\alpha_1+2\alpha_2}.
$$

Since $\beta$ is long and the $\varepsilon_i$ are orthonormal, $\beta^\vee=\beta$. The [coroot](../../../semisimple-lie-algebra.md#coroot) pairing gives

$$
\boxed{\langle\alpha_1,\beta^\vee\rangle=0,
\qquad
\langle\alpha_2,\beta^\vee\rangle=1}.
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The displayed calculation identifies the root system of $\mathfrak{so}_5(\mathbb C)$ as $B_2$. The symplectic Lie algebra $\mathfrak{sp}_4(\mathbb C)$ has root system $C_2$. After exchanging the two simple-root labels, the $B_2$ and $C_2$ Cartan matrices agree, so their Dynkin diagrams define the same complex simple Lie algebra. The classification of finite-dimensional complex simple Lie algebras therefore gives

$$
\boxed{\mathfrak{so}_5(\mathbb C)\cong\mathfrak{sp}_4(\mathbb C)}.
$$

This is the [Isomorphism between so5 and sp4](../../../semisimple-lie-algebra.md#isomorphism-between-so5-and-sp4).

## 4

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Choose positive roots $\Phi^+$ and let

$$
\rho=\frac12\sum_{\alpha\in\Phi^+}\alpha
$$

be the [Weyl vector](../../../semisimple-lie-algebra.md#half-sum-of-positive-roots). For a [dominant integral weight](../../../semisimple-lie-algebra.md#dominant-integral-weight) $\lambda$, the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) is

$$
\boxed{\dim V(\lambda)
=\prod_{\alpha\in\Phi^+}
\frac{\langle\lambda+\rho,\alpha^\vee\rangle}
{\langle\rho,\alpha^\vee\rangle}}.
$$

Here $\alpha^\vee$ is the coroot and $\langle\ ,\ \rangle$ is the natural weight-coroot pairing.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Write the nonzero highest weight of $V$ as

$$
\lambda=\sum_{j=1}^{\ell}m_j\omega_j,
\qquad m_j\in\mathbb Z_{\geq0}.
$$

Choose $i$ with $m_i>0$. Then $\lambda-\omega_i$ is dominant. Every positive coroot is a nonnegative combination of simple coroots, so every numerator in the Weyl dimension formula for $\lambda$ is at least the corresponding numerator for $\omega_i$. Thus

$$
\dim V(\lambda)\geq\dim V(\omega_i).
$$

Minimality of $\dim V$ forces equality. If $\lambda\ne\omega_i$, some simple-coroot factor is strictly larger, making the product strict. Hence $\lambda=\omega_i$ and

$$
\boxed{V\cong V(\omega_i)},
$$

so $V$ is a [fundamental representation](../../../semisimple-lie-algebra.md#fundamental-representation).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For an irreducible representation $V(\lambda)$, write

$$
\lambda=\sum_i m_i\omega_i.
$$

Form

$$
T=\bigotimes_iV(\omega_i)^{\otimes m_i}.
$$

The tensor product of highest-weight vectors is killed by all positive-root spaces and has weight $\lambda$. It therefore generates a highest-weight constituent isomorphic to $V(\lambda)$. By [complete reducibility of semisimple Lie algebra representations](../../../semisimple-lie-algebra.md#weyl-s-theorem-on-complete-reducibility), this constituent is a subrepresentation of $T$. This proves the [generation by fundamental representations](../../../semisimple-lie-algebra.md#generation-by-fundamental-representations) statement.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For $\mathfrak{sl}_3(\mathbb C)$ there are two fundamental weights. The corresponding [Fundamental representations of sl3](../../../semisimple-lie-algebra.md#fundamental-representations-of-sl3) are

$$
\boxed{V(\omega_1)=\mathbb C^3,\qquad
V(\omega_2)=\Lambda^2\mathbb C^3\cong(\mathbb C^3)^*}.
$$

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Let $V=V(\omega_1)$, so $V^*=V(\omega_2)$. First,

$$
V\otimes V
=\operatorname{Sym}^2V\oplus\Lambda^2V
\cong V(2\omega_1)\oplus V(\omega_2).
$$

The highest-weight tensor-product rule gives

$$
V(2\omega_1)\otimes V(\omega_2)
\cong V(2\omega_1+\omega_2)\oplus V(\omega_1)
$$

and

$$
V(\omega_2)\otimes V(\omega_2)
\cong V(2\omega_2)\oplus V(\omega_1).
$$

The dimensions $15+3+6+3=27$ check the decomposition. Therefore the [Triple tensor decomposition for the defining sl3 representation](../../../semisimple-lie-algebra.md#triple-tensor-decomposition-for-the-defining-sl3-representation) is

$$
\boxed{V\otimes V\otimes V^*
\cong V(2\omega_1+\omega_2)\oplus
V(2\omega_2)\oplus V(\omega_1)^{\oplus2}}.
$$

Thus one may take

$$
\boxed{(\lambda_1,\lambda_2,\lambda_3,\lambda_4)
=(2\omega_1+\omega_2,\,2\omega_2,\,\omega_1,\,\omega_1).}
$$

## 5

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The [classification of finite-dimensional sl2 representations](../../../semisimple-lie-algebra.md#classification-of-finite-dimensional-sl2-representations) says that for every $n\geq0$ there is one irreducible module $V(n)$ of dimension $n+1$, with weights

$$
n,n-2,\ldots,-n
$$

of multiplicity one, and every finite-dimensional $\mathfrak{sl}_2(\mathbb C)$-module is a direct sum of these irreducibles.

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice) is

$$
X=\{\lambda\in\mathfrak t^*:
\langle\lambda,\alpha^\vee\rangle\in\mathbb Z
\text{ for every }\alpha\in\Phi\}.
$$

For each root $\alpha$, restrict $V$ to the subalgebra

$$
\mathfrak m_\alpha=\operatorname{span}\{e_\alpha,h_\alpha,f_\alpha\}
\cong\mathfrak{sl}_2.
$$

If $V_\lambda\ne0$, the $\mathfrak{sl}_2$ classification shows that the $h_\alpha$-eigenvalue $\lambda(h_\alpha)=\langle\lambda,\alpha^\vee\rangle$ is an integer. Hence $\lambda\in X$.

The same classification makes every $\alpha$-string symmetric under

$$
\lambda\longmapsto
\lambda-\langle\lambda,\alpha^\vee\rangle\alpha=s_\alpha\lambda
$$

and preserves weight multiplicity. Since the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) is generated by these simple reflections,

$$
\boxed{V_{w\lambda}\ne0\quad\text{and}\quad
\dim V_{w\lambda}=\dim V_\lambda
\quad(w\in W)}.
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Take $\mathfrak g=\mathfrak{sl}_3(\mathbb C)$ and its adjoint representation $V=\mathfrak g$. This representation is irreducible because $\mathfrak g$ is simple. Its zero-weight space is the Cartan subalgebra $\mathfrak t$, so

$$
\boxed{\operatorname{mult}(0)=\dim\mathfrak t=2}.
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The [dominance order](../../../semisimple-lie-algebra.md#dominance-order) is

$$
\mu\preceq\lambda
\quad\Longleftrightarrow\quad
\lambda-\mu=\sum_i n_i\alpha_i
\quad(n_i\in\mathbb Z_{\geq0}).
$$

Suppose $\lambda\ne\mu$. Put $\delta=\lambda-\mu$. Since $\mu$ is dominant,

$$
(\lambda,\delta)=(\mu,\delta)+(\delta,\delta)>0.
$$

Writing $\delta=\sum_i n_i\alpha_i$, some index with $n_i>0$ therefore satisfies $(\lambda,\alpha_i)>0$, equivalently $\langle\lambda,\alpha_i^\vee\rangle>0$. The $\mathfrak{sl}_2$ lowering operator

$$
f_i:V_\lambda\longrightarrow V_{\lambda-\alpha_i}
$$

is injective by the [Injectivity of sl2 lowering above weight zero](../../../semisimple-lie-algebra.md#injectivity-of-sl2-lowering-above-weight-zero). Hence

$$
\operatorname{mult}(\lambda)
\leq\operatorname{mult}(\lambda-\alpha_i).
$$

The new weight still dominates $\mu$ in the partial order. Iterating until reaching $\mu$ gives

$$
\boxed{\operatorname{mult}(\mu)\geq\operatorname{mult}(\lambda)}.
$$

This is the [weight multiplicity decreases away from a dominant weight](../../../semisimple-lie-algebra.md#weight-multiplicity-decreases-away-from-a-dominant-weight) property.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
