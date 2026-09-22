# Paper 102

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/Paper_102.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/Paper_102.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $D=\operatorname{ad}y$. The [generalized eigenspace](../../../linear-operator-theory.md#generalized-eigenspace) decomposition of the [linear map](../../../vector-space.md#linear-map) $D$ is

$$
L=\bigoplus_\lambda L_{\lambda,y},
\qquad
L_{\lambda,y}=\ker(D-\lambda I)^N
$$

for any sufficiently large $N$. Because $D$ is a [derivation](../../../lie-algebra.md#derivation-of-a-lie-algebra), the [generalized-eigenspace bracket lemma](../../../lie-algebra.md#generalized-eigenspace-bracket-lemma) gives

$$
[L_{\lambda,y},L_{\mu,y}]\subseteq L_{\lambda+\mu,y}.
$$

Consequently $L_{0,y}$ is a [Lie subalgebra](../../../lie-algebra.md#lie-subalgebra).

The set $I(K)=\{x\in L:[x,K]\subseteq K\}$ is the [normalizer of a Lie subalgebra](../../../lie-algebra.md#normalizer-of-a-lie-subalgebra) $K$. Certainly $L_{0,y}\subseteq I(L_{0,y})$. Conversely, if $x\in I(L_{0,y})$, then $y\in L_{0,y}$ gives

$$
Dx=[y,x]\in L_{0,y}.
$$

On the direct sum of the nonzero generalized eigenspaces, $D$ is [invertible](../../../calculus.md#invertible-linear-map). Hence the nonzero-eigenvalue component of $x$ vanishes, and

$$
\boxed{I(L_{0,y})=L_{0,y}.}
$$

Now let $K$ be a [Lie subalgebra](../../../lie-algebra.md#lie-subalgebra) containing $L_{0,y}$. Since $y\in K$, the subspace $K$ is $D$-invariant. The generalized zero eigenspace of the induced map on $L/K$ is the image of $L_{0,y}$, hence is zero. If $x\in I(K)$, then $Dx=[y,x]\in K$, so $x+K$ lies in that zero eigenspace. Thus $x\in K$ and

$$
\boxed{I(K)=K.}
$$

A [nilpotent Lie algebra](../../../lie-algebra.md#nilpotent-lie-algebra) is one whose [lower central series](../../../lie-algebra.md#lower-central-series-of-a-lie-algebra)

$$
\gamma_1(L)=L,
\qquad
\gamma_{r+1}(L)=[L,\gamma_r(L)]
$$

eventually reaches zero. Suppose $L$ is nilpotent and $K\subsetneq L$. Choose the least $r\geq2$ for which $\gamma_r(L)\subseteq K$. Then $\gamma_{r-1}(L)\nsubseteq K$, and any

$$
x\in\gamma_{r-1}(L)\setminus K
$$

satisfies $[x,K]\subseteq[L,\gamma_{r-1}(L)]=\gamma_r(L)\subseteq K$. Therefore $x\in I(K)\setminus K$, proving the [normalizer condition for a nilpotent Lie algebra](../../../lie-algebra.md#normalizer-condition-for-a-nilpotent-lie-algebra)

$$
\boxed{K\subsetneq I(K).}
$$

It remains to prove the converse needed here. The [Engel lemma](../../../lie-algebra.md#engel-lemma) states that if a finite-dimensional [Lie algebra of linear maps](../../../lie-algebra.md#lie-algebra-representation) consists of [nilpotent maps](../../../linear-operator-theory.md#nilpotent-linear-map), then the maps have a common nonzero vector in their kernels. To prove it, induct on the dimension of the algebra. For a maximal proper subalgebra $H$, induction applied to the action of $H$ on $L/H$ produces $x\notin H$ with $[H,x]\subseteq H$. Thus $H$ is an ideal of codimension one. Induction also gives a nonzero common kernel

$$
W=\{v:Hv=0\}.
$$

The ideal property makes $W$ invariant under $L$; a nilpotent representative of a basis of $L/H$ has a nonzero kernel on $W$, yielding a vector killed by all of $L$.

Apply the lemma to the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra). It produces a nonzero element of the [center of a Lie algebra](../../../lie-algebra.md#center-of-a-lie-algebra). Induction on $\dim L$, followed by passage to the quotient by this center, proves [Engel theorem](../../../lie-algebra.md#engel-s-theorem): if every $\operatorname{ad}y$ is nilpotent, then $L$ is nilpotent. The hypothesis $L_{0,y}=L$ says exactly that every $\operatorname{ad}y$ is nilpotent, so

$$
\boxed{L\text{ is nilpotent}.}
$$

## 2

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A finite [root system](../../../semisimple-lie-algebra.md#root-system) in a real [Euclidean vector space](../../../functional-analysis.md#euclidean-norm) $E$ is a finite spanning set $\Phi\subset E\setminus\{0\}$ such that, for every $\alpha\in\Phi$, the [root reflection](../../../semisimple-lie-algebra.md#root-reflection)

$$
s_\alpha(v)=v-\frac{2(v,\alpha)}{(\alpha,\alpha)}\alpha
$$

preserves $\Phi$, and the [Cartan integer](../../../semisimple-lie-algebra.md#cartan-integer) $2(\beta,\alpha)/(\alpha,\alpha)$ is an integer for all $\alpha,\beta\in\Phi$. It is [reduced](../../../semisimple-lie-algebra.md#reduced-root-system) when the only scalar multiples of $\alpha$ in $\Phi$ are $\alpha$ and $-\alpha$. Its [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) is the subgroup of the [orthogonal group](../../../linear-algebra.md#orthogonal-group) generated by the reflections $s_\alpha$. A [base of a root system](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system) $\Delta$ is a [basis](../../../vector-space.md#basis) of $E$ such that every root is an integer combination of elements of $\Delta$ whose nonzero coefficients all have the same sign.

The [coroot](../../../semisimple-lie-algebra.md#coroot) of $\alpha$ is

$$
\alpha^\vee=\frac{2\alpha}{(\alpha,\alpha)}.
$$

Let $C$ be the [Weyl chamber](../../../semisimple-lie-algebra.md#fundamental-chamber-of-a-root-system) determined by $\Delta$:

$$
C=\{v\in E:(v,\alpha)>0\text{ for every }\alpha\in\Delta\}.
$$

The roots $\alpha$ and $\alpha^\vee$ are positive scalar multiples, so their reflecting hyperplanes and their positive half-spaces are identical. The same chamber $C$ therefore defines positivity in the [coroot system](../../../semisimple-lie-algebra.md#root-system) $\Phi^\vee$. Its walls correspond exactly to the rays $\mathbb R_{>0}\alpha^\vee$ for $\alpha\in\Delta$. Hence its simple roots are

$$
\boxed{\Delta^\vee=\{\alpha^\vee:\alpha\in\Delta\},}
$$

which is therefore a base of $\Phi^\vee$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For an arbitrary finite-dimensional complex [Lie algebra](../../../lie-algebra.md) $L$, a [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) is a nilpotent [Lie subalgebra](../../../lie-algebra.md#lie-subalgebra) $H$ equal to its own [normalizer](../../../lie-algebra.md#normalizer-of-a-lie-subalgebra). When $L$ is [semisimple](../../../semisimple-lie-algebra.md), this is equivalently a maximal abelian subalgebra consisting of elements that act semisimply in the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra).

Choose such an $H$. Simultaneous diagonalization gives the [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition)

$$
L=H\oplus\bigoplus_{\alpha\in\Phi}L_\alpha,
\qquad
L_\alpha=\{x\in L:[h,x]=\alpha(h)x\text{ for every }h\in H\}.
$$

The nonzero [weights](../../../semisimple-lie-algebra.md#weight-of-a-representation) $\alpha\in H^*$ are the roots. The restriction of the [Killing form](../../../lie-algebra.md#killing-form) $B$ to $H$ is a [nondegenerate bilinear form](../../../linear-algebra.md#nondegenerate-bilinear-form), so each $\alpha$ corresponds to a unique $t_\alpha\in H$ with $\alpha(h)=B(t_\alpha,h)$. On the real span of these $t_\alpha$, the restriction of $B$ supplies a positive-definite inner product after choosing the standard real form. The [sl2 subalgebra associated with a root](../../../semisimple-lie-algebra.md#sl2-subalgebra-associated-with-a-root) gives

$$
s_\alpha(\beta)=\beta-\langle\beta,\alpha^\vee\rangle\alpha,
\qquad
\langle\beta,\alpha^\vee\rangle\in\mathbb Z,
$$

and shows that these reflections preserve the finite set $\Phi$. Thus the roots form a finite reduced crystallographic [root system](../../../semisimple-lie-algebra.md#root-system), whose [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) is generated by these reflections.

## 3

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A finite-dimensional [Lie algebra](../../../lie-algebra.md) $L$ is [semisimple](../../../semisimple-lie-algebra.md) when its [solvable radical](../../../lie-algebra.md#radical-of-a-lie-algebra) is zero, equivalently when it has no nonzero solvable [ideals](../../../lie-algebra.md#ideal-of-a-lie-algebra).

We prove the [Weyl complete reducibility theorem](../../../semisimple-lie-algebra.md#weyl-complete-reducibility-theorem). Induct on the dimension of a finite-dimensional $L$-module $V$. It is enough first to split a submodule $W$ of codimension one. The one-dimensional quotient is trivial because a semisimple Lie algebra is [perfect](../../../semisimple-lie-algebra.md#perfect-lie-algebra). By induction, $W$ is a direct sum of irreducible modules. A [Casimir element](../../../semisimple-lie-algebra.md#casimir-element) formed using the [Killing form](../../../lie-algebra.md#killing-form) commutes with the $L$-action, acts as zero on every trivial summand, and acts by a nonzero scalar on every nontrivial irreducible summand. Its image is therefore the sum $W_1$ of the nontrivial summands, while its kernel contains the trivial summands $W_0$ and maps onto $V/W$. Thus

$$
V=W_1\oplus\ker\Omega.
$$

Inside $\ker\Omega$, choose a lift $v$ of a basis of $V/W$. For $x\in L$, $xv\in W_0$, and $L$ acts trivially on $W_0$. Hence $[x,y]v=0$ for all $x,y\in L$. Since $L=[L,L]$, actually $xv=0$ for every $x$, so $\mathbb Cv$ is the required invariant complement.

This codimension-one case implies the general case. For an arbitrary submodule $W\subseteq V$, let

$$
X=\{f\in\operatorname{Hom}_{\mathbb C}(V,W):f|_W\text{ is scalar}\}
$$

with the natural [Hom representation](../../../lie-algebra.md#hom-representation). The maps vanishing on $W$ form an $L$-submodule $X_0$ of codimension one. Splitting $X_0$ supplies an $L$-equivariant $f$ with $f|_W=I_W$. Then

$$
V=W\oplus\ker f,
$$

so every invariant subspace has an invariant complement and every finite-dimensional representation is completely reducible.

For the requested example, embed $\mathfrak{sl}_2$ as the upper-left $2\times2$ block in the [special linear Lie algebra](../../../semisimple-lie-algebra.md#special-linear-lie-algebra) $\mathfrak{sl}_3$. Under the restricted [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra),

$$
\mathfrak{sl}_3
=\underbrace{\mathfrak{sl}_2}_{V_2}
\oplus\underbrace{\mathbb C\operatorname{diag}(1,1,-2)}_{V_0}
\oplus\underbrace{\langle E_{13},E_{23}\rangle}_{V_1}
\oplus\underbrace{\langle E_{31},E_{32}\rangle}_{V_1}.
$$

Here $V_n$ is the irreducible $\mathfrak{sl}_2$-module of highest weight $n$. The first summand is the three-dimensional adjoint module, the second is trivial, and the last two are the two-dimensional defining module and its dual, which are isomorphic. This explicit direct sum demonstrates complete reducibility.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Because $M$ is a finite-dimensional [semisimple module](../../../module-theory.md#semisimple-module), it has an [isotypic decomposition](../../../module-theory.md#isotypic-decomposition)

$$
M\simeq\bigoplus_{i=1}^t S_i^{m_i},
$$

where the $S_i$ are pairwise nonisomorphic [simple right $R$-modules](../../../module-theory.md#irreducible-module). By [Schur lemma](../../../representation-theory.md#schur-s-lemma),

$$
D_i=\operatorname{End}_R(S_i)
$$

is a [division ring](../../../commutative-algebra.md#division-ring), while $\operatorname{Hom}_R(S_i,S_j)=0$ for $i\ne j$. Consequently every endomorphism preserves the isotypic summands and is a matrix of entries from $D_i$ on each one. Therefore

$$
\boxed{\operatorname{End}_R(M)\simeq
\prod_{i=1}^t M_{m_i}(D_i).}
$$

If the ground field is algebraically closed and the $S_i$ are finite-dimensional over it, [Schur lemma](../../../representation-theory.md#schur-s-lemma) gives $D_i=k$.

## 4

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A vertex $i$ of a [quiver](../../../algebra.md#quiver) is a [sink](../../../algebra.md#sink-of-a-quiver) when no arrow starts at $i$. A [representation of a quiver](../../../algebra.md#representation-of-a-quiver) assigns a vector space $V_j$ to every vertex and a linear map $V_a:V_j\to V_\ell$ to every arrow $a:j\to\ell$. A morphism $f:V\to W$ is a family of linear maps $f_j:V_j\to W_j$ such that $f_\ell V_a=W_af_j$ for every arrow. The quiver has [finite representation type](../../../algebra.md#finite-representation-type-of-a-quiver) when it has only finitely many isomorphism classes of indecomposable finite-dimensional representations.

At a sink $i$, the [Bernstein–Gelfand–Ponomarev reflection functor](../../../algebra.md#bernstein-gelfand-ponomarev-reflection-functor) replaces

$$
V_i\quad\text{by}\quad
\ker\left(\bigoplus_{a:j\to i}V_j\longrightarrow V_i\right)
$$

and reverses the arrows ending at $i$; the new arrow maps are the kernel inclusion followed by the coordinate projections. Every representation is a direct sum of copies of the simple representation $S_i$ and a representation for which the displayed incoming map is surjective. On the latter representations, reflection at the resulting source, using the corresponding cokernel, is inverse up to natural isomorphism. Thus reflection gives a bijection between indecomposable representations other than $S_i$ on the two sides. Adding the one omitted simple representation on each side proves that reversing all arrows into a sink preserves finite representation type.

For the four-arrow star $Q_1$, take $V_1=\cdots=V_4=k$, $V_5=k^2$, and let the four arrows have images

$$
k(1,0),\quad k(0,1),\quad k(1,1),\quad k(1,\lambda),
\qquad \lambda\in k\setminus\{0,1\}.
$$

An endomorphism must preserve the first two lines, so its map on $V_5$ is diagonal. Preserving the third forces its diagonal entries to agree, and then all vertex maps are multiplication by that same scalar. The endomorphism ring is therefore $k$, so this representation is a [brick module](../../../module-theory.md#brick-module) and hence indecomposable. Any isomorphism between parameters preserves the first three labelled lines; the induced [projective linear transformation](../../../projective-space.md#projective-linear-transformation) is therefore the identity, and the fourth line gives $\lambda=\mu$. Since $k$ is infinite, this is an infinite family of pairwise nonisomorphic indecomposables. Hence $Q_1$ is not of finite representation type. Repeatedly applying the reflection result to sinks or, dually, to sources shows that every orientation obtained by reversing some of its arrows also has infinite representation type.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
