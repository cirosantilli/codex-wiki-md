# Paper 1

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_1.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_1.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For the [Adjoint representation of a Lie algebra](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra), the operator associated with $x\in L$ is

$$
\operatorname{ad}_x(y)=[x,y].
$$

The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) gives $[\operatorname{ad}_x,\operatorname{ad}_y]=\operatorname{ad}_{[x,y]}$, so this really is a [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation). Define the [lower central series of a Lie algebra](../../../lie-algebra.md#lower-central-series-of-a-lie-algebra) by $L^1=L$ and $L^{r+1}=[L,L^r]$. A [nilpotent Lie algebra](../../../lie-algebra.md#nilpotent-lie-algebra) is one for which $L^{c+1}=0$ for some integer $c$. If this holds, $\operatorname{ad}_x$ carries $L^r$ into $L^{r+1}$, and consequently $(\operatorname{ad}_x)^cL=0$. This proves one implication without any condition on the field.

For the converse, we prove the linear form of the [Engel theorem](../../../lie-algebra.md#engel-s-theorem): if $A\subseteq\operatorname{End}(V)$ is a finite-dimensional [Lie algebra](../../../lie-algebra.md) consisting entirely of [nilpotent linear maps](../../../linear-operator-theory.md#nilpotent-linear-map), with $V\ne0$ finite-dimensional, then there is a nonzero vector annihilated by all of $A$. This argument works over any field.

Induct on $\dim A$. The assertion is immediate when $A=0$. First observe that if $b^m=0$, then its [commutator](../../../lie-algebra.md#commutator) action on $\operatorname{End}(V)$ is nilpotent, because

$$
(\operatorname{ad}_b)^r(T)=\sum_{j=0}^r(-1)^j\binom rj b^{r-j}Tb^j=0\qquad(r\ge2m-1).
$$

Let $B$ be a proper [Lie subalgebra](../../../lie-algebra.md#lie-subalgebra) of $A$. The [commutator](../../../lie-algebra.md#commutator) action of $B$ on $A/B$ therefore consists of [nilpotent linear maps](../../../linear-operator-theory.md#nilpotent-linear-map). Its image has dimension at most $\dim B<\dim A$, so induction supplies a nonzero coset $a+B$ annihilated by $B$. Thus $[B,a]\subseteq B$, and the normalizer $N_A(B)=\{a\in A:[a,B]\subseteq B\}$ strictly contains $B$. This is the [Engel normalizer lemma](../../../lie-algebra.md#engel-normalizer-lemma).

Choose $B$ maximal among proper [Lie subalgebras](../../../lie-algebra.md#lie-subalgebra). Its normalizer must be $A$, so $B$ is a [Lie algebra ideal](../../../lie-algebra.md#ideal-of-a-lie-algebra). Moreover $\dim(A/B)=1$: otherwise the inverse image of a one-dimensional subalgebra of $A/B$ would lie strictly between $B$ and $A$. By induction,

$$
W=\{v\in V:bv=0\text{ for all }b\in B\}\ne0.
$$

Since $B$ is an ideal, $W$ is $A$-invariant: $b(av)=a(bv)+[b,a]v=0$. Take $x\in A\setminus B$. Its restriction to $W$ is nilpotent and hence has a nonzero kernel. A nonzero vector in that kernel is annihilated by $B$ and $x$, and therefore by all of $A$. This completes the induction.

Apply this result successively to $V$, then its quotient by a common annihilated line, and so on. We obtain a complete flag $0=V_0\subset V_1\subset\cdots\subset V_n=V$ with $AV_i\subseteq V_{i-1}$. Equivalently every element of $A$ is strictly upper triangular in one common basis; any product of $n$ such operators is zero.

Now take $V=L$ and $A=\operatorname{ad}(L)$. The hypothesis supplies exactly the nilpotence needed above. Every iterated bracket of length $n+1$, where $n=\dim L$, is an application of $n$ adjoint operators and vanishes. These brackets span $L^{n+1}$, giving $L^{n+1}=0$. The zero algebra is already nilpotent. Thus **$L$ is nilpotent if and only if every $\operatorname{ad}_x$ is nilpotent**. The common flag is essential: separate nilpotence of unrelated operators would not imply that their mixed products vanish.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use the [derived series of a Lie algebra](../../../lie-algebra.md#derived-series-of-a-lie-algebra)

$$
L^{(0)}=L,\qquad L^{(r+1)}=[L^{(r)},L^{(r)}].
$$

A [solvable Lie algebra](../../../lie-algebra.md#solvable-lie-algebra) has $L^{(r)}=0$ for some $r$. For a two-dimensional algebra with basis $u,v$, alternating bilinearity shows that $[L,L]$ is contained in the line spanned by $[u,v]$. A one-dimensional [Lie algebra](../../../lie-algebra.md) is abelian, so $[[L,L],[L,L]]=0$. **Every two-dimensional complex [Lie algebra](../../../lie-algebra.md) is solvable, with derived length at most two.** This dimension argument actually works over any field with the alternating definition of a [Lie bracket](../../../lie-algebra.md#lie-bracket).

There is a genuine qualification in the last request: the assertion about all [Irreducible Lie algebra representations](../../../lie-algebra.md#irreducible-lie-algebra-representation) is true for finite-dimensional representations. Without that restriction, the [infinite-dimensional simple module for the two-dimensional affine Lie algebra](../../../lie-algebra.md#infinite-dimensional-simple-module-for-the-two-dimensional-affine-lie-algebra) is a counterexample. Take $L=\mathbb Cx\oplus\mathbb Cy$, with $[x,y]=y$, and let it act on $V=\mathbb C[t]$ by

$$
(xf)(t)=tf(t),\qquad(yf)(t)=f(t-1).
$$

Then $[x,y]f=tf(t-1)-(t-1)f(t-1)=yf$, so this is a [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation). Any nonzero [submodule](../../../module-theory.md#submodule) is stable under multiplication by $t$, hence is an ideal $p(t)\mathbb C[t]$. Stability under $y$ implies $p(t)\mid p(t-1)$. The two [polynomials](../../../polynomial.md) have the same degree; their leading coefficients also agree, so $p(t-1)=p(t)$. In characteristic zero this forces $p$ to be constant. Thus $V$ is infinite-dimensional and irreducible, while $L$ is solvable. **The literal unrestricted assertion is false.**

Here is a proof of the intended finite-dimensional assertion, including the essential [Lie theorem](../../../lie-algebra.md#lie-s-theorem) argument. We prove that a nonzero finite-dimensional representation $\rho:L\to\operatorname{End}(V)$ of a complex solvable algebra has a common [eigenvector](../../../linear-operator-theory.md#eigenvector), by induction on $\dim L$. If $L=0$, any nonzero vector works. Otherwise $[L,L]\ne L$; choose a hyperplane $K$ containing $[L,L]$. It is a solvable ideal, and $L=K\oplus\mathbb Cx$. Induction gives $v\ne0$ and $\lambda\in K^*$ with $\rho(y)v=\lambda(y)v$ for all $y\in K$. Write $X=\rho(x)$ and suppress $\rho$ on elements of $K$.

Let $v_j=X^jv$ and let $m$ be the first index for which $v_m$ lies in the span of $v_0,\ldots,v_{m-1}$. The space $W=\operatorname{span}(v_0,\ldots,v_{m-1})$ is $X$-invariant. Repeatedly using $yX=Xy+[y,x]$ and $[y,x]\in K$ proves inductively that

$$
yv_j-\lambda(y)v_j\in\operatorname{span}(v_0,\ldots,v_{j-1}).
$$

Thus $W$ is $K$-invariant, and every $y\in K$ has constant diagonal $\lambda(y)$ in this basis. The [trace](../../../linear-algebra.md#matrix-trace) of a [commutator](../../../lie-algebra.md#commutator) is zero, so

$$
0=\operatorname{tr}_W[X,y]=m\lambda([x,y]).
$$

Since we work over $\mathbb C$, $\lambda([x,y])=0$ for all $y\in K$. Therefore the nonzero simultaneous [eigenspace](../../../linear-operator-theory.md#eigenspace)

$$
V_\lambda=\{w\in V:yw=\lambda(y)w\text{ for every }y\in K\}
$$

is $X$-invariant: $yXw=\lambda(y)Xw+\lambda([y,x])w=\lambda(y)Xw$. A complex linear operator on a nonzero finite-dimensional space has an [eigenvector](../../../linear-operator-theory.md#eigenvector). An [eigenvector](../../../linear-operator-theory.md#eigenvector) of $X|_{V_\lambda}$ is consequently a common [eigenvector](../../../linear-operator-theory.md#eigenvector) for $L$.

Its span is a one-dimensional [submodule](../../../module-theory.md#submodule). If $V$ is irreducible, that span must be all of $V$. Hence **every finite-dimensional irreducible representation of a finite-dimensional complex solvable [Lie algebra](../../../lie-algebra.md) has dimension one**. Conversely a one-dimensional representation is given by a [linear functional](../../../linear-algebra.md#linear-functional) on $L/[L,L]$, because every [commutator](../../../lie-algebra.md#commutator) acts by zero. Passing repeatedly to quotients also gives the [simultaneous triangularization of a Lie algebra representation](../../../lie-algebra.md#simultaneous-triangularization-of-a-lie-algebra-representation). Neither the [eigenvector](../../../linear-operator-theory.md#eigenvector) step nor the [trace](../../../linear-algebra.md#matrix-trace) argument extends to the infinite-dimensional counterexample above.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A finite-dimensional complex [Lie algebra](../../../lie-algebra.md) is a [semisimple Lie algebra](../../../semisimple-lie-algebra.md) when its [solvable radical](../../../lie-algebra.md#radical-of-a-lie-algebra) is zero, equivalently when it has no nonzero solvable ideals. Its [Killing form](../../../lie-algebra.md#killing-form) is the [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form)

$$
B_L(x,y)=\operatorname{tr}_L(\operatorname{ad}_x\operatorname{ad}_y).
$$

The cyclic [trace](../../../linear-algebra.md#matrix-trace) identity and $\operatorname{ad}_{[z,x]}=[\operatorname{ad}_z,\operatorname{ad}_x]$ give

$$
B_L([z,x],y)+B_L(x,[z,y])=0.
$$

Thus the [Killing form](../../../lie-algebra.md#killing-form) is an [invariant bilinear form on a Lie algebra](../../../lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra). In particular its radical $R=\{x:B_L(x,L)=0\}$ is an ideal.

We supply the [trace](../../../linear-algebra.md#matrix-trace) argument needed for nondegeneracy rather than assuming the [Cartan criterion for semisimplicity](../../../lie-algebra.md#cartan-criterion-for-semisimplicity). The matrix form of the [Cartan solvability criterion](../../../lie-algebra.md#cartan-solvability-criterion) says: if $A\subseteq\operatorname{End}_{\mathbb C}(V)$ and $\operatorname{tr}(uv)=0$ for every $u\in[A,A]$, $v\in A$, then $A$ is solvable. To prove this direction, fix $u\in[A,A]$. Let $V=\bigoplus_\lambda V_\lambda$ be its [generalized eigenspace](../../../linear-operator-theory.md#generalized-eigenspace) decomposition, and define $s$ to act on $V_\lambda$ by the scalar $\overline\lambda$. On $\operatorname{Hom}(V_\mu,V_\lambda)$, the semisimple part of $\operatorname{ad}_u$ has [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda-\mu$, whereas $\operatorname{ad}_s$ acts by $\overline\lambda-\overline\mu=\overline{\lambda-\mu}$. [Polynomial interpolation](../../../numerical-analysis.md#polynomial-interpolation) on the finitely many [eigenvalues](../../../linear-operator-theory.md#eigenvalue), with all derivatives through the sizes of the nilpotent blocks set to zero, therefore gives

$$
\operatorname{ad}_s=p(\operatorname{ad}_u),\qquad p(0)=0.
$$

Here the same difference always has the same conjugate, so the interpolation is consistent; the prescribed zero derivatives remove every nilpotent block. Since $\operatorname{ad}_u(A)\subseteq[A,A]$, it follows that $[s,A]\subseteq[A,A]$.

Write $u=\sum_j[a_j,b_j]$. By cyclicity and the [trace](../../../linear-algebra.md#matrix-trace) hypothesis,

$$
\operatorname{tr}(us)=\sum_j\operatorname{tr}(a_j[b_j,s])=0.
$$

On the other hand, $\operatorname{tr}(us)=\sum_\lambda\dim(V_\lambda)|\lambda|^2$. Thus all [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $u$ vanish, and every element of $[A,A]$ is nilpotent. The [Engel theorem](../../../lie-algebra.md#engel-s-theorem) makes $[A,A]$ nilpotent as a [Lie algebra](../../../lie-algebra.md), hence solvable; $A/[A,A]$ is abelian, so $A$ is solvable. This is the [Conjugate-spectrum proof of Cartan solvability](../../../lie-algebra.md#conjugate-spectrum-proof-of-cartan-solvability).

Apply this to the Killing radical $R$. For $x,y\in R$, the adjoint actions preserve $R$ and act as zero on $L/R$, because $R$ is an ideal. Computing traces in a basis adapted to $R$ gives

$$
B_R(x,y)=B_L(x,y)=0.
$$

The matrix [Lie algebra](../../../lie-algebra.md) $\operatorname{ad}_R(R)$ consequently satisfies the [trace](../../../linear-algebra.md#matrix-trace) criterion and is solvable. Its kernel is $Z(R)$, an abelian ideal; a central extension of a solvable algebra is solvable. Thus $R$ is solvable. This proves the reusable assertion that the [Killing radical is a solvable ideal](../../../lie-algebra.md#killing-radical-is-a-solvable-ideal). Semisimplicity forces $R=0$, and hence **$B_L$ is nondegenerate**.

A [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) is a nilpotent subalgebra $H$ which is self-normalizing:

$$
N_L(H)=\{x\in L:[x,H]\subseteq H\}=H.
$$

For a complex semisimple algebra this is equivalently a maximal toral subalgebra. The nilpotent, self-normalizing definition permits a proof of the restricted nondegeneracy without first assuming the toral characterization.

Use the [generalized-weight decomposition for a nilpotent Lie algebra](../../../semisimple-lie-algebra.md#generalized-weight-decomposition-for-a-nilpotent-lie-algebra) for the adjoint action of $H$:

$$
L=\bigoplus_\lambda L^\lambda,\qquad
L^\lambda=\{v:(\operatorname{ad}_h-\lambda(h)I)^{\dim L}v=0\text{ for all }h\in H\}.
$$

For completeness, the stability underlying this decomposition follows directly from nilpotence of $H$. For fixed $h$, every $\operatorname{ad}_h$ on $H$ is nilpotent. If $T=\rho(h)$ and $S=\rho(y)$ in a finite-dimensional representation, then $(\operatorname{ad}_T)^rS=0$ for sufficiently large $r$. The identity

$$
(T-aI)^N S=\sum_{j=0}^N\binom Nj (\operatorname{ad}_T)^j(S)(T-aI)^{N-j}
$$

shows that $S$ preserves each [generalized eigenspace](../../../linear-operator-theory.md#generalized-eigenspace) of $T$. Starting with a basis of $H$, refine these primary decompositions successively; all summands remain $H$-invariant. Each resulting summand has only one [eigenvalue](../../../linear-operator-theory.md#eigenvalue) for each basis element. The [Lie theorem](../../../lie-algebra.md#lie-s-theorem) triangularizes the action on that summand, so those [eigenvalues](../../../linear-operator-theory.md#eigenvalue) extend to a single linear character $\lambda$ on all of $H$. This proves the displayed decomposition and nilpotence of all shifted operators there.

Since $H$ is nilpotent, $H\subseteq L^0$. The space $L^0$ is a subalgebra: repeated use of the derivation rule for $\operatorname{ad}_h$ shows that the bracket of two generalized zero-[eigenvectors](../../../linear-operator-theory.md#eigenvector) is another such vector. If $L^0/H\ne0$, the adjoint action of $H$ on this quotient consists entirely of nilpotent maps. The [Engel theorem](../../../lie-algebra.md#engel-s-theorem) supplies a nonzero coset $x+H$ with $[H,x]\subseteq H$, contradicting self-normalization. Therefore the [zero generalized weight space of a Cartan subalgebra](../../../semisimple-lie-algebra.md#zero-generalized-weight-space-of-a-cartan-subalgebra) is exactly $H$.

Finally, $B_L(H,L^\lambda)=0$ when $\lambda\ne0$. Choose $h\in H$ with $\lambda(h)\ne0$ and put $T=\operatorname{ad}_h$. On $H$, a power $T^m$ vanishes. On $L^\lambda$, $T$ is invertible. For $u\in H$ and $v\in L^\lambda$, write $v=T^m w$; invariance gives

$$
B_L(u,v)=B_L(u,T^m w)=(-1)^mB_L(T^m u,w)=0.
$$

If $u\in H$ is orthogonal to $H$, it is now orthogonal to every summand of $L$, so nondegeneracy of $B_L$ implies $u=0$. **The restriction $B_L|_{H\times H}$ is nondegenerate.** This establishes the [nondegeneracy of the Killing form on a Cartan subalgebra](../../../semisimple-lie-algebra.md#nondegeneracy-of-the-killing-form-on-a-cartan-subalgebra) for every [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra), without requiring a chosen root basis.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) $V$ is completely reducible when it is a [direct sum](../../../vector-space.md#direct-sum) of irreducible [submodules](../../../module-theory.md#submodule). In finite dimension this is equivalent to saying that every [submodule](../../../module-theory.md#submodule) $W\subseteq V$ has an invariant complementary subspace. Indeed, one may split off a minimal nonzero [submodule](../../../module-theory.md#submodule) and induct on dimension; conversely, if $V$ is a finite sum of simple [submodules](../../../module-theory.md#submodule), choose a maximal sum $U$ of these with $U\cap W=0$. If $W+U\ne V$, some simple summand $S$ is not contained in $W+U$. Then $S\cap(W+U)=0$ by simplicity, so $U+S$ is a larger sum disjoint from $W$, a contradiction. Thus $V=W\oplus U$.

We prove the required splitting by [Haar averaging produces invariant complements](../../../semisimple-lie-algebra.md#haar-averaging-produces-invariant-complements). The structural input is the [compact real form of a complex semisimple Lie algebra](../../../semisimple-lie-algebra.md#compact-real-form-of-a-complex-semisimple-lie-algebra): there is a real semisimple algebra $\mathfrak k$ with $L=\mathfrak k\oplus i\mathfrak k$, whose simply connected integrating Lie group $K$ is compact. This structural fact is independent of the complete-reducibility assertion. One standard construction uses [root vectors](../../../semisimple-lie-algebra.md#root-vector) normalized so that $[e_\alpha,e_{-\alpha}]=h_\alpha$, with real structure constants compatible with the involution $e_\alpha\mapsto-e_{-\alpha}$ and $h_\alpha\mapsto-h_\alpha$. The real span

$$
\mathfrak k=\operatorname{span}_{\mathbb R}\{ih_i,\ e_\alpha-e_{-\alpha},\ i(e_\alpha+e_{-\alpha}):\alpha>0\}
$$

is closed under brackets, complexifies to $L$, and has negative-definite [Killing form](../../../lie-algebra.md#killing-form). The compactness criterion for real semisimple [Lie algebras](../../../lie-algebra.md) then gives a compact simply connected $K$. Thus this route uses root structure and compact integration, not the theorem being proved.

Restrict $\rho:L\to\operatorname{End}_{\mathbb C}(V)$ to $\mathfrak k$. The [integration of a Lie-algebra representation](../../../lie-algebra.md#integration-of-a-lie-algebra-representation) gives a representation $R:K\to\operatorname{GL}_{\mathbb C}(V)$, since $K$ is simply connected. Choose any positive-definite [Hermitian inner product](../../../linear-algebra.md#hermitian-form) $\langle\ ,\ \rangle_0$ and average using normalized [Haar measure](../../../measure-theory.md#haar-measure):

$$
\langle v,w\rangle_K=\int_K\langle R(g)v,R(g)w\rangle_0\,d\mu(g).
$$

The integral exists by compactness. It is positive-definite because $R(g)v\ne0$ for $v\ne0$, and it is $K$-invariant by translation invariance of [Haar measure](../../../measure-theory.md#haar-measure). Equivalently, every $\rho(a)$ with $a\in\mathfrak k$ is skew-Hermitian for this inner product.

Let $W$ be an $L$-[submodule](../../../module-theory.md#submodule). It is invariant under $\mathfrak k$, hence under the exponentials generating the connected group $K$. For $v\in W^\perp$, $w\in W$ and $g\in K$,

$$
\langle R(g)v,w\rangle_K=\langle v,R(g^{-1})w\rangle_K=0.
$$

Consequently the [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) $W^\perp$ is $K$-invariant, and differentiation makes it $\mathfrak k$-invariant. It is a complex vector subspace, so it is also invariant under $i\mathfrak k$ and hence under $L$. Therefore $V=W\oplus W^\perp$ as $L$-[modules](../../../module-theory.md#module-mathematics).

Induction on $\dim V$ now expresses $V$ as a finite [direct sum](../../../vector-space.md#direct-sum) of irreducible [submodules](../../../module-theory.md#submodule). **Every finite-dimensional representation of a finite-dimensional complex semisimple [Lie algebra](../../../lie-algebra.md) is completely reducible.** The compact real form need not be the real form originally used to present $L$; in particular the averaging argument does not require the given presentation to be unitary.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Here [root systems](../../../semisimple-lie-algebra.md#root-system) are finite, reduced and crystallographic, as for complex semisimple [Lie algebras](../../../lie-algebra.md). For a [base of a root system](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system) $\Delta=\{\alpha_1,\ldots,\alpha_r\}$, the [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) has one vertex for each [simple root](../../../semisimple-lie-algebra.md#simple-root). Two distinct vertices have $a_{ij}a_{ji}$ bonds, with the arrow on a multiple bond pointing toward the shorter root. The [classification of finite crystallographic Dynkin diagrams](../../../semisimple-lie-algebra.md#classification-of-finite-crystallographic-dynkin-diagrams) consists of the following connected diagrams; the integers describing arms count vertices away from the unique branching vertex.

- $A_r$ ($r\ge1$): a chain with only single bonds.
- $B_r$ ($r\ge2$): a chain with one double bond at an end; that end is short.
- $C_r$ ($r\ge3$): the same bond pattern, but that end is long. The rank-two system is $C_2\cong B_2$; $C_1=A_1$.
- $D_r$ ($r\ge4$): a simply laced tree with three arms of lengths $1,1,r-3$.
- $E_6,E_7,E_8$: simply laced trees with three arms respectively of lengths $(1,2,2)$, $(1,2,3)$ and $(1,2,4)$.
- $F_4$: a four-vertex chain, with single, double, single bonds in order, and two long roots adjacent on one side of the middle bond and two short roots on the other.
- $G_2$: two vertices joined by a triple bond, one long and one short.

This is classification up to diagram isomorphism and overall rescaling of the root system. It includes the conventional identifications $D_3\cong A_3$ and $B_1\cong A_1$ when those low-rank notations are used. The weighting here encodes root lengths and bonds; it is not the separate theory of vertex labels attached to nilpotent orbits. Dropping the crystallographic or reduced hypothesis changes the classification.

Precisely, a [base of a root system](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system) is a vector-space basis $\Delta\subset\Phi$ such that each root has a unique expansion $\beta=\sum_i n_i\alpha_i$, with integer coefficients all nonnegative or all nonpositive. This defines the positive and negative roots. We use the column-coroot convention for the [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix):

$$
a_{ij}=\langle\alpha_i,\alpha_j^\vee\rangle=\frac{2(\alpha_i,\alpha_j)}{(\alpha_j,\alpha_j)},\qquad
\alpha_j^\vee=\frac{2\alpha_j}{(\alpha_j,\alpha_j)}.
$$

Some conventions transpose this matrix; specifying which index labels the coroot resolves that difference. The [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) is the subgroup of orthogonal transformations generated by the [Weyl reflections](../../../semisimple-lie-algebra.md#weyl-reflection)

$$
s_\alpha(v)=v-\frac{2(v,\alpha)}{(\alpha,\alpha)}\alpha\qquad(\alpha\in\Phi).
$$

For the [C3 root system](../../../semisimple-lie-algebra.md#c3-root-system), take an orthonormal basis $e_1,e_2,e_3$ of $\mathbb R^3$ and

$$
\Phi=\{\pm2e_i:1\le i\le3\}\ \cup\ \{\pm e_i\pm e_j:1\le i<j\le3\}.
$$

There are six long roots of squared length $4$ and twelve short roots of squared length $2$. A base is $\alpha_1=e_1-e_2$, $\alpha_2=e_2-e_3$, $\alpha_3=2e_3$. The [Cartan matrix convention for C3](../../../semisimple-lie-algebra.md#cartan-matrix-convention-for-c3) above gives

$$
\boxed{A=\begin{pmatrix}2&-1&0\\-1&2&-1\\0&-2&2\end{pmatrix}}.
$$

Thus the double bond connects $\alpha_2$ to $\alpha_3$, with its arrow directed toward $\alpha_2$.

An explicit complex [Lie algebra](../../../lie-algebra.md) realizing this root system is the [symplectic Lie algebra](../../../semisimple-lie-algebra.md#symplectic-lie-algebra)

$$
\mathfrak{sp}_6(\mathbb C)=\{X\in M_6(\mathbb C):X^TJ+JX=0\},\qquad
J=\begin{pmatrix}0&I_3\\-I_3&0\end{pmatrix}.
$$

It is closed under [commutators](../../../lie-algebra.md#commutator), since the two identities $X^TJ=-JX$, $Y^TJ=-JY$ imply $[X,Y]^TJ=-J[X,Y]$. Equivalently,

$$
X=\begin{pmatrix}A&B\\C&-A^T\end{pmatrix},\qquad B=B^T,\quad C=C^T,
$$

so its dimension is $9+6+6=21$. A [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) is

$$
H=\{\operatorname{diag}(h_1,h_2,h_3,-h_1,-h_2,-h_3)\},\qquad e_i(h)=h_i.
$$

With $E_{ab}$ denoting a matrix unit, the [root spaces](../../../semisimple-lie-algebra.md#root-space) have generators $E_{ij}-E_{3+j,3+i}$ for $e_i-e_j$ ($i\ne j$), $E_{i,3+j}+E_{j,3+i}$ for $e_i+e_j$ ($i<j$), and $E_{i,3+i}$ for $2e_i$; the analogous lower-left generators give the negative roots. These are all eighteen [root spaces](../../../semisimple-lie-algebra.md#root-space), each one-dimensional, and together with $H$ they exhaust the algebra.

For an explicit semisimplicity check, let $I\ne0$ be an ideal. Simultaneous diagonalization of $\operatorname{ad}H$ makes $I$ a sum of its intersections with $H$ and these [root spaces](../../../semisimple-lie-algebra.md#root-space). If it contains a nonzero $h\in H$, some root has $\alpha(h)\ne0$, and $[h,L_\alpha]$ supplies a [root vector](../../../semisimple-lie-algebra.md#root-vector) in $I$. Thus $I$ always contains a [root vector](../../../semisimple-lie-algebra.md#root-vector). Bracket it with its opposite [root vector](../../../semisimple-lie-algebra.md#root-vector) to obtain a nonzero coroot $h_\alpha\in I$. Whenever $(\alpha,\beta)\ne0$, bracketing $h_\alpha$ with either $L_\beta$ or $L_{-\beta}$ puts both [root spaces](../../../semisimple-lie-algebra.md#root-space) into $I$. The graph of the roots with edges for nonzero inner products is connected: $2e_i$ connects to $e_i+e_j$, which connects to $2e_j$, and every short root connects to an axis root. Repeating the argument yields all [root spaces](../../../semisimple-lie-algebra.md#root-space) and then all of $H$ from their brackets. Hence $I=L$: **the constructed algebra is simple, and therefore semisimple**.

The reflections in $e_1-e_2$ and $e_2-e_3$ exchange adjacent coordinates, while reflection in $2e_3$ changes the sign of the third coordinate. They generate every signed permutation. Conversely reflection in any displayed root is a signed permutation. Thus

$$
\boxed{W(C_3)\cong(\mathbb Z/2\mathbb Z)^3\rtimes S_3,\qquad |W(C_3)|=48}.
$$

The reflecting hyperplanes are $x_i=0$ and $x_i=\pm x_j$. A fundamental open [Weyl chamber](../../../semisimple-lie-algebra.md#fundamental-chamber-of-a-root-system) is $x_1>x_2>x_3>0$. Every regular point has three nonzero coordinates of distinct absolute values; its signs and the ordering of those absolute values specify exactly one of the $2^3\cdot3!=48$ chambers. The closure of this chamber is generated by the rays through $(1,0,0)$, $(1,1,0)$ and $(1,1,1)$. This is the [Weyl chamber geometry of C3](../../../semisimple-lie-algebra.md#weyl-chamber-geometry-of-c3).

<a id="5/image-c3-roots-and-the-spherical-tessellation-into-48-weyl-chambers"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-1-c3-roots-chambers.png)

**[Figure 1](#5/image-c3-roots-and-the-spherical-tessellation-into-48-weyl-chambers). C3 roots and the spherical tessellation into 48 Weyl chambers**.

The left panel retains the actual long and short root lengths. The right panel radially projects a hemisphere of the unit sphere, draws every visible reflecting great-circle arc, and highlights the chamber $x_1>x_2>x_3>0$. Each spherical triangle is the section of a three-dimensional chamber by the sphere; opposite triangles on the rear hemisphere supply the remaining chambers. [Roots of a root system](../../../semisimple-lie-algebra.md#root-of-a-root-system) are normal to the chamber walls, rather than generally lying along their edges.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Choose a [base of a root system](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system) and its [positive roots](../../../semisimple-lie-algebra.md#positive-root), so that the [triangular decomposition of a Lie algebra](../../../semisimple-lie-algebra.md#triangular-decomposition-of-a-lie-algebra) is $L=\mathfrak n^-\oplus H\oplus\mathfrak n^+$. A [primitive element of a Lie algebra representation](../../../semisimple-lie-algebra.md#highest-weight-vector) of weight $\omega\in H^*$ is a nonzero vector $v$ such that

$$
hv=\omega(h)v\quad(h\in H),\qquad xv=0\quad(x\in\mathfrak n^+).
$$

Equivalently it is a [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector). Being primitive depends on the chosen positive system; no integrality condition is part of this definition.

Construct the [Verma module](../../../semisimple-lie-algebra.md#verma-module) for an arbitrary $\omega$. The subalgebra $\mathfrak b=H\oplus\mathfrak n^+$ has a one-dimensional [module](../../../module-theory.md#module-mathematics) $\mathbb C_\omega$ on which $H$ acts by $\omega$ and $\mathfrak n^+$ acts by zero. This is a representation because $[\mathfrak b,\mathfrak b]\subseteq\mathfrak n^+$. Set

$$
M(\omega)=U(L)\otimes_{U(\mathfrak b)}\mathbb C_\omega,
$$

where $U$ denotes the [universal enveloping algebra](../../../lie-algebra.md#universal-enveloping-algebra). The [Poincaré-Birkhoff-Witt theorem](../../../lie-algebra.md#poincare-birkhoff-witt-theorem), applied with negative-[root vectors](../../../semisimple-lie-algebra.md#root-vector) first, then Cartan vectors and positive-[root vectors](../../../semisimple-lie-algebra.md#root-vector), gives

$$
M(\omega)\cong U(\mathfrak n^-)
$$

as vector spaces. In particular $v_\omega=1\otimes1$ is nonzero, generates $M(\omega)$, and is primitive of weight $\omega$.

The same ordered monomials show that $M(\omega)$ is a [direct sum](../../../vector-space.md#direct-sum) of weight spaces, with weights of the form

$$
\omega-\sum_{i=1}^r n_i\alpha_i,\qquad n_i\in\mathbb Z_{\ge0},
$$

and that its weight-$\omega$ space is exactly $\mathbb Cv_\omega$. Each vector has only finitely many weight components. If a [submodule](../../../module-theory.md#submodule) contains a vector with nonzero weight-$\omega$ component, choose $h\in H$ that separates $\omega$ from the finitely many other weights of that vector. [Polynomial interpolation](../../../numerical-analysis.md#polynomial-interpolation) in the action of $h$ extracts a nonzero multiple of $v_\omega$. Such a [submodule](../../../module-theory.md#submodule) is all of $M(\omega)$, because $v_\omega$ generates it. Consequently every proper [submodule](../../../module-theory.md#submodule) has zero component in weight $\omega$.

Let $N$ be the sum of all proper [submodules](../../../module-theory.md#submodule). Every finite sum still has zero weight-$\omega$ component, so $N$ is proper; it contains every proper [submodule](../../../module-theory.md#submodule) and is therefore the unique maximal proper [submodule](../../../module-theory.md#submodule). Its quotient

$$
\boxed{L(\omega)=M(\omega)/N}
$$

is irreducible, and the nonzero image of $v_\omega$ is primitive of weight $\omega$. This proves existence for every $\omega\in H^*$ and gives the [irreducible quotient of a Verma module](../../../semisimple-lie-algebra.md#irreducible-quotient-of-a-verma-module). It also proves uniqueness up to isomorphism among irreducible [modules](../../../module-theory.md#module-mathematics) generated by a primitive vector of that weight: the defining relations induce a surjection from $M(\omega)$, whose proper kernel must be $N$.

These [modules](../../../module-theory.md#module-mathematics) are not generally finite-dimensional. For example, in an $\mathfrak{sl}_2$ root subalgebra, a primitive vector with $hv=\lambda v$ satisfies

$$
e f^k v=k(\lambda-k+1)f^{k-1}v.
$$

If its irreducible highest-weight [module](../../../module-theory.md#module-mathematics) is finite-dimensional, the weight-lowering sequence eventually stops. For the first $m$ with $f^{m+1}v=0$ and $f^mv\ne0$, the identity forces $\lambda=m\in\mathbb Z_{\ge0}$. In general a finite-dimensional highest-weight [module](../../../module-theory.md#module-mathematics) therefore requires nonnegative integral values on all [simple coroots](../../../semisimple-lie-algebra.md#simple-coroot); arbitrary $\omega$ in the request must allow infinite-dimensional representations. This is consistent with the finite-dimensional qualification made in Question 2.

For [simple coroots](../../../semisimple-lie-algebra.md#simple-coroot) $h_1,\ldots,h_r$ forming a basis of $H$, the [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight) are the [dual basis](../../../linear-algebra.md#dual-basis) $\omega_1,\ldots,\omega_r\in H^*$:

$$
\omega_i(h_j)=\delta_{ij}.
$$

For the [special linear Lie algebra](../../../semisimple-lie-algebra.md#special-linear-lie-algebra) $\mathfrak{sl}_3(\mathbb C)$, take the diagonal [trace](../../../linear-algebra.md#matrix-trace)-zero [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) and [positive roots](../../../semisimple-lie-algebra.md#positive-root) corresponding to upper triangular matrix units. Write $\varepsilon_i(\operatorname{diag}(t_1,t_2,t_3))=t_i$. The [simple roots](../../../semisimple-lie-algebra.md#simple-root) are $\alpha_1=\varepsilon_1-\varepsilon_2$, $\alpha_2=\varepsilon_2-\varepsilon_3$, and the [simple coroots](../../../semisimple-lie-algebra.md#simple-coroot) are

$$
h_1=\operatorname{diag}(1,-1,0),\qquad h_2=\operatorname{diag}(0,1,-1).
$$

The [fundamental weights of sl3](../../../semisimple-lie-algebra.md#fundamental-weights-of-sl3) are therefore

$$
\boxed{\omega_1(\operatorname{diag}(t_1,t_2,t_3))=t_1,\qquad
\omega_2(\operatorname{diag}(t_1,t_2,t_3))=t_1+t_2=-t_3}.
$$

Checking these on $h_1,h_2$ gives the two coordinate vectors $(1,0)$ and $(0,1)$. In the Euclidean [trace](../../../linear-algebra.md#matrix-trace)-zero plane they can also be written

$$
\omega_1=\frac{2\alpha_1+\alpha_2}{3}=\left(\frac23,-\frac13,-\frac13\right),\qquad
\omega_2=\frac{\alpha_1+2\alpha_2}{3}=\left(\frac13,\frac13,-\frac23\right).
$$

The [Fundamental representations of sl3](../../../semisimple-lie-algebra.md#fundamental-representations-of-sl3) make these weights concrete: $\mathbb C^3$ has primitive vector $e_1$ of weight $\omega_1$, and $\Lambda^2\mathbb C^3$ has primitive vector $e_1\wedge e_2$ of weight $\omega_2$. Every finite-dimensional irreducible highest weight is $a\omega_1+b\omega_2$ with nonnegative integers $a,b$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
