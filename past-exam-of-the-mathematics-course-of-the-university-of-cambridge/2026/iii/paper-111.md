# Paper 111

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20111.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20111.pdf)

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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [fundamental system of a root system](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system) is a subset $\Delta\subset\Phi$ which is a [basis](../../../vector-space.md#basis) of $V$ and for which every $\beta\in\Phi$ has an expansion

$$
\beta=\sum_{\alpha\in\Delta}c_\alpha\alpha
$$

whose coefficients are either all nonnegative or all nonpositive. Its associated [positive system of a root system](../../../semisimple-lie-algebra.md#positive-system-of-a-root-system) is

$$
\Pi=\left\{\beta\in\Phi:c_\alpha\geq0\text{ for every }\alpha\in\Delta\right\}.
$$

**Thus $\Phi=\Pi\sqcup(-\Pi)$, and the elements of $\Delta$ are the [simple roots](../../../semisimple-lie-algebra.md#simple-root).**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [Weyl reflection](../../../semisimple-lie-algebra.md#weyl-reflection) in $\alpha$ satisfies

$$
s_\alpha(\alpha)=-\alpha.
$$

Now take $\beta\in\Pi\setminus\{\alpha\}$ and expand it in the [basis](../../../vector-space.md#basis) $\Delta$. At least one coefficient belonging to a simple root other than $\alpha$ is positive. Since

$$
s_\alpha(\beta)=\beta-\langle\beta,\alpha^\vee\rangle\alpha,
$$

the reflection changes only the coefficient of $\alpha$. Every root has simple-root coefficients of one sign, so the unchanged positive coefficient prevents $s_\alpha(\beta)$ from being negative. Hence $s_\alpha(\beta)\in\Pi$. Because $s_\alpha$ is an involution, it permutes $\Pi\setminus\{\alpha\}$, while it exchanges $\alpha$ and $-\alpha$. Therefore

$$
\boxed{s_\alpha(\Pi)=(\Pi\sqcup\{-\alpha\})\setminus\{\alpha\}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $C$ be the [fundamental chamber of a root system](../../../semisimple-lie-algebra.md#fundamental-chamber-of-a-root-system). The chambers $wC$ and $ws_\alpha C$ are adjacent across the reflecting hyperplane orthogonal to $w(\alpha)$. The chamber $wC$ lies on the side on which $w(\alpha)$ is positive. If $w(\alpha)\in\Pi$, then $C$ lies on that same side, so crossing this wall moves one step farther from $C$; if $w(\alpha)\in-\Pi$, it moves one step nearer. The gallery distance from $C$ to $wC$ is the [Coxeter length](../../../semisimple-lie-algebra.md#coxeter-length) $\ell(w)$, and adjacent chamber distances differ by one. Consequently

$$
\boxed{w(\alpha)\in\Pi
\quad\Longleftrightarrow\quad
\ell(ws_\alpha)=\ell(w)+1
\quad\Longleftrightarrow\quad
\ell(ws_\alpha)>\ell(w).}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Write $N(w)$ for the [inversion set of a Weyl-group element](../../../semisimple-lie-algebra.md#inversion-set-of-a-weyl-group-element). Part b shows that $s_\alpha$ permutes $\Pi\setminus\{\alpha\}$. It follows that right multiplication by $s_\alpha$ changes the size of the inversion set by

$$
|N(ws_\alpha)|=
\begin{cases}
|N(w)|+1,&w(\alpha)\in\Pi,\\
|N(w)|-1,&w(\alpha)\in-\Pi.
\end{cases}
$$

Indeed, all roots other than $\alpha$ are merely relabelled, while $ws_\alpha(\alpha)=-w(\alpha)$. Part c gives exactly the same recursion for the [Coxeter length](../../../semisimple-lie-algebra.md#coxeter-length). Both quantities vanish at the identity, so induction along any word in the simple reflections gives

$$
\boxed{\ell(w)=|N(w)|
=\left|\{\beta\in\Pi:w(\beta)\in-\Pi\}\right|.}
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

By the assumed transitivity on [fundamental systems](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system), some $w_0\in W$ sends $\Delta$ to $-\Delta$. It therefore sends the entire [positive system of a root system](../../../semisimple-lie-algebra.md#positive-system-of-a-root-system) $\Pi$ to $-\Pi$. Part d then gives

$$
\ell(w_0)=|\Pi|=\frac{|\Phi|}{2}.
$$

For every $w\in W$, its [inversion set](../../../semisimple-lie-algebra.md#inversion-set-of-a-weyl-group-element) is contained in $\Pi$, so $\ell(w)\leq|\Pi|$ and $w_0$ has maximal length.

If $u$ also has maximal length, then $N(u)=\Pi$, so $u(\Pi)=-\Pi$. Hence $w_0^{-1}u$ preserves $\Pi$ and has no inversions. Part d makes its [Coxeter length](../../../semisimple-lie-algebra.md#coxeter-length) zero, so it is the identity. Thus $u=w_0$, proving that the [longest element of a finite Coxeter group](../../../lie-theory.md#longest-element-of-a-coxeter-group) is unique and has length $|\Phi|/2$.

## 2

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $V$ be the real [vector space](../../../vector-space.md) with basis $(e_i)_{i\in I}$. The [Coxeter Gram matrix](../../../lie-theory.md#coxeter-gram-matrix) defines the symmetric [bilinear form](../../../linear-algebra.md#bilinear-form)

$$
\langle e_i,e_j\rangle=G(W)_{ij}=-2\cos\left(\frac{\pi}{m_{ij}}\right).
$$

Its diagonal entries are $2$. The [Geometric representation of a Coxeter group](../../../lie-theory.md#geometric-representation-of-a-coxeter-group) is generated by the reflections

$$
\sigma(x_i)(v)=v-\langle v,e_i\rangle e_i.
$$

Each has square one, and on $\operatorname{span}\{e_i,e_j\}$ the product $\sigma(x_i)\sigma(x_j)$ has order $m_{ij}$. The reflections therefore satisfy the Coxeter relations and define a [group representation](../../../representation-theory.md#group-representation) $\sigma:W\to GL(V)$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Coxeter graph](../../../lie-theory.md#coxeter-graph) has vertex set $I$. Distinct vertices $i,j$ are joined precisely when $m_{ij}\geq3$, and the edge is labelled $m_{ij}$ when $m_{ij}>3$; the customary unlabelled edge therefore means $m_{ij}=3$. The [Coxeter system](../../../lie-theory.md#coxeter-system) is an [Irreducible Coxeter system](../../../lie-theory.md#irreducible-coxeter-system) precisely when this graph is [connected](../../../graph.md#connected-graph).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Put

$$
a=2\cos\left(\frac{\pi}{m_{ij}}\right).
$$

After ordering $I_1$ before $I_2$, the only nonzero off-diagonal entries between the two blocks occur at $(i,j)$ and $(j,i)$, where they equal $-a$. Thus

$$
G(W)=
\begin{pmatrix}
G(W_1)&-a,e_ie_j^T\\
-a,e_je_i^T&G(W_2)
\end{pmatrix},
$$

where the coordinate vectors in the two blocks are understood. Expanding the [determinant](../../../linear-algebra.md#determinant) according to whether neither or both cross-block entries are selected gives

$$
\det G(W)
=\det G(W_1)\det G(W_2)
-a^2\det G(W_1')\det G(W_2').
$$

The minus sign is the sign of the transposition pairing the two cross-block entries. This formula remains valid when either diagonal block is singular, so no inverse or [Schur complement](../../../linear-algebra.md#schur-complement) is needed.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

All edges in the [Type E(p,q,k) Coxeter graph](../../../lie-theory.md#type-e-p-q-k-coxeter-graph) are unlabelled, so the factor $a^2$ in part c is one. Separate the arm of length $p$ from the central vertex. The remaining two arms form a type $A_{q+k+1}$ chain, while deleting the central vertex leaves the disjoint type $A_q$ and type $A_k$ chains. Using $\det G(A_r)=r+1$ in the formula from part c yields

$$
\begin{aligned}
\det G(E(p,q,k))
&=(p+1)(q+k+2)-p(q+1)(k+1)\\
&=(p+1)(q+1)(k+1)
\left(\frac1{p+1}+\frac1{q+1}+\frac1{k+1}-1\right).
\end{aligned}
$$

The associated [bilinear form](../../../linear-algebra.md#bilinear-form) is degenerate exactly when

$$
\frac1{p+1}+\frac1{q+1}+\frac1{k+1}=1.
$$

The positive-integer solutions of $1/a+1/b+1/c=1$, up to permutation, are $(3,3,3)$, $(2,4,4)$, and $(2,3,6)$. Consequently the degenerate arm-length triples are the permutations of

$$
(2,2,2),\qquad(1,3,3),\qquad(1,2,5).
$$

For every other allowed $(p,q,k)$ the determinant is nonzero, so the form is [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form).

## 3

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Generic Hecke algebra of a Coxeter system](../../../lie-theory.md#iwahori-hecke-algebra) is the free module with basis $(T_w)_{w\in W}$ over the polynomial ring in parameters $a_i$, subject to $a_i=a_j$ whenever $x_i$ and $x_j$ are conjugate, and with multiplication

$$
T_iT_w=
\begin{cases}
T_{x_iw},&\ell(x_iw)>\ell(w),\\
a_iT_{x_iw}+(a_i-1)T_w,&\ell(x_iw)<\ell(w).
\end{cases}
$$

Equivalently, its generators satisfy the Coxeter braid relations and

$$
(T_i-a_i)(T_i+1)=0.
$$

In type $A_n$, all simple generators are conjugate, so there is one parameter.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A [BN-pair](../../../lie-theory.md#bn-pair) consists of subgroups $B,N\leq G$ for which $G=\langle B,N\rangle$, the subgroup $H=B\cap N$ is normal in $N$, the quotient $W=N/H$ is generated by a distinguished set $S$ of involutions, and the Bruhat multiplication and nondegeneracy axioms hold. The quotient is the associated [Weyl group](../../../semisimple-lie-algebra.md#weyl-group), and the axioms give the [Bruhat decomposition of a BN-pair](../../../lie-theory.md#bruhat-decomposition-of-a-bn-pair)

$$
G=\bigsqcup_{w\in W}B\dot wB.
$$

The [Iwahori-Hecke algebra of a BN-pair](../../../lie-theory.md#iwahori-hecke-algebra-of-a-bn-pair) may be defined, up to the usual opposite-algebra convention, by

$$
H_k(G,B)=\operatorname{End}_{kG}(k[G/B]).
$$

Its standard basis $(T_w)_{w\in W}$ is indexed by the Bruhat double cosets. For a simple generator $x_i$ represented by $\dot x_i\in N$, set

$$
q_i=[B:B\cap\dot x_iB\dot x_i^{-1}].
$$

The double-coset multiplication rule is the generic rule from part a with $a_i$ specialized to $q_i\cdot1_k$. Thus $H_k(G,B)$ is a [specialization](../../../associative-algebra.md#specialization-of-an-algebra) of the generic algebra.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Every [Hecke parameter of a BN-pair](../../../lie-theory.md#hecke-parameter-of-a-bn-pair) $q_i$ divides $|B|$ and, because $B$ is a $q$-group, is a power of $q$. If $q\equiv1\pmod p$, then $q_i=1$ in the field $k$ of [characteristic](../../../algebra.md#characteristic-of-a-field) $p$. The specialized quadratic relation becomes

$$
T_i^2=1,
$$

while the braid relations are unchanged. These are the defining relations of the [Coxeter group](../../../lie-theory.md#coxeter-group) $W$, so $x_i\mapsto T_i$ induces a surjective homomorphism

$$
k[W]\longrightarrow H_k(G,B).
$$

Both algebras have bases indexed by $W$, hence the homomorphism is an isomorphism of [group algebras](../../../associative-algebra.md#group-algebra).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

There is a missing hypothesis in the printed claim: it is false when every irreducible component of $W$ has type $A_1$. The intended statement holds as soon as $W$ has an [irreducible component](../../../lie-theory.md#irreducible-coxeter-system) of rank at least two, which we now assume.

Since $q=p$, every [Hecke parameter of a BN-pair](../../../lie-theory.md#hecke-parameter-of-a-bn-pair) vanishes in $k$, and $H$ is the [0-Hecke algebra](../../../lie-theory.md#0-hecke-algebra) with

$$
T_i^2=-T_i.
$$

Let $w_0$ be the [longest element of a finite Coxeter group](../../../lie-theory.md#longest-element-of-a-coxeter-group). Choose a simple generator $s$ in a component of rank at least two, put

$$
r=w_0sw_0,qquad v=w_0s,qquad X=T_v+T_{w_0}.
$$

The element $r$ is again a simple generator. The identities $rv=w_0$ and $\ell(w_0)=\ell(v)+1$ give

$$
T_rX=T_{w_0}-T_{w_0}=0.
$$

If $t\ne r$ is simple, then $t$ is a left descent of both $v$ and $w_0$: using $\ell(w_0u)=\ell(w_0)-\ell(u)$, one gets $\ell(tv)=\ell(v)-1$. Hence

$$
T_tX=-T_v-T_{w_0}=-X.
$$

The one-dimensional subspace $kX$ is therefore a [left ideal](../../../associative-algebra.md#left-ideal). It is nonzero because $T_v$ and $T_{w_0}$ are distinct basis elements.

Every [reduced expression in a Coxeter group](../../../lie-theory.md#reduced-expression-in-a-coxeter-group) for $v=w_0s$ contains $r$: in an irreducible finite component of rank at least two, deleting one final generator from $w_0$ does not remove any vertex from its support. A reduced expression for $w_0$ contains $r$ as well. Since $T_rX=0$, associativity now gives

$$
T_vX=T_{w_0}X=0,
\qquad
X^2=(T_v+T_{w_0})X=0.
$$

If $H$ were a [semisimple algebra](../../../associative-algebra.md#semisimple-algebra), the left ideal $kX$ would be a direct summand of the regular module. The corresponding projection would produce a nonzero idempotent in $kX$, impossible because $(kX)^2=0$. Thus $H$ is not semisimple.

For completeness, if $W\cong(A_1)^m$, then

$$
H\cong k[T_1,\ldots,T_m]/(T_i(T_i+1))
\cong(k\times k)^{\otimes m},
$$

which is semisimple. This is the counterexample showing why the omitted rank condition is necessary.

## 4

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [Coxeter number](../../../lie-theory.md#coxeter-number) is the order of a [Coxeter element](../../../lie-theory.md#coxeter-element). In the stated families the values are

$$
\begin{array}{c|c|c}
W&\text{Coxeter type}&h\\ \hline
D_{2n}&I_2(n)&n\\
S_n&A_{n-1}&n\\
SS_n&B_n&2n\\
ESS_n&D_n&2n-2.
\end{array}
$$

Here $D_{2n}$ is the [dihedral group](../../../finite-group-theory.md#dihedral-group) of order $2n$, $S_n$ is the [symmetric group](../../../finite-group-theory.md#symmetric-group), $SS_n$ is the [signed symmetric group](../../../lie-theory.md#hyperoctahedral-group), and $ESS_n$ is the [even signed symmetric group](../../../lie-theory.md#even-signed-symmetric-group).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Set

$$
a_{ij}=2\cos\left(\frac{\pi}{m_{ij}}\right),
\qquad c_i=x_1\cdots x_i,
\qquad c_0=1.
$$

In the [Geometric representation of a Coxeter group](../../../lie-theory.md#geometric-representation-of-a-coxeter-group),

$$
\sigma(x_i)e_j=e_j+a_{ij}e_i,
$$

including $i=j$, since $a_{ii}=2\cos\pi=-2$. As $\beta_i=\sigma(c_{i-1})e_i$, telescoping gives

$$
\sigma(c_i)e_j-\sigma(c_{i-1})e_j
=a_{ij}\beta_i.
$$

Summing from $i=1$ to $j-1$ yields

$$
\beta_j=e_j+\sum_{i<j}a_{ij}\beta_i,
$$

or equivalently

$$
e_j=\beta_j-\sum_{i<j}2\cos\left(\frac{\pi}{m_{ij}}\right)\beta_i.
$$

Summing the same telescoping identity all the way to $n$ and substituting this first formula gives

$$
\begin{aligned}
\sigma(c)e_j
&=e_j+\sum_{i=1}^na_{ij}\beta_i\\
&=\beta_j+\sum_{i\geq j}2\cos\left(\frac{\pi}{m_{ij}}\right)\beta_i,
\end{aligned}
$$

which is the second required identity.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $B$ be the matrix whose $i$th column consists of the coordinates of $\beta_i$ in the basis $(e_j)$. Define the upper-triangular matrix $U$ and lower-triangular matrix $L$ by

$$
U_{ij}=
\begin{cases}
1,&i=j,\\
-a_{ij},&i<j,\\
0,&i>j,
\end{cases}
\qquad
L_{ij}=
\begin{cases}
1+a_{ii}=-1,&i=j,\\
a_{ij},&i>j,\\
0,&i<j.
\end{cases}
$$

The first identity in part b says $I=BU$, so $B=U^{-1}$. The second says that the matrix $C$ of $\sigma(c)$ is $C=BL=U^{-1}L$. Since $U$ has diagonal entries one, $\det U=1$, and therefore

$$
\det(tI-C)
=\det\bigl(U^{-1}(tU-L)\bigr)
=\det(tU-L).
$$

**Thus $\det(tU-L)$ is the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) of the [Coxeter element](../../../lie-theory.md#coxeter-element) in its geometric representation.**

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

At $t=1$, the diagonal entries of $U-L$ are $2$, while every off-diagonal $(i,j)$ entry is

$$
-a_{ij}=-2\cos\left(\frac{\pi}{m_{ij}}\right).
$$

Hence $U-L$ is exactly the [Coxeter Gram matrix](../../../lie-theory.md#coxeter-gram-matrix) $G(W)$, and part c gives

$$
\det(I-C)=\det G(W).
$$

For a [Finite Coxeter group](../../../lie-theory.md#finite-coxeter-group) the Gram matrix is [positive definite](../../../linear-algebra.md#positive-definite-matrix), and for a [Hyperbolic Coxeter group](../../../lie-theory.md#hyperbolic-coxeter-group) it is nondegenerate with Lorentzian signature. In either case $\det(I-C)\ne0$, so $1$ is not an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of $C$ and the [Coxeter element](../../../lie-theory.md#coxeter-element) fixes no nonzero vector.

For an [Affine Coxeter group](../../../lie-theory.md#affine-coxeter-group), the Gram form has a nonzero [radical](../../../linear-algebra.md#radical-of-a-bilinear-form). If $0\ne v\in\operatorname{rad}G(W)$, then $\langle v,e_i\rangle=0$ for every $i$, and every generating reflection satisfies

$$
\sigma(x_i)v=v-\langle v,e_i\rangle e_i=v.
$$

Their product $\sigma(c)$ therefore fixes $v$. Thus every affine Coxeter element has a nonzero fixed vector.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
