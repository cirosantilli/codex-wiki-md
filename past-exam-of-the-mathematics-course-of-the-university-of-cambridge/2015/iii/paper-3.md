# Paper 3

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_3.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_3.pdf)

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
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
    - [i](#6/a/i)
      - [Solution](#6/a/i/solution)
    - [ii](#6/a/ii)
      - [Solution](#6/a/ii/solution)
    - [iii](#6/a/iii)
      - [Solution](#6/a/iii/solution)
    - [iv](#6/a/iv)
      - [Solution](#6/a/iv/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)

## 1

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [representation of a quiver](../../../algebra.md#representation-of-a-quiver) assigns a $k$-vector space $X_i$ to each vertex $i\in Q_0$ and a [linear map](../../../vector-space.md#linear-map) $f_\rho:X_{s(\rho)}\to X_{t(\rho)}$ to each arrow $\rho\in Q_1$. Here $s(\rho)$ and $t(\rho)$ are its source and target. A [quiver representation morphism](../../../algebra.md#quiver-representation-morphism) $\theta:X\to Y$ is a family of [linear maps](../../../vector-space.md#linear-map) $\theta_i:X_i\to Y_i$ such that every arrow square commutes:

$$
\boxed{\theta_{t(\rho)}f_\rho=g_\rho\theta_{s(\rho)}\quad(\rho\in Q_1).}
$$

Composition and identities are defined vertex by vertex. A [quiver representation morphism](../../../algebra.md#quiver-representation-morphism) is an isomorphism precisely when every $\theta_i$ is invertible.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Use the following [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical) facts for a unital algebra: a [nilpotent ideal](../../../commutative-algebra.md#nilpotent-ideal) is contained in the [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical); under a surjective algebra homomorphism the image of the [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical) is contained in the radical of the quotient; and a finite product of fields has zero [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical). For completeness, if $I^N=0$ and $x\in I$, then $ax\in I$ for every $a\in A$, and $1-ax$ is invertible with inverse $\sum_{j=0}^{N-1}(ax)^j$. The usual unit criterion for the [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical) therefore gives $I\subseteq J(A)$. The quotient assumption gives $J(A)\subseteq I$. Hence

$$
\boxed{I=J(A).}
$$

This is the [nilpotent ideal with semisimple quotient radical criterion](../../../noncommutative-algebra.md#nilpotent-ideal-with-semisimple-quotient-radical-criterion).

For the finite [quiver](../../../algebra.md#quiver) under consideration, let $R$ be the [arrow ideal of a path algebra](../../../algebra.md#arrow-ideal-of-a-path-algebra), spanned by paths of positive length. If $Q$ has $r$ vertices and no oriented cycle, a path cannot repeat a vertex, so $R^r=0$. Meanwhile $kQ/R\cong\prod_{i\in Q_0}k$, with the constant paths giving the coordinate idempotents. The criterion just proved yields **$J(kQ)=R$**.

The condition on cycles is necessary. A [quiver with one loop](../../../algebra.md#quiver-with-one-loop) has [path algebra](../../../algebra.md#path-algebra) $k[t]$, whose arrow ideal is $(t)$. But **$J(k[t])=0\ne(t)$**: the maximal ideals $(t-a)$, $a\in k$, have intersection zero, since the algebraically closed field $k$ is infinite and a nonzero polynomial has only finitely many roots. Thus the arrow ideal need not be the [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical) when oriented cycles are present.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Rows in the following matrix index the source, columns the target, in the order $X,Y,Z$. Solving the arrow-square equation for a [quiver representation morphism](../../../algebra.md#quiver-representation-morphism) gives

$$
\boxed{\bigl(\dim_k\operatorname{Hom}_Q(U,V)\bigr)_{U,V=X,Y,Z}=\begin{pmatrix}1&0&1\\0&1&0\\0&1&1\end{pmatrix}.}
$$

In particular, the nonzero morphisms between distinct representations are **$X\to Z$ and $Z\to Y$**, each a one-dimensional family of scalar multiples of the vertexwise inclusion or projection. A map $Y\to Z$ is forced to vanish at the source by the identity arrow of $Z$; similarly a map $Z\to X$ is forced to vanish at the target. Maps between $X$ and $Y$ are zero. Each [endomorphism ring](../../../module-theory.md#endomorphism-ring) is $k$.

The [extension complex of quiver representations](../../../algebra.md#extension-complex-of-quiver-representations) for the [one-arrow quiver](../../../algebra.md#kronecker-quiver-with-one-arrow) is

$$
\operatorname{Hom}(U_1,V_1)\oplus\operatorname{Hom}(U_2,V_2)\longrightarrow\operatorname{Hom}(U_1,V_2),\qquad(h_1,h_2)\longmapsto f_Vh_1-h_2f_U.
$$

Its [cokernel](../../../linear-algebra.md#cokernel) is $\operatorname{Ext}^1_Q(U,V)$. Substitution of the three representations gives

$$
\boxed{\bigl(\dim_k\operatorname{Ext}^1_Q(U,V)\bigr)_{U,V=X,Y,Z}=\begin{pmatrix}0&0&0\\1&0&0\\0&0&0\end{pmatrix}.}
$$

Here the first argument is the quotient endpoint of a [short exact sequence](../../../module-theory.md#short-exact-sequence). Thus the only possible nonsplit endpoint pair is **subobject $X$, quotient $Y$**. The sequence

$$
0\longrightarrow X\longrightarrow Z\longrightarrow Y\longrightarrow0
$$

is nonsplit, since $Z$ is indecomposable. More explicitly, all extensions with these endpoints have a middle arrow $k\xrightarrow{\lambda}k$: $\lambda=0$ gives the [split short exact sequence](../../../module-theory.md#split-short-exact-sequence), while each $\lambda\ne0$ gives a middle representation isomorphic to $Z$. With endpoint identifications fixed the extension classes form $k$; up to endpoint automorphisms all nonzero classes give this same nonsplit sequence. There are **no other nonsplit sequences with the listed endpoints**, including equal endpoints.

## 2

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [path algebra](../../../algebra.md#path-algebra) $kQ$ is the $k$-vector space with basis all directed paths, including the length-zero path $e_i$ at each vertex. Extend path composition bilinearly, declaring the product zero when the paths cannot be composed. We use the left-module convention: $pq$ means first traverse $q$, then $p$; for an arrow $\rho:i\to j$, $e_j\rho e_i=\rho$.

The constant paths are mutually orthogonal [idempotents](../../../commutative-algebra.md#idempotent). For any path $p:i\to j$,

$$
e_jp=p=pe_i,\qquad e_\ell p=0\ (\ell\ne j),\qquad pe_\ell=0\ (\ell\ne i).
$$

Consequently, for the finite vertex set used here,

$$
\boxed{1_{kQ}=\sum_{i\in Q_0}e_i.}
$$

It acts as an identity on every basis path, hence on the entire [path algebra](../../../algebra.md#path-algebra). Finiteness of the vertex set is what makes this a genuine element of the algebra; an infinite-vertex path algebra instead has finite vertex sums as local units.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

There is one constant path and $r$ loop generators; every other path is a word in those loops. Distinct words are distinct basis paths, so there are no relations among the generators. Therefore

$$
\boxed{kL_r\cong k\langle x_1,\ldots,x_r\rangle,}
$$

the [free associative algebra](../../../associative-algebra.md#free-associative-algebra) on $r$ generators, with each loop sent to its corresponding generator. For $r=1$ this is $k[x_1]$; for $r\geq2$ it is noncommutative. The [quiver with one loop](../../../algebra.md#quiver-with-one-loop) is the $r=1$ case of the [quiver with r loops](../../../algebra.md#quiver-with-r-loops).

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Number the source vertices $1,\ldots,r$ and the sink $c=r+1$, and write $a_i:i\to c$ for the arrows. The only basis paths are $e_1,\ldots,e_r,e_c,a_1,\ldots,a_r$. Using standard [matrix units](../../../vector-space.md#matrix-unit), define

$$
e_i\longmapsto E_{ii},\qquad e_c\longmapsto E_{cc},\qquad a_i\longmapsto E_{ci}.
$$

The relations $e_ca_i=a_i=a_ie_i$, orthogonality of the vertex [idempotents](../../../commutative-algebra.md#idempotent), and $a_ia_j=0$ agree exactly with multiplication of these [matrix units](../../../vector-space.md#matrix-unit). The map is therefore an algebra homomorphism, and its images form a basis of the algebra

$$
\boxed{kS_r\cong\left\{\begin{pmatrix}\operatorname{diag}(\lambda_1,\ldots,\lambda_r)&0\\v&\mu\end{pmatrix}:\lambda_i,\mu\in k,\ v\in k^{1\times r}\right\}.}
$$

This is an explicit isomorphism of the [path algebra](../../../algebra.md#path-algebra) of the [subspace quiver](../../../algebra.md#subspace-quiver) with a $(2r+1)$-dimensional triangular matrix algebra.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

First split off the kernel of each source-to-sink arrow. Each kernel contributes copies of the simple representation supported at that source. The remaining arrows are injective, so identify the three source spaces with subspaces $U_1,U_2,U_3$ of the sink space $V$. We now give an elementary [three-subspace decomposition](../../../algebra.md#three-subspace-decomposition).

Split off the common intersection $U_1\cap U_2\cap U_3$: any projection onto it preserves all three subspaces. Next split off each pairwise intersection. For example, once the triple intersection has gone, $W=U_1\cap U_2$ is disjoint from $U_3$; a projection onto $W$ that kills $U_3$ preserves $U_1,U_2,U_3$. This extracts blocks whose membership is exactly $\{1,2\}$. Repeating for the other pairs leaves pairwise disjoint subspaces.

For each $i$, choose a complement $W_i$ to $U_i\cap(U_j+U_\ell)$ in $U_i$. A projection onto $W_i$ killing $U_j+U_\ell$ preserves the triple, so these complements split off as blocks of membership exactly $\{i\}$. In the remaining triple, every $U_i$ lies in the sum of the other two and all pairwise intersections are zero. Thus the sum is $U_1\oplus U_2$, and both projections of $U_3$ onto $U_1,U_2$ are isomorphisms. Hence $U_3$ is the graph of an isomorphism $T:U_1\to U_2$. Choose a basis $u_a$ of $U_1$ and the basis $Tu_a$ of $U_2$; this graph decomposes into two-dimensional blocks with three distinct lines. A complement to $U_1+U_2+U_3$ in $V$ contributes sink-only simple blocks.

The complete list of indecomposable blocks is therefore:

- **Three source simples**, with zero sink space.
- **Eight blocks with one-dimensional sink**, one for each subset $S\subseteq\{1,2,3\}$: the source space is $k$ for $i\in S$ and zero otherwise, and every nonzero arrow is the identity.
- **One exceptional block**, with all three source spaces $k$, sink $k^2$, and arrows $1\mapsto e_1$, $1\mapsto e_2$, $1\mapsto e_1+e_2$.

Each of the first eleven blocks has [endomorphism ring](../../../module-theory.md#endomorphism-ring) $k$. For the [exceptional indecomposable of the three-subspace quiver](../../../algebra.md#exceptional-indecomposable-of-the-three-subspace-quiver), an endomorphism of $k^2$ preserving the first two lines is diagonal; preserving the third makes its two diagonal entries equal. Its [endomorphism ring](../../../module-theory.md#endomorphism-ring) is also $k$, so all twelve are indecomposable. Their [dimension vectors of quiver representations](../../../algebra.md#dimension-vector-of-a-quiver-representation) distinguish them. The decomposition argument proves completeness, and hence **there are exactly $12$ isomorphism classes**. No general classification theorem is needed.

<a id="2/c/image-exceptional-three-subspace-representation-with-a-two-dimensional-sink-and-three-distinct-image-lines"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-3-three-subspace-exception.png)

**[Figure 1](#2/c/image-exceptional-three-subspace-representation-with-a-two-dimensional-sink-and-three-distinct-image-lines). Exceptional three-subspace representation with a two-dimensional sink and three distinct image lines**.

## 3

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Set $A=kQ$, $X_i=e_iX$, and let $f_\rho$ be the action of the arrow $\rho$ on $X_{s(\rho)}$. Write $P_i=Ae_i$, a left [projective module](../../../module-theory.md#projective-module). The [standard projective resolution of a quiver representation](../../../algebra.md#standard-projective-resolution-of-a-quiver-representation) is

$$
\boxed{0\longrightarrow\bigoplus_{\rho\in Q_1}P_{t(\rho)}\otimes_kX_{s(\rho)}\xrightarrow{d}\bigoplus_{i\in Q_0}P_i\otimes_kX_i\xrightarrow{\varepsilon}X\longrightarrow0.}
$$

The algebra acts on the first tensor factor. The augmentation is $\varepsilon(p\otimes x)=px$. On the summand for $\rho:i\to j$, the differential sends $p\otimes x$ to $p\rho\otimes x$ in the $i$-summand minus $p\otimes f_\rho(x)$ in the $j$-summand. Here $p\in Ae_j$, so $p\rho\in Ae_i$. These formulas specify every term and map, and $\varepsilon d=0$.

Exactness is the standard path resolution fact: the relations identify a path acting on a vector with successively applying its arrows; uniqueness of the first traversed arrow supplies injectivity of the relation map. Each $Ae_i$ is a direct summand of $A$ because $e_i$ is an [idempotent](../../../commutative-algebra.md#idempotent), and tensoring with a $k$-vector space gives a direct sum of copies of $Ae_i$. Both terms preceding $X$ are consequently [projective modules](../../../module-theory.md#projective-module). Thus the displayed sequence is a [projective resolution](../../../algebra.md#projective-resolution) of length at most one.

The same path resolution works for arbitrary left modules, with possibly infinite-dimensional $X_i$ and arbitrary direct sums of [projective modules](../../../module-theory.md#projective-module). Hence every left $A$-module has projective dimension at most one. Equivalently, **$A$ is a left hereditary ring**: if $N\subseteq P$ with $P$ projective, dimension shifting gives $\operatorname{Ext}^1_A(N,M)\cong\operatorname{Ext}^2_A(P/N,M)=0$ for every $M$, so $N$ is projective. This argument also covers [quivers](../../../algebra.md#quiver) with oriented cycles.

For dimension vectors $\mathbf n,\mathbf m\in\mathbb R^{Q_0}$, define the [Ringel form](../../../algebra.md#ringel-form)

$$
\boxed{\langle\mathbf n,\mathbf m\rangle_Q=\sum_{i\in Q_0}n_im_i-\sum_{\rho\in Q_1}n_{s(\rho)}m_{t(\rho)}.}
$$

Apply $\operatorname{Hom}_A(-,Y)$ to the [projective resolution](../../../algebra.md#projective-resolution). Evaluation at $e_i$ identifies $\operatorname{Hom}_A(P_i\otimes_kV,Y)$ with $\operatorname{Hom}_k(V,Y_i)$. Consequently there is an exact sequence

$$
0\longrightarrow\operatorname{Hom}_Q(X,Y)\longrightarrow C^0\xrightarrow{\delta}C^1\longrightarrow\operatorname{Ext}^1_Q(X,Y)\longrightarrow0,
$$

where

$$
C^0=\bigoplus_i\operatorname{Hom}_k(X_i,Y_i),\quad C^1=\bigoplus_\rho\operatorname{Hom}_k(X_{s(\rho)},Y_{t(\rho)}),\quad(\delta h)_\rho=g_\rho h_{s(\rho)}-h_{t(\rho)}f_\rho.
$$

This is the [extension complex of quiver representations](../../../algebra.md#extension-complex-of-quiver-representations). Taking its alternating dimension sum yields

$$
\boxed{\dim\operatorname{Hom}_Q(X,Y)-\dim\operatorname{Ext}^1_Q(X,Y)=\langle\dim X,\dim Y\rangle_Q.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $K=\ker f_\rho$ and $C=Y_j/\operatorname{im}g_\rho$. Consider the map from the arrow term of the [extension complex of quiver representations](../../../algebra.md#extension-complex-of-quiver-representations) to $\operatorname{Hom}_k(K,C)$ that restricts its $\rho$-component to $K$ and then takes the quotient in $Y_j$. This map is surjective: a map $K\to C$ can be lifted to $Y_j$ and extended from $K$ to $X_i$.

Every coboundary is killed by this map, since for $x\in K$,

$$
(\delta h)_\rho(x)=g_\rho h_i(x)-h_jf_\rho(x)=g_\rho h_i(x)\in\operatorname{im}g_\rho.
$$

It therefore induces a surjection

$$
\operatorname{Ext}^1_Q(X,Y)\twoheadrightarrow\operatorname{Hom}_k(\ker f_\rho,\operatorname{coker}g_\rho).
$$

Both vector spaces in the final [Hom functor](../../../algebra.md#hom-functor) are nonzero, so its dimension is positive. Hence **$\operatorname{Ext}^1_Q(X,Y)\ne0$**. This is the [kernel-cokernel obstruction to splitting a quiver extension](../../../algebra.md#kernel-cokernel-obstruction-to-splitting-a-quiver-extension) and remains valid for loops and repeated arrows elsewhere in the [quiver](../../../algebra.md#quiver).

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

If an arrow map failed to have maximal [matrix rank](../../../vector-space.md#matrix-rank), it would have both a nonzero [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map) and a nonzero [cokernel](../../../linear-algebra.md#cokernel). Apply the preceding obstruction with $Y=X$. It would give $\operatorname{Ext}^1_Q(X,X)\ne0$, contrary to the assumption. Therefore **every arrow map is injective or surjective**, equivalently its rank is the minimum of the two vertex dimensions. This is a necessary property of a [rigid quiver representation](../../../algebra.md#rigid-quiver-representation).

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

We first record why [rigid quiver representations have open orbits](../../../algebra.md#rigid-quiver-representations-have-open-orbits). Let $\mathbf n=\dim X$, $G=\prod_i\operatorname{GL}(X_i)$ and $R=\operatorname{Rep}_Q(\mathbf n)$. The stabilizer is $\operatorname{Aut}_Q(X)$, the nonempty open set of units in $\operatorname{End}_Q(X)$, so it has dimension $\dim\operatorname{End}_Q(X)$. The [dimension formula for an algebraic group homomorphism](../../../algebraic-geometry.md#dimension-formula-for-an-algebraic-group-homomorphism), or the same constant-fiber argument for the orbit map, gives

$$
\dim\mathcal O_X=\sum_i n_i^2-\dim\operatorname{End}_Q(X).
$$

By the [Ringel form](../../../algebra.md#ringel-form) identity and $\operatorname{Ext}^1_Q(X,X)=0$, this equals $\sum_\sigma n_{s(\sigma)}n_{t(\sigma)}=\dim R$. An algebraic-group orbit is locally closed; since $R$ is an irreducible [affine space](../../../geometry-and-topology.md#affine-space), this full-dimensional orbit is open and dense.

Write $q=\rho\pi$ for the composed path. Each matrix entry of $q$ is a polynomial function on $R$. Since $qX=0$, change of basis makes it zero on all of $\mathcal O_X$, hence on all of $R$ by density. Suppose instead that $X_{t(\rho)}\ne0$. The condition $\pi X\ne0$ ensures that every vertex space visited by $\pi$ is nonzero. Choose a vector $v_a\ne0$ and a functional $\ell_a$ with $\ell_a(v_a)=1$ at every vertex visited by $q$. Assign to every arrow $\sigma$ occurring in $q$ the map $v_{t(\sigma)}\ell_{s(\sigma)}$, and assign arbitrary maps, say zero, to the other arrows. At this representation, the path $q$ carries its initial chosen vector to its final chosen vector, so $q$ is nonzero, a contradiction.

The construction uses a single assigned map per arrow, so it still works if an arrow or vertex occurs repeatedly in the path. Therefore

$$
\boxed{X_{t(\rho)}=0.}
$$

This proves the [path identities in a rigid quiver representation](../../../algebra.md#path-identities-in-a-rigid-quiver-representation) claim for an arbitrary [quiver](../../../algebra.md#quiver). Maximal rank of the individual arrows alone would not justify the conclusion about their composition.

## 4

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [dimension of a topological space by irreducible chains](../../../algebraic-geometry.md#dimension-of-a-topological-space-by-irreducible-chains) is the supremum of the integers $d$ for which there is a chain $Z_0\subsetneq Z_1\subsetneq\cdots\subsetneq Z_d$ of nonempty irreducible closed subsets of the space. Closedness here is relative to the given locally closed space. For varieties this is their [Krull dimension](../../../commutative-algebra.md#krull-dimension).

An [algebraic group](../../../algebraic-geometry.md#algebraic-group) is a group whose underlying space is an [algebraic variety](../../../algebraic-geometry.md#algebraic-variety) and whose multiplication $G\times G\to G$ and inversion $G\to G$ are morphisms. An [algebraic group action](../../../algebraic-geometry.md#algebraic-group-action) on a variety $V$ is a morphism $G\times V\to V$ satisfying the identity and associativity axioms of a [group action](../../../group-theory.md#group-action).

For the homomorphism $\varphi$, the kernel is $\varphi^{-1}(1_H)$, so **the kernel is closed**. To prove closedness of the image, use the [Chevalley constructibility theorem](../../../algebraic-geometry.md#chevalley-constructibility-theorem): the image of a morphism of varieties is constructible. Thus $S=\varphi(G)$ is a [constructible subset of a variety](../../../algebraic-geometry.md#constructible-subset-of-a-variety) and an abstract subgroup. Its closure $C$ is also a subgroup: translation by elements of $S$ preserves $C$, and continuity then extends multiplication and inversion to $C$.

A dense constructible subset contains a dense open subset $U$ of its closure. For $c\in C$, both $U$ and $cU$ are dense open subsets of $C$, so their intersection is nonempty. If $u=cv$ with $u,v\in U\subseteq S$, then $c=uv^{-1}\in S$. Hence $S=C$, proving that **the image is closed**. This is the principle that a [constructible subgroup is closed](../../../algebraic-geometry.md#constructible-subgroup-is-closed).

Every nonempty fiber of $G\to S$ is a translate of $\ker\varphi$ and has that same dimension. The [fiber dimension theorem](../../../algebraic-geometry.md#fiber-dimension-theorem) therefore gives

$$
\boxed{\dim G=\dim\ker\varphi+\dim\operatorname{im}\varphi.}
$$

This [dimension formula for an algebraic group homomorphism](../../../algebraic-geometry.md#dimension-formula-for-an-algebraic-group-homomorphism) is a dimension statement, so it does not require separability of $\varphi$.

For a [dimension vector of a quiver representation](../../../algebra.md#dimension-vector-of-a-quiver-representation) $\mathbf n$, set

$$
\operatorname{Rep}_Q(\mathbf n)=\prod_{\rho:i\to j}\operatorname{Hom}_k(k^{n_i},k^{n_j}),\qquad\operatorname{GL}(\mathbf n)=\prod_i\operatorname{GL}_{n_i}(k).
$$

The [base change action on quiver representations](../../../algebra.md#base-change-action-on-quiver-representations) is

$$
\boxed{(g\cdot f)_\rho=g_{t(\rho)}f_\rho g_{s(\rho)}^{-1}.}
$$

The entries are regular functions on the product of the [general linear groups](../../../group-theory.md#general-linear-group) and the [quiver representation space](../../../algebra.md#quiver-representation-space), because inverse entries are cofactors divided by the invertible determinant. Thus this is an [algebraic group action](../../../algebraic-geometry.md#algebraic-group-action).

For nonzero $\mathbf n$, let $\Delta k^\times$ be the common scalar subgroup $(\lambda I_{n_i})_i$ and define $\operatorname{PGL}(\mathbf n)=\operatorname{GL}(\mathbf n)/\Delta k^\times$. Common scalars act trivially, so the formula descends to an [algebraic group action](../../../algebraic-geometry.md#algebraic-group-action) of this [projective base change group of a quiver](../../../algebra.md#projective-base-change-group-of-a-quiver). This is a quotient by one common scalar, not a product of the individual projective groups. If every $n_i=0$, the representation space is a point and both actions are taken to be trivial.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

An [algebraic group](../../../algebraic-geometry.md#algebraic-group) is [connected](../../../geometry-and-topology.md#connected-space) when its underlying [Zariski topology](../../../algebraic-geometry.md#zariski-topology) is a [connected space](../../../geometry-and-topology.md#connected-space). An [unipotent algebraic group](../../../lie-theory.md#unipotent-algebraic-group) is a [linear algebraic group](../../../lie-theory.md#linear-algebraic-group) whose elements, in a faithful matrix realization, satisfy that $u-I$ is nilpotent. A [reductive algebraic group](../../../lie-theory.md#reductive-group), in the connected convention, is a [connected](../../../geometry-and-topology.md#connected-space) [linear algebraic group](../../../lie-theory.md#linear-algebraic-group) whose [unipotent radical](../../../lie-theory.md#unipotent-radical) is trivial: it has no nontrivial connected normal unipotent algebraic subgroup.

Let $E=\operatorname{End}_Q(X)$. It is a finite-dimensional associative algebra, and $\operatorname{Aut}_Q(X)=E^\times$. The latter is the nonempty open subset where the determinant on $\bigoplus_iX_i$ is nonzero. Since the affine space $E$ is irreducible, this open subset is irreducible and hence connected. It is a [linear algebraic group](../../../lie-theory.md#linear-algebraic-group): within $\operatorname{GL}(\bigoplus_iX_i)$ it is cut out by the linear equations of preserving the vertex summands and commuting with the arrow maps. Thus **the automorphism group is connected**.

By the [Krull–Schmidt theorem](../../../module-theory.md#krull-schmidt-theorem), write $X\cong\bigoplus_{a=1}^sM_a^{\oplus m_a}$, with pairwise nonisomorphic indecomposables $M_a$. The [Fitting lemma](../../../module-theory.md#fitting-lemma) makes each $\operatorname{End}_Q(M_a)$ a local algebra. Its residue division algebra is $k$: every element of a finite-dimensional division algebra over the algebraically closed field has an eigenvalue for left multiplication, and subtracting that scalar gives a noninvertible element, hence zero.

The standard radical description of the endomorphism algebra of a [Krull-Schmidt decomposition](../../../module-theory.md#krull-schmidt-decomposition) therefore gives

$$
E/J(E)\cong\prod_{a=1}^s\operatorname{Mat}_{m_a}(k).
$$

Concretely, maps between nonisomorphic summands lie in the radical, while on each isotypic block one reduces all entries modulo the local radical. The off-diagonal rule follows because a composition $M_a\to M_b\to M_a$ cannot be a unit for $a\ne b$: it would split $M_a$ off the indecomposable $M_b$, forcing an isomorphism. The finite-dimensional radical description then identifies the kernel of this block reduction with $J(E)$. Put $U=1+J(E)$. The [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical) of the finite-dimensional algebra is nilpotent, so every $1+j$ is a unit and is unipotent on $\bigoplus_iX_i$. Also $U$ is closed, being the translate of the linear subspace $J(E)$, and normal, being the kernel of

$$
E^\times\longrightarrow\prod_a\operatorname{GL}_{m_a}(k).
$$

This map has an explicit algebraic section: after fixing the direct-sum decomposition, a matrix $B_a$ acts on the $m_a$ copies by $B_a\otimes1_{M_a}$. These block actions give a subgroup $L\cong\prod_a\operatorname{GL}_{m_a}(k)$ with trivial intersection with $U$. Every unit is uniquely a product of an element of $U$ and one of $L$. Hence

$$
\boxed{\operatorname{Aut}_Q(X)\cong(1+J(E))\rtimes\prod_{a=1}^s\operatorname{GL}_{m_a}(k).}
$$

This [Levi decomposition of a quiver automorphism group](../../../algebra.md#levi-decomposition-of-a-quiver-automorphism-group) holds in every characteristic; the section is constructed directly from the multiplicity spaces.

## 5

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A representation of the [one-arrow quiver](../../../algebra.md#kronecker-quiver-with-one-arrow) is an $n_2\times n_1$ matrix $F$. If $r=\operatorname{rank}F$, changes of basis put it in the form with an $r\times r$ identity block and all other entries zero. Since multiplication by invertible matrices preserves [matrix rank](../../../vector-space.md#matrix-rank),

$$
\boxed{\mathcal O_X=\{M\in\operatorname{Mat}_{n_2\times n_1}(k):\operatorname{rank}M=r\}.}
$$

This describes the orbit for every $0\leq r\leq\min(n_1,n_2)$, including the zero orbit. Its dimension is

$$
\boxed{\dim\mathcal O_X=r(n_1+n_2-r).}
$$

Indeed, choosing its $r$-dimensional image contributes $r(n_2-r)$ parameters in a [Grassmannian](../../../differential-geometry.md#grassmannian), and choosing a surjective map from $k^{n_1}$ onto that image contributes $rn_1$. This is a [rank orbit of a matrix under left-right multiplication](../../../vector-space.md#rank-orbit-of-a-matrix-under-left-right-multiplication).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

If $y=g\cdot x$, the component maps $g_i$ are invertible and satisfy $g_{t(\rho)}f_\rho=f'_\rho g_{s(\rho)}$. Thus they define a [quiver representation isomorphism](../../../algebra.md#quiver-representation-isomorphism) $X_x\to X_y$. Conversely, any such isomorphism consists of invertible maps $g_i$, and its commuting squares rearrange to $f'_\rho=g_{t(\rho)}f_\rho g_{s(\rho)}^{-1}$. Therefore

$$
\boxed{\mathcal O_X=\{x\in\operatorname{Rep}_Q(\mathbf n):X_x\cong X\}.}
$$

The [base change action on quiver representations](../../../algebra.md#base-change-action-on-quiver-representations) consequently identifies its orbits exactly with isomorphism classes at fixed [dimension vector of a quiver representation](../../../algebra.md#dimension-vector-of-a-quiver-representation).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Split the sequence as vector spaces at each vertex. In these coordinates, the middle arrow maps have block form

$$
f^Y_\rho=\begin{pmatrix}f^X_\rho&\xi_\rho\\0&f^Z_\rho\end{pmatrix}.
$$

For $t\in k^\times$, change basis by $\operatorname{diag}(tI_{X_i},I_{Z_i})$ at every vertex. It changes the off-diagonal block to $t\xi_\rho$. These arrow matrices depend polynomially on $t$ and at $t=0$ give $X\oplus Z$. Thus the [split extension as a degeneration](../../../representation-theory.md#split-extension-as-a-degeneration) shows

$$
\mathcal O_{X\oplus Z}\subseteq\overline{\mathcal O_Y}.
$$

We must check that the two orbits are different. If $Y\cong X\oplus Z$, apply $\operatorname{Hom}_Q(Z,-)$ to the original [short exact sequence](../../../module-theory.md#short-exact-sequence). Exactness makes the kernel of $\operatorname{Hom}(Z,Y)\to\operatorname{End}(Z)$ equal to $\operatorname{Hom}(Z,X)$. The assumed isomorphism of the middle representation gives $\dim\operatorname{Hom}(Z,Y)=\dim\operatorname{Hom}(Z,X)+\dim\operatorname{End}(Z)$, so this map is surjective. In particular the identity of $Z$ lifts to $Z\to Y$, splitting the sequence, a contradiction. Hence the orbits are indeed distinct.

The group $\operatorname{GL}(\mathbf n)$ is irreducible, so $\overline{\mathcal O_Y}$ is irreducible. An algebraic-group orbit is locally closed, hence open in its closure; its boundary is a proper closed subset of smaller dimension. The distinct orbit $\mathcal O_{X\oplus Z}$ lies in that boundary. Therefore

$$
\boxed{\dim\mathcal O_{X\oplus Z}<\dim\mathcal O_Y.}
$$

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

An acyclic finite [quiver](../../../algebra.md#quiver) has integer vertex weights $w_i$ such that $w_j>w_i$ for every arrow $i\to j$; for example, let $w_i$ be the maximum length of a path ending at $i$. For $t\ne0$, act by $g_i(t)=t^{w_i}I_{n_i}$. Then

$$
(g(t)\cdot f)_\rho=t^{w_{t(\rho)}-w_{s(\rho)}}f_\rho.
$$

Every exponent is positive. The arrow matrices therefore extend polynomially to $t=0$ with all arrows zero, which is the origin of the [quiver representation space](../../../algebra.md#quiver-representation-space). The values for $t\ne0$ lie in $\mathcal O_X$, so

$$
\boxed{0\in\overline{\mathcal O_X}\quad\text{for every }X.}
$$

This proves that [acyclic quiver representations degenerate to zero](../../../algebra.md#acyclic-quiver-representations-degenerate-to-zero), also when some vertex spaces are zero.

## 6

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

A nonzero finite-dimensional [quiver representation](../../../algebra.md#representation-of-a-quiver) is a [brick module](../../../module-theory.md#brick-module) when $\operatorname{End}_Q(X)=k\,1_X$. If $X=U\oplus V$ with both summands nonzero, projection onto $U$ is an [idempotent](../../../commutative-algebra.md#idempotent) endomorphism different from zero and the identity. That is impossible in $k\,1_X$. Hence **every brick is indecomposable**.

For the requested converse counterexample, take the [dual-number algebra](../../../commutative-algebra.md#dual-number) $A=k[\varepsilon]/(\varepsilon^2)$ and its left regular module $A$. The algebra is local with maximal ideal $(\varepsilon)$, and it is not simple because this is a nonzero proper ideal. The module is indecomposable: its [endomorphism ring](../../../module-theory.md#endomorphism-ring) is $A^{\mathrm{op}}\cong A$, which has no nontrivial [idempotents](../../../commutative-algebra.md#idempotent). But this ring has dimension two over $k$, so **the regular module is not a brick**. Thus indecomposable need not mean brick without the positive-definiteness hypothesis used below.

<h4 id="6/a/i">i</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6/a/i)

Use the allowed [Ringel lemma on bricks](../../../module-theory.md#ringel-lemma-on-bricks) in the following precise form: a finite-dimensional indecomposable [quiver representation](../../../algebra.md#representation-of-a-quiver) that is not a [brick module](../../../module-theory.md#brick-module) contains a nonzero brick $B$ with $\operatorname{Ext}^1_Q(B,B)\ne0$.

Suppose such a nonbrick indecomposable existed, and let $\mathbf b=\dim B$. The [Tits form of a quiver](../../../algebra.md#tits-form-of-a-quiver) is $q_Q(\mathbf b)=\langle\mathbf b,\mathbf b\rangle_Q$, so the [Ringel form](../../../algebra.md#ringel-form) identity would give

$$
q_Q(\mathbf b)=\dim\operatorname{End}_Q(B)-\dim\operatorname{Ext}^1_Q(B,B)=1-\dim\operatorname{Ext}^1_Q(B,B)\leq0.
$$

Positive definiteness gives $q_Q(\mathbf b)>0$ for nonzero $\mathbf b$, a contradiction. Therefore **every indecomposable is a brick**.

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/a/ii)

If $X$ is indecomposable, part (i) makes it a [brick module](../../../module-theory.md#brick-module). For its nonzero [dimension vector of a quiver representation](../../../algebra.md#dimension-vector-of-a-quiver-representation) $\mathbf n$,

$$
0<q_Q(\mathbf n)=1-\dim\operatorname{Ext}^1_Q(X,X)\leq1.
$$

The [Tits form of a quiver](../../../algebra.md#tits-form-of-a-quiver) takes integer values on integer vectors, so **$q_Q(\mathbf n)=1$ and $X$ has no self-extensions**.

Conversely, suppose $\mathbf n$ has nonnegative integer entries and $q_Q(\mathbf n)=1$. Choose a representation $M$ of that dimension vector whose orbit has maximal dimension. Such an orbit exists because dimensions are integers bounded by $\dim\operatorname{Rep}_Q(\mathbf n)$. If $M=U\oplus V$ with nonzero $U,V$, a nonzero extension in either direction would, by part 5(c), produce a middle representation of the same dimension vector with larger orbit. Hence $\operatorname{Ext}^1_Q(U,V)=\operatorname{Ext}^1_Q(V,U)=0$.

Writing $\mathbf u=\dim U$ and $\mathbf v=\dim V$, the [Ringel form](../../../algebra.md#ringel-form) identity then gives

$$
\begin{aligned}
1=q_Q(\mathbf u+\mathbf v)&=q_Q(\mathbf u)+q_Q(\mathbf v)+\langle\mathbf u,\mathbf v\rangle_Q+\langle\mathbf v,\mathbf u\rangle_Q\\
&=q_Q(\mathbf u)+q_Q(\mathbf v)+\dim\operatorname{Hom}_Q(U,V)+\dim\operatorname{Hom}_Q(V,U)\geq2.
\end{aligned}
$$

The last inequality uses positive integral values of $q_Q$ at both nonzero vectors. This contradiction makes $M$ indecomposable. Thus **the indecomposable dimension vectors are exactly the positive roots $q_Q(\mathbf n)=1$**.

<h4 id="6/a/iii">iii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/a/iii)

An indecomposable of dimension vector $\mathbf n$ is a [brick module](../../../module-theory.md#brick-module) and has $q_Q(\mathbf n)=1$ by the previous parts. Its [automorphism group of a quiver representation](../../../algebra.md#automorphism-group-of-a-quiver-representation) has dimension one. Therefore

$$
\dim\mathcal O_X=\sum_i n_i^2-1=\sum_{\rho:i\to j}n_in_j=\dim\operatorname{Rep}_Q(\mathbf n).
$$

It follows that its orbit is open and dense in the irreducible [quiver representation space](../../../algebra.md#quiver-representation-space). Two different indecomposables of the same dimension vector would give two disjoint nonempty open orbits. Nonempty open subsets of an irreducible space must intersect, so this is impossible. Hence **an indecomposable is uniquely determined by its dimension vector, up to isomorphism**. This is the [positive definite Tits form indecomposable classification](../../../algebra.md#positive-definite-tits-form-indecomposable-classification).

<h4 id="6/a/iv">iv</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#6/a/iv)

If $Q_0$ is empty, there are no nonzero indecomposables and the conclusion is immediate. Otherwise positive definiteness of the [Tits form of a quiver](../../../algebra.md#tits-form-of-a-quiver) gives a constant $c>0$ with $q_Q(v)\geq c\|v\|^2$ for every real vector $v$: take the minimum of $q_Q$ on the compact unit sphere. Every [positive root of a quiver](../../../algebra.md#positive-root-of-a-quiver) therefore satisfies $\|\mathbf n\|^2\leq1/c$. Only finitely many nonnegative integer vectors lie in this bounded set. Parts (ii) and (iii) give exactly one indecomposable isomorphism class for each such root, and no others. Consequently **$Q$ has finite representation type**.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Number the vertices consecutively along the underlying chain. Orientation does not affect the quadratic [Tits form of a quiver](../../../algebra.md#tits-form-of-a-quiver):

$$
q_Q(\mathbf n)=\sum_{i=1}^m n_i^2-\sum_{i=1}^{m-1}n_in_{i+1}=\frac12\sum_{i=0}^m(n_{i+1}-n_i)^2,\qquad n_0=n_{m+1}=0.
$$

If $\mathbf n$ has nonnegative integer coordinates and $q_Q(\mathbf n)=1$, the sum of integer squares on the right is $2$. There are therefore exactly two nonzero consecutive differences, each of absolute value one. Their sum is zero, so one is $+1$ and the other $-1$. Nonnegativity forces the $+1$ to occur first. Thus the [positive roots of type A](../../../algebra.md#positive-roots-of-type-a) are exactly the vectors with **a single nonempty interval of ones and zeros elsewhere**.

There is one such vector for every pair of endpoints $1\leq a\leq b\leq m$, giving

$$
\boxed{\#\{\text{positive roots of type }A_m\}=\frac{m(m+1)}2.}
$$

For $A_3$, the full list is

$$
\boxed{(1,0,0),\ (0,1,0),\ (0,0,1),\ (1,1,0),\ (0,1,1),\ (1,1,1).}
$$

The difference-of-coordinates proof includes $m=1$ and is independent of the chosen arrow orientation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
