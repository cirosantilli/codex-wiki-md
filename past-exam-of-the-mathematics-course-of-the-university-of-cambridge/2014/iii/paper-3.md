# Paper 3

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_3.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_3.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)

## 1

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write a finite [quiver](../../../algebra.md#quiver) as $Q=(Q_0,Q_1,s,t)$, with vertex and arrow sets and source/target maps. A [representation of a quiver](../../../algebra.md#representation-of-a-quiver) assigns a [vector space](../../../vector-space.md) $X_i$ to each vertex and a [linear map](../../../vector-space.md#linear-map) $f_\rho:X_{s(\rho)}\to X_{t(\rho)}$ to each arrow. A [quiver representation morphism](../../../algebra.md#quiver-representation-morphism) $h:X\to Y$ is a family satisfying $h_{t(\rho)}f_\rho=g_\rho h_{s(\rho)}$.

The [path algebra](../../../algebra.md#path-algebra) $A=kQ$ has every directed path, including each length-zero path $e_i$, as a [basis](../../../vector-space.md#basis). Multiplication is composition when endpoints match, and zero otherwise; in $pq$, the path $q$ is traversed first. The [orthogonal idempotents](../../../commutative-algebra.md#orthogonal-idempotent) satisfy $1=\sum_ie_i$.

The [path-algebra module equivalence](../../../algebra.md#path-algebra-module-equivalence) is explicit. From a representation, form $M=\bigoplus_iX_i$, let $e_i$ project onto $X_i$, and let each path act by the composite of its arrow maps. Conversely, an $A$-[module](../../../module-theory.md#module-mathematics) gives $X_i=e_iM$ and $f_\rho(x)=\rho x$. An $A$-[module homomorphism](../../../module-theory.md#module-homomorphism) restricts to the required vertex maps, and a compatible family extends by direct sum. These constructions are mutually inverse up to their evident natural identifications.

**$kQ$ is finite-dimensional exactly when $Q$ is finite and has no oriented cycle.** For a finite [acyclic quiver](../../../algebra.md#acyclic-quiver), paths have length at most $|Q_0|-1$. An oriented cycle has arbitrarily many distinct powers, giving infinitely many basis paths. If arbitrary infinite quivers are allowed, finiteness of both vertices and arrows is also necessary; the unital module correspondence above uses finite $Q_0$.

Choose only the orientation $1\to2\to3$. The [interval representations of an equioriented three-vertex quiver](../../../algebra.md#interval-representations-of-an-equioriented-three-vertex-quiver) $I[a,b]$ have $k$ at vertices $a,\ldots,b$, zero elsewhere, and identity arrows within that interval. The complete list is

$$
\boxed{I[1,1],\ I[2,2],\ I[3,3],\ I[1,2],\ I[2,3],\ I[1,3]}.
$$

Here is an elementary proof, without the [Gabriel theorem](../../../algebra.md#gabriel-s-theorem). For $X_1\xrightarrow fX_2\xrightarrow gX_3$, set $K=\operatorname{im}f\cap\ker g$. Choose $F$ complementing $K$ in $\operatorname{im}f$, $G$ complementing $K$ in $\ker g$, and $H$ complementing $\operatorname{im}f+\ker g$ in $X_2$. Then $X_2=K\oplus F\oplus G\oplus H$, and $g$ is injective on $F\oplus H$. Lift bases of $K,F$ to a complement of $\ker f$ in $X_1$, and extend the bases of $gF,gH$ to $X_3$. These bases split $X$ into precisely the six kinds of interval block. Every block has [endomorphism ring](../../../module-theory.md#endomorphism-ring) $k$, hence is indecomposable, and their different supports make them pairwise nonisomorphic. The same basis argument handles arbitrary vertex dimensions; each indecomposable block itself is finite-dimensional.

## 2

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a finite [acyclic quiver](../../../algebra.md#acyclic-quiver), the [arrow ideal of a path algebra](../../../algebra.md#arrow-ideal-of-a-path-algebra) $R$ is nilpotent, and $A/R\cong\prod_{i\in Q_0}k$. If $S$ is a [simple module](../../../module-theory.md#irreducible-module), its [submodule](../../../module-theory.md#submodule) $RS$ is either zero or $S$. The latter would imply $R^dS=S$ for every $d$, contradicting nilpotence. Thus $RS=0$, and a simple module over the product of fields is supported at one coordinate. Therefore **the simples are exactly $S(i)$**, with $k$ at $i$, zero elsewhere, and zero arrows; the vertex $i$ is unique.

A finite-dimensional [semisimple module](../../../module-theory.md#semisimple-module) is consequently $\bigoplus_iS(i)^{\oplus n_i}$, where $n_i=\dim X_i$. Its [dimension vector of a quiver representation](../../../algebra.md#dimension-vector-of-a-quiver-representation) determines its isomorphism class.

For an arbitrary finite quiver, cycles allowed, the [vertex projective module of a path algebra](../../../algebra.md#vertex-projective-module-of-a-path-algebra) is $P(i)=Ae_i$. Its space at vertex $j$ has [basis](../../../vector-space.md#basis) all paths from $i$ to $j$, and an arrow acts by adjoining that arrow at the end of the path. Its [endomorphism ring](../../../module-theory.md#endomorphism-ring) is

$$
\boxed{\operatorname{End}_A(P(i))\cong(e_iAe_i)^{\mathrm{op}}},
$$

where $e_iAe_i$ is spanned by the closed paths based at $i$. The opposite multiplication appears because endomorphisms act by right multiplication.

The [evaluation isomorphism for a vertex projective](../../../algebra.md#evaluation-isomorphism-for-a-vertex-projective) is

$$
\boxed{\operatorname{Hom}_Q(P(i),X)\longrightarrow X_i,\qquad h\longmapsto h(e_i)}.
$$

For $x\in X_i$, its inverse sends a path $p$ starting at $i$ to $px$. This proves both injectivity and surjectivity, and is natural in $X$. Vertex evaluation is exact, so $P(i)$ is a [projective module](../../../module-theory.md#projective-module); alternatively it is a direct summand of the free module $A$.

The [closed-path corner of a path algebra is a domain](../../../algebra.md#closed-path-corner-of-a-path-algebra-is-a-domain): in a product of two nonzero linear combinations, choose their longest path lengths. Concatenation in that top degree has a unique cut at those lengths, so a product of two nonzero top coefficients cannot cancel. Hence its only [idempotents](../../../commutative-algebra.md#idempotent) are zero and one. The same is true of the opposite ring, proving $P(i)$ is an [indecomposable module](../../../module-theory.md#indecomposable-module), even when cycles make it infinite-dimensional.

For $1\to2\leftarrow3$, the paths starting at vertex $1$ are $e_1$ and the arrow $1\to2$. Thus the displayed $k\xrightarrow{1}k\leftarrow0$ is **$P(1)$ and is projective**.

## 3

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [extension group](../../../algebra.md#extension-group) $\operatorname{Ext}^1_Q(V,W)$ consists of equivalence classes of [short exact sequences](../../../module-theory.md#short-exact-sequence) $0\to W\to E\to V\to0$, with the zero class represented by a split sequence and addition given by the [Baer sum](../../../algebra.md#baer-sum). The [extension complex of quiver representations](../../../algebra.md#extension-complex-of-quiver-representations) gives

$$
0\to\operatorname{Hom}_Q(V,W)\to\bigoplus_i\operatorname{Hom}_k(V_i,W_i)\xrightarrow{\gamma_{V,W}}\bigoplus_{\rho:i\to j}\operatorname{Hom}_k(V_i,W_j)\to\operatorname{Ext}^1_Q(V,W)\to0.
$$

The printed map has $\gamma(u)_\rho=u_jf_\rho-g_\rho u_i$, so its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is $\operatorname{Hom}_Q(V,W)$ and its [cokernel](../../../linear-algebra.md#cokernel) is $\operatorname{Ext}^1_Q(V,W)$. Reversing the overall differential sign changes neither identification.

For dimension vectors $\mathbf v,\mathbf w$, the [Ringel form](../../../algebra.md#ringel-form) is

$$
\boxed{\langle\mathbf v,\mathbf w\rangle_Q=\sum_iv_iw_i-\sum_{\rho:i\to j}v_iw_j=\dim\operatorname{Hom}_Q(V,W)-\dim\operatorname{Ext}^1_Q(V,W)}.
$$

The first expression makes its dependence only on the dimension vectors explicit.

For the one-loop representation $V=k$ with loop scalar $\lambda$, $\gamma(u)=u\lambda-\lambda u=0$ on $k$. Both cochain spaces have dimension one, so **$\dim\operatorname{Ext}^1_Q(V,V)=1$**, for every $\lambda$. Concretely, a self-extension has loop matrix $\left(\begin{smallmatrix}\lambda&c\\0&\lambda\end{smallmatrix}\right)$, with $c$ the extension parameter.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [four-subspace quiver](../../../algebra.md#four-subspace-quiver) has four one-dimensional sources and a two-dimensional sink. Its [Tits form of a quiver](../../../algebra.md#tits-form-of-a-quiver) at this dimension vector is $q=4\cdot1^2+2^2-4(1\cdot2)=0$.

An [endomorphism](../../../algebra.md#endomorphism) comprises source scalars $a_1,\ldots,a_4$ and a sink matrix $T$. The first two columns $e_1,e_2$ force $T=\operatorname{diag}(a_1,a_2)$. The third column $e_1+e_2$ then forces $a_1=a_2=a_3$, making $T$ scalar. Since the fourth column $(\lambda,1)^T$ is always nonzero, its scalar is also the same, for every $\lambda$.

Thus $\operatorname{End}_Q(V)=k$, so the representation is a [brick module](../../../module-theory.md#brick-module). The [Ringel form](../../../algebra.md#ringel-form) gives

$$
\boxed{\dim\operatorname{Ext}^1_Q(V,V)=\dim\operatorname{End}_Q(V)-q=1}.
$$

This conclusion also covers $\lambda=0,1$, where the fourth line repeats one of the earlier lines; the first three lines already force scalar endomorphisms.

## 4

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [unipotent algebraic group](../../../lie-theory.md#unipotent-algebraic-group) admits a faithful linear representation in which every group element is a [unipotent matrix](../../../lie-theory.md#unipotent-matrix). For $E=\operatorname{End}_Q(X)$, invertibility is the nonvanishing condition $\prod_i\det h_i\ne0$. Therefore $\operatorname{Aut}_Q(X)=E^\times$ is a nonempty [Zariski-open subset](../../../algebraic-geometry.md#zariski-open-set) of the vector space $E$.

Take a [Krull-Schmidt decomposition](../../../module-theory.md#krull-schmidt-decomposition) $X\cong\bigoplus_{a=1}^rM_a^{\oplus m_a}$, with pairwise nonisomorphic [indecomposable modules](../../../module-theory.md#indecomposable-module). The [Fitting lemma](../../../module-theory.md#fitting-lemma) makes each $\operatorname{End}_Q(M_a)$ a [local endomorphism ring](../../../module-theory.md#local-endomorphism-ring). Its residue [division algebra](../../../algebra.md#division-algebra) is $k$: over an [algebraically closed field](../../../algebra.md#algebraically-closed-field), every element of a finite-dimensional division algebra has an eigenvalue and hence must be scalar. The [semisimple quotient of a module endomorphism algebra](../../../module-theory.md#semisimple-quotient-of-a-module-endomorphism-algebra) consequently gives, for the [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical) $J=J(E)$,

$$
E/J\cong\prod_{a=1}^rM_{m_a}(k),\qquad E^\times\longrightarrow\prod_{a=1}^r\operatorname{GL}_{m_a}(k)
$$

is surjective with kernel $1+J$. The nilpotence of $J$ makes $(1+j)^{-1}=1-j+j^2-\cdots$ finite and each $1+j$ unipotent. The kernel is closed and normal. Acting on the multiplicity spaces embeds the product of [general linear groups](../../../group-theory.md#general-linear-group) back into $E^\times$ and splits this quotient. This proves the [Levi decomposition of a quiver automorphism group](../../../algebra.md#levi-decomposition-of-a-quiver-automorphism-group)

$$
\boxed{\operatorname{Aut}_Q(X)\cong(1+J)\rtimes\prod_{a=1}^r\operatorname{GL}_{m_a}(k)}.
$$

Since $1+J$ is the [unipotent radical](../../../lie-theory.md#unipotent-radical), a nonzero $X$ is indecomposable exactly when **$\operatorname{Aut}_Q(X)/R_u(\operatorname{Aut}_Q(X))\cong\mathbb G_m$**: the product has a single factor of size one.

For the [base change action on quiver representations](../../../algebra.md#base-change-action-on-quiver-representations), the orbit map is $g\mapsto(g_jx_\rho g_i^{-1})_{\rho:i\to j}$. Substituting $g_i=I+\epsilon u_i$, with $\epsilon^2=0$, shows its differential is

$$
\boxed{\xi_x(u)_\rho=u_jx_\rho-x_\rho u_i}.
$$

Its kernel is $\operatorname{End}_Q(X)$. The stabilizer is smooth because it is open in that vector space. Hence the differential has rank $\dim\operatorname{GL}(\mathbf n)-\dim\operatorname{Aut}_Q(X)=\dim\mathcal O_X$, and its image is the [Zariski tangent space](../../../algebraic-geometry.md#zariski-tangent-space) $T_x\mathcal O_X$. The [normal space to a quiver orbit](../../../algebra.md#normal-space-to-a-quiver-orbit) is therefore

$$
\boxed{T_x\operatorname{Rep}_Q(\mathbf n)/T_x\mathcal O_X\cong\operatorname{Ext}^1_Q(X,X)}.
$$

The ambient [quiver representation space](../../../algebra.md#quiver-representation-space) is an irreducible affine space, and orbits are locally closed. An orbit is open exactly when its dimension equals that ambient dimension, equivalently when $\operatorname{Ext}^1_Q(X,X)=0$. This proves that [rigid quiver representations have open orbits](../../../algebra.md#rigid-quiver-representations-have-open-orbits). Such an orbit is dense and unique, since two nonempty open subsets of an irreducible space intersect.

## 5

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

For a finitely generated [associative algebra](../../../associative-algebra.md) $A$, the [representation variety of an associative algebra](../../../associative-algebra.md#representation-variety-of-an-associative-algebra) consists of generator matrices satisfying all defining polynomial relations. With fixed orthogonal idempotents $1=\sum_{i=1}^me_i$, require a representation on $\bigoplus_i k^{n_i}$ to send $e_i$ to the standard vertex projector. This is the meaning of $\operatorname{Rep}_A(\mathbf n)$; without specified idempotents, use the usual single dimension $r$ and $\operatorname{Rep}_A(r)=\operatorname{Hom}_{k\text{-alg}}(A,M_r(k))$. Polynomial relations cut out a closed [affine variety](../../../algebraic-geometry.md#affine-algebraic-set) in the space of generator matrices.

The group $G=\prod_i\operatorname{GL}_{n_i}(k)$ acts by conjugation, preserving the prescribed projectors. Its stabilizer is $\operatorname{Aut}_A(X)$, a nonempty open subset of $\operatorname{End}_A(X)$. The [orbit dimension formula](../../../group-theory.md#orbit-dimension-formula) consequently gives

$$
\boxed{\dim G-\dim\mathcal O_X=\dim\operatorname{Stab}_G(x)=\dim\operatorname{Aut}_A(X)=\dim\operatorname{End}_A(X)}.
$$

A [degeneration of a module](../../../module-theory.md#degeneration-of-a-module) $X$ to $Y$ means that $\mathcal O_Y\subseteq\overline{\mathcal O_X}$, equivalently that one representative of $Y$ lies in this closure.

For $0\to X'\to X\to X''\to0$, choose a vector-space splitting, so every generator has block matrix $x_g=\left(\begin{smallmatrix}x'_g&b_g\\0&x''_g\end{smallmatrix}\right)$. Conjugation by $\operatorname{diag}(tI,I)$, $t\ne0$, gives

$$
x_g(t)=\begin{pmatrix}x'_g&t b_g\\0&x''_g\end{pmatrix}.
$$

This polynomial family extends to $t=0$, retains all algebra relations, and at zero represents $X'\oplus X''$. Thus [splitting an extension gives a module degeneration](../../../representation-theory.md#split-extension-as-a-degeneration). Iterating along a [composition series](../../../finite-group-theory.md#composition-series) gives **$X\rightsquigarrow\operatorname{gr}X=\bigoplus_jX_j/X_{j-1}$**. Degenerations are transitive because an orbit closure is closed and invariant under base change.

For the [one-arrow quiver](../../../algebra.md#kronecker-quiver-with-one-arrow) with dimension vector $(n_1,n_2)$,

$$
\boxed{\operatorname{Rep}_Q(n_1,n_2)=\operatorname{Hom}_k(k^{n_1},k^{n_2})\cong M_{n_2\times n_1}(k)}.
$$

The action is $A\mapsto g_2Ag_1^{-1}$. Its [rank orbits of a matrix under left-right multiplication](../../../vector-space.md#rank-orbit-of-a-matrix-under-left-right-multiplication) are indexed by $r=0,\ldots,\min(n_1,n_2)$, with a representative containing an $r\times r$ identity block and zeros elsewhere. Their dimensions are $r(n_1+n_2-r)$; their closures contain exactly matrices of rank at most $r$.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Write the two arrow matrices as $(A,B)\in M_2(k)^2$. The [base change action on quiver representations](../../../algebra.md#base-change-action-on-quiver-representations) sends them to $(g_2Ag_1^{-1},g_3Bg_2^{-1})$. Starting from $(I,I)$ yields precisely the pairs with both matrices invertible: given such a pair, choose $g_1=I$, $g_2=A$, $g_3=BA$. Hence

$$
\boxed{\mathcal O_X=\{(A,B):\det A\det B\ne0\}\cong\operatorname{GL}_2(k)^2}.
$$

This is a nonempty [Zariski-open subset](../../../algebraic-geometry.md#zariski-open-set) of the irreducible affine space $M_2(k)^2$, so its closure is the entire representation space. Its boundary in that closure is $\{\det A\det B=0\}$.

The [rank classification of a two-step linear map](../../../algebra.md#rank-classification-of-a-two-step-linear-map) says an orbit is determined by $(r,s,t)=(\operatorname{rank}A,\operatorname{rank}B,\operatorname{rank}(BA))$. Indeed, the six interval multiplicities from the elementary decomposition are

$$
m_{13}=t,\quad m_{12}=r-t,\quad m_{23}=s-t,\quad m_{11}=2-r,\quad m_{22}=2-r-s+t,\quad m_{33}=2-s.
$$

They are nonnegative exactly when $0\le r,s\le2$ and $\max(0,r+s-2)\le t\le\min(r,s)$. Apart from the open orbit $(2,2,2)$, **there are nine boundary orbits**. Put $D=\operatorname{diag}(1,0)$ and $E=\operatorname{diag}(0,1)$; representatives are

$$
\begin{array}{c|c|c}
(r,s,t)&A&B\\\hline
(0,0,0)&0&0\\
(0,1,0)&0&D\\
(0,2,0)&0&I\\
(1,0,0)&D&0\\
(2,0,0)&I&0\\
(1,1,0)&D&E\\
(1,1,1)&D&D\\
(1,2,1)&D&I\\
(2,1,1)&I&D
\end{array}
$$

The two rank-one/rank-one cases differ by whether $\operatorname{im}A\subseteq\ker B$; the individual arrow ranks alone do not distinguish them.

## 6

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

A nonzero finite-dimensional representation is a [brick module](../../../module-theory.md#brick-module) when its [endomorphism ring](../../../module-theory.md#endomorphism-ring) is a division algebra. Over the algebraically closed field $k$, this means $\operatorname{End}_Q(X)=k$: for any endomorphism $f$, an eigenvalue $\lambda$ makes $f-\lambda I$ noninvertible, hence zero in a division algebra.

For a counterexample to the converse of “brick implies indecomposable”, take the one-loop representation $k^2$ with nilpotent Jordan block $N=\left(\begin{smallmatrix}0&1\\0&0\end{smallmatrix}\right)$. Its [endomorphism ring](../../../module-theory.md#endomorphism-ring) is $k[N]\cong k[t]/(t^2)$, a [local endomorphism ring](../../../module-theory.md#local-endomorphism-ring) of dimension two. It has no nontrivial [idempotents](../../../commutative-algebra.md#idempotent), so the module is indecomposable, but it is not a brick.

For the [one-arrow quiver](../../../algebra.md#kronecker-quiver-with-one-arrow), splitting the kernel, image and target complement decomposes any representation into copies of $k\to0$, $0\to k$ and $k\xrightarrow{1}k$. Each has endomorphism ring $k$. Therefore **every indecomposable of the one-arrow quiver is a brick**.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

For the [Kronecker quiver](../../../algebra.md#kronecker-quiver) representation with arrows $I$ and $N=\left(\begin{smallmatrix}0&1\\0&0\end{smallmatrix}\right)$, an endomorphism $(P,Q)$ satisfies $Q=P$ and $PN=NP$. Solving the second equation gives

$$
\operatorname{End}_Q(X)=\left\{\begin{pmatrix}a&b\\0&a\end{pmatrix}:a,b\in k\right\}\cong k[t]/(t^2).
$$

Thus **this representation is indecomposable but is not a brick**: its endomorphism ring is a [local endomorphism ring](../../../module-theory.md#local-endomorphism-ring), while the nonzero endomorphism $N$ is nilpotent.

For a general indecomposable non-brick, the [proof of Ringel lemma on bricks](../../../module-theory.md#proof-of-ringel-lemma-on-bricks) finds a proper indecomposable submodule with nonzero self-extensions. Repetition in strictly decreasing dimension reaches a [brick module](../../../module-theory.md#brick-module) $Y\subset X$ with $\operatorname{Ext}^1_Q(Y,Y)\ne0$. The linked proof supplies the minimal-rank, retraction and hereditary-extension steps.

Now assume the [Tits form of a quiver](../../../algebra.md#tits-form-of-a-quiver) is positive definite. If an indecomposable $X$ were not a brick, this $Y$ would give the contradiction

$$
0<q(\dim Y)=1-\dim\operatorname{Ext}^1_Q(Y,Y)\le0.
$$

Hence $X$ is a brick. For its nonzero dimension vector $\mathbf n$, positivity and integrality then imply

$$
0<q(\mathbf n)=1-\dim\operatorname{Ext}^1_Q(X,X)\le1,\qquad \boxed{q(\mathbf n)=1,\quad\operatorname{Ext}^1_Q(X,X)=0}.
$$

Thus every indecomposable in this case is a rigid brick. This deduction uses the [Ringel lemma on bricks](../../../module-theory.md#ringel-lemma-on-bricks) and the [Ringel form](../../../algebra.md#ringel-form), without requiring the full [Gabriel theorem](../../../algebra.md#gabriel-s-theorem).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
