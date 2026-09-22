# Paper 3

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2017/paperia_3_0.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2017/paperia_3_0.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2E](#2e)
  - [Solution](#2e/solution)
- [3B](#3b)
  - [Solution](#3b/solution)
- [4B](#4b)
  - [a](#4b/a)
    - [Solution](#4b/a/solution)
  - [b](#4b/b)
    - [Solution](#4b/b/solution)
- [5E](#5e)
  - [Solution](#5e/solution)
- [6E](#6e)
  - [Solution](#6e/solution)
- [7E](#7e)
  - [a](#7e/a)
    - [Solution](#7e/a/solution)
  - [b](#7e/b)
    - [Solution](#7e/b/solution)
- [8E](#8e)
  - [a](#8e/a)
    - [Solution](#8e/a/solution)
  - [b](#8e/b)
    - [Solution](#8e/b/solution)
- [9B](#9b)
  - [a](#9b/a)
    - [Solution](#9b/a/solution)
  - [b](#9b/b)
    - [Solution](#9b/b/solution)
  - [c](#9b/c)
    - [Solution](#9b/c/solution)
- [10B](#10b)
  - [Solution](#10b/solution)
- [11B](#11b)
  - [a](#11b/a)
    - [Solution](#11b/a/solution)
  - [b](#11b/b)
    - [Solution](#11b/b/solution)
  - [c](#11b/c)
    - [Solution](#11b/c/solution)
- [12B](#12b)
  - [a](#12b/a)
    - [Solution](#12b/a/solution)
  - [b](#12b/b)
    - [Solution](#12b/b/solution)
  - [c](#12b/c)
    - [Solution](#12b/c/solution)

## 1E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

Use the [Riemann sphere](../../../complex-analysis.md#riemann-sphere) convention for evaluating a [Möbius transformation](../../../group-theory.md#mobius-transformation) at a pole and at infinity. When the three prescribed points are finite, take

$$
f(z)=\frac{(w_3-w_1)(z-w_2)}{(w_3-w_2)(z-w_1)}.
$$

Its zero is $w_2$, its pole is $w_1$, and substitution at $w_3$ gives one. The remaining three cases are

$$
\boxed{
\begin{array}{c|c}
\text{point at infinity}&f(z)\\ \hline
w_1=\infty&(z-w_2)/(w_3-w_2)\\
w_2=\infty&(w_3-w_1)/(z-w_1)\\
w_3=\infty&(z-w_2)/(z-w_1).
\end{array}}
$$

All coefficient [determinants](../../../linear-algebra.md#determinant) are nonzero because the points are distinct. There is only one such [Möbius transformation](../../../group-theory.md#mobius-transformation): the composite of any two candidate maps, one inverted, fixes $\infty,0,1$; fixing infinity makes it affine, and fixing zero and one makes it the identity.

For this question use the [cross-ratio](../../../group-theory.md#cross-ratio) normalization

$$
\boxed{[w_1,w_2,w_3,w_4]=f(w_4).}
$$

In the finite case this is $(w_3-w_1)(w_4-w_2)/[(w_3-w_2)(w_4-w_1)]$, with the corresponding limits if a point is infinite. It is finite and distinct from zero and one, since $w_4$ is distinct from the other three points and $f$ is a [bijection](../../../function.md#bijection). Ordering conventions for the [cross-ratio](../../../group-theory.md#cross-ratio) differ; the definition here is fixed by the specified images, rather than by importing another ordering formula.

A [generalized circle](../../../group-theory.md#generalized-circle-under-a-mobius-transformation) means either a [circle](../../../topology.md#circle) or a [straight line](../../../geometry-and-topology.md#straight-line) completed by infinity. Let $K$ be the unique [generalized circle](../../../group-theory.md#generalized-circle-under-a-mobius-transformation) through the first three points. Its image under $f$ is the unique [generalized circle](../../../group-theory.md#generalized-circle-under-a-mobius-transformation) through $\infty,0,1$, namely $\mathbb R\cup\{\infty\}$. Therefore $w_4\in K$ exactly when $f(w_4)$ is real. Conversely a real $f(w_4)$ lies on that extended real line, whose inverse image is $K$. This proves the [real cross-ratio criterion for a generalized circle](../../../group-theory.md#real-cross-ratio-criterion-for-a-generalized-circle) in both directions.

## 2E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2e/solution">Solution</h3>

↑ **Parent:** [2E](#2e)

A [subgroup](../../../group.md#subgroup) $H$ of a [group](../../../group.md) $G$ is a [normal subgroup](../../../group-theory.md#normal-subgroup) when $gHg^{-1}=H$ for every $g\in G$, equivalently $gH=Hg$. The [quotient group](../../../group-theory.md#quotient-group) $G/H$ has the left [cosets](../../../group-theory.md#coset) as elements, with $(gH)(kH)=gkH$, identity $H$ and inverse $(gH)^{-1}=g^{-1}H$. Normality makes this multiplication independent of representatives.

The [first isomorphism theorem for groups](../../../group-theory.md#first-isomorphism-theorem) says that for a [group homomorphism](../../../group-theory.md#group-homomorphism) $\varphi:G\to K$, its [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) is normal and

$$
G/\ker\varphi\cong\operatorname{im}\varphi,
\qquad g\ker\varphi\longmapsto\varphi(g).
$$

The image is taken with the induced [group operation](../../../group.md#group-operation); surjectivity onto all of $K$ is not required.

For the given [upper triangular matrices](../../../linear-algebra.md#upper-triangular-matrix), take diagonal entries:

$$
\varphi\!\begin{pmatrix}a&b\\0&d\end{pmatrix}=(a,d)
\quad\text{in}\quad\mathbb R^\times\times\mathbb R^\times.
$$

The target is a [direct product of groups](../../../group-theory.md#direct-product-of-groups), with multiplication of nonzero [real numbers](../../../arithmetic.md#real-number) in each coordinate. Indeed the product of two such [matrices](../../../vector-space.md#matrix) has diagonal $(aa',dd')$, proving the [group homomorphism](../../../group-theory.md#group-homomorphism) property. Any pair of nonzero diagonal entries is attained by a [diagonal matrix](../../../linear-algebra.md#diagonal-matrix), so $\varphi$ is surjective. Its [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) consists precisely of the [matrices](../../../vector-space.md#matrix) with $a=d=1$, namely $H$. Hence

$$
\boxed{H\trianglelefteq G,\qquad G/H\cong(\mathbb R^\times)^2}
$$

with coordinatewise multiplication, not addition on $\mathbb R^2$.

## 3B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3b/solution">Solution</h3>

↑ **Parent:** [3B](#3b)

The boundary ray has $y/x=3/5$, and its intersection with the [hyperbola](../../../geometry-and-topology.md#hyperbola) is $(5/4,3/4)$. Under the given [change of variables](../../../calculus.md#change-of-variables-formula), $x^2-y^2=r^2$ and $y/x=\tanh\theta$. Thus the region becomes

$$
0\leq r\leq1,\qquad 0\leq\theta\leq\operatorname{artanh}(3/5)=\log2.
$$

The [hyperbolic functions](../../../calculus.md#hyperbolic-function) satisfy $\cosh^2\theta-\sinh^2\theta=1$, so the [Jacobian determinant](../../../calculus.md#jacobian-determinant) is

$$
\det\frac{\partial(x,y)}{\partial(r,\theta)}
=\det\begin{pmatrix}\cosh\theta&r\sinh\theta\\\sinh\theta&r\cosh\theta\end{pmatrix}=r.
$$

It is positive in the interior. The coordinate degeneracy at $r=0$ is a boundary set of area zero and does not affect the [change of variables formula](../../../calculus.md#change-of-variables-formula). Therefore

$$
\int_A y\,dx\,dy
=\int_0^{\log2}\int_0^1 r^2\sinh\theta\,dr\,d\theta
=\frac13(\cosh(\log2)-1)
=\boxed{\frac1{12}}.
$$

Here $\cosh(\log2)=5/4$. The PDF specifies two line segments and one hyperbolic arc; the duplicated $y=0$ line in the TeX is not an extra boundary condition.

## 4B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4b/a">a</h3>

↑ **Parent:** [4B](#4b)

<h4 id="4b/a/solution">Solution</h4>

↑ **Parent:** [A](#4b/a)

Use the [Einstein summation convention](../../../linear-algebra.md#einstein-notation). Substitute the given [basis](../../../vector-space.md#basis) transformation into the expansion of the [vector](../../../vector-space.md#vector):

$$
v_j e_j=v'_iR_{ij}e_j.
$$

By [linear independence](../../../vector-space.md#linear-independence) of the [basis](../../../vector-space.md#basis) [vectors](../../../vector-space.md#vector), $v_j=R_{ij}v'_i$. In [matrix](../../../vector-space.md#matrix) notation $v=R^Tv'$. A [rotation matrix](../../../linear-algebra.md#rotation-matrix) is [orthogonal](../../../linear-algebra.md#orthogonal-vectors), so multiplication by $R$ gives

$$
\boxed{v'_i=R_{ij}v_j,\qquad v_i=R_{ji}v'_j.}
$$

The placement of the transpose follows from the specified convention $e'_i=R_{ij}e_j$. It must not be guessed from a different convention for an active rotation of a [vector](../../../vector-space.md#vector).

<h3 id="4b/b">b</h3>

↑ **Parent:** [4B](#4b)

<h4 id="4b/b/solution">Solution</h4>

↑ **Parent:** [B](#4b/b)

The [quotient theorem for Cartesian tensors](../../../linear-algebra.md#quotient-theorem-for-cartesian-tensors) here says: if contracting $T_{ij}$ with every [vector](../../../vector-space.md#vector) $v_j$ gives the components $w_i=T_{ij}v_j$ of a [vector](../../../vector-space.md#vector) in every right-handed [orthonormal basis](../../../linear-algebra.md#orthonormal-basis), then $T$ obeys the second-order [tensor](../../../linear-algebra.md#tensor) transformation law. Conversely that transformation law guarantees the contraction is a [vector](../../../vector-space.md#vector). One may equivalently test that $u_iT_{ij}v_j$ is a [scalar](../../../vector-space.md#scalar) for every pair of [vectors](../../../vector-space.md#vector) $u,v$.

By part (a), $v'=Rv$ and $w'=Rw$. The contraction property in the new [basis](../../../vector-space.md#basis) says

$$
T'Rv=w'=Rw=RTv.
$$

Since this holds for every test [vector](../../../vector-space.md#vector), $T'R=RT$. Using $R^{-1}=R^T$ gives

$$
\boxed{T'=RTR^T,\qquad T'_{ij}=R_{ik}R_{j\ell}T_{k\ell}.}
$$

For the converse, $T'v'=RTR^TRv=RTv=Rw$, exactly the [vector](../../../vector-space.md#vector) law. For the equivalent [scalar](../../../vector-space.md#scalar) formulation, invariance of $u^TTv$ for every $u,v$ gives $u^TR^TT'Rv=u^TTv$, forcing the same [matrix](../../../vector-space.md#matrix) identity.

The quantifier “every” matters: an arbitrary nonzero [matrix](../../../vector-space.md#matrix) can annihilate one fixed [vector](../../../vector-space.md#vector), so a single successful contraction cannot establish tensoriality. The stated [bases](../../../vector-space.md#basis) test proper rotations; transformation under [orthogonal reflections](../../../linear-algebra.md#reflection-in-a-hyperplane) would require an additional hypothesis if that were wanted. “Second-order” counts tensor indices, rather than the [matrix rank](../../../vector-space.md#matrix-rank) of a particular component [matrix](../../../vector-space.md#matrix).

## 5E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5e/solution">Solution</h3>

↑ **Parent:** [5E](#5e)

Restrict the quotient projection $\pi:G\to G/N$ to $H$. This is a [group homomorphism](../../../group-theory.md#group-homomorphism) with

$$
\ker(\pi|_H)=H\cap N.
$$

Its image is a nontrivial [subgroup](../../../group.md#subgroup) of the prime-order [quotient group](../../../group-theory.md#quotient-group), because $H$ is not contained in $N$. By [Lagrange's theorem for finite groups](../../../group-theory.md#lagrange-s-theorem), the image has order $p$ and is all of $G/N$. The [first isomorphism theorem for groups](../../../group-theory.md#first-isomorphism-theorem) therefore gives

$$
\boxed{H\cap N\trianglelefteq H,\qquad [H:H\cap N]=p.}
$$

For the second assertion, partition $C$ into [conjugacy classes](../../../group-theory.md#conjugacy-class) for $N$. Because $N$ is normal, [conjugation](../../../group-theory.md#conjugation) by $G$ permutes these smaller classes: $g\operatorname{Cl}_N(x)g^{-1}=\operatorname{Cl}_N(gxg^{-1})$. This [group action](../../../group-theory.md#group-action) is transitive since any two elements of $C$ are conjugate in $G$. Elements of $N$ fix every $N$-class, so the action factors through $G/N$.

If $m$ is the number of smaller classes, the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) for this transitive action gives $m\mid |G/N|=p$. Thus

$$
\boxed{C\text{ is one }N\text{-class, or a disjoint union of }p\text{ such classes}.}
$$

Distinct [conjugacy classes](../../../group-theory.md#conjugacy-class) are disjoint because they are [orbits of a group action](../../../group-theory.md#orbit-of-a-group-action). This proves [conjugacy class splitting in a prime-index normal subgroup](../../../group-theory.md#conjugacy-class-splitting-in-a-prime-index-normal-subgroup) without assuming all $G$-conjugations are already conjugations by $N$.

## 6E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6e/solution">Solution</h3>

↑ **Parent:** [6E](#6e)

[Lagrange's theorem for finite groups](../../../group-theory.md#lagrange-s-theorem) states that for a [subgroup](../../../group.md#subgroup) $H$ of a finite [group](../../../group.md) $G$, $|G|=[G:H]|H|$. For $x\in G$, two powers among $1,x,\ldots,x^{|G|}$ coincide, giving $x^m=1$ for some positive $m$. The least such exponent $d$ is the [order of a group element](../../../group-theory.md#order-of-a-group-element), and the [cyclic subgroup](../../../group.md#cyclic-subgroup) generated by $x$ consists of the $d$ distinct powers $1,x,\ldots,x^{d-1}$. Apply [Lagrange's theorem for finite groups](../../../group-theory.md#lagrange-s-theorem) to obtain $d\mid|G|$.

[Cauchy's theorem for finite groups](../../../finite-group-theory.md#cauchy-theorem-for-groups) states that if a prime $p$ divides the order of a finite [group](../../../group.md), the [group](../../../group.md) contains an element of order $p$.

The classification of a [group of order eight](../../../finite-group-theory.md#group-of-order-eight) is

$$
\boxed{C_8,\quad C_4\times C_2,\quad C_2\times C_2\times C_2,\quad D_8,\quad Q_8.}
$$

Here $D_8$ denotes the [dihedral group](../../../finite-group-theory.md#dihedral-group) of order eight, not a [group](../../../group.md) of order sixteen. To prove exhaustiveness, every element order is $1,2,4$ or $8$. An element of order eight generates the whole [group](../../../group.md), giving $C_8$.

If no element has order four or eight, every nonidentity element is an [involution](../../../group-theory.md#involution). Since $(ab)^{-1}=ab$ while $a^{-1}=a$ and $b^{-1}=b$, we have $ab=ba$. Choose an [involution](../../../group-theory.md#involution) $a$, another $b$ outside $\langle a\rangle$, and then $c$ outside the four-element [subgroup](../../../group.md#subgroup) $\langle a,b\rangle$. The factors commute and each added factor has trivial intersection with the preceding [subgroup](../../../group.md#subgroup). The [internal direct product theorem](../../../group-theory.md#internal-direct-product-theorem) gives $G\cong C_2^3$, an [elementary abelian group](../../../group.md#elementary-abelian-group).

Otherwise choose $a$ of order four and set $A=\langle a\rangle$. It has index two, so is normal. Choose $b\notin A$. The two [cosets](../../../group-theory.md#coset) show that $a,b$ generate $G$ and that $b^2\in A$. There is no element of order eight, so $b^2$ is either $1$ or $a^2$.

If $G$ is abelian and $b^2=1$, the [internal direct product theorem](../../../group-theory.md#internal-direct-product-theorem) yields $G=A\times\langle b\rangle\cong C_4\times C_2$. If instead $b^2=a^2$, let $c=a^{-1}b$; commutativity gives $c^2=1$ and $c\notin A$, producing the same direct product.

If $G$ is nonabelian, [conjugation](../../../group-theory.md#conjugation) by $b$ is a nonidentity [group automorphism](../../../algebra.md#group-automorphism) of $A$: otherwise $a,b$ would commute and hence so would all of $G$. Thus $bab^{-1}=a^{-1}$. With $b^2=1$ these are the relations of $D_8$; with $b^2=a^2$ they are the relations of the [quaternion group](../../../finite-group-theory.md#quaternion-group) $Q_8$. In either presentation every word reduces to $a^ib^j$, $0\leq i<4$, $0\leq j<2$. The standard eight-element model maps onto $G$, and equal orders make that [group homomorphism](../../../group-theory.md#group-homomorphism) an isomorphism.

Finally [group isomorphisms](../../../algebra.md#group-isomorphism) preserve element orders. The following numbers of elements distinguish all five possibilities:

| [Group](../../../group.md) | Order 1 | Order 2 | Order 4 | Order 8 |
| --- | --- | --- | --- | --- |
| $C_8$ | 1 | 1 | 2 | 4 |
| $C_4\times C_2$ | 1 | 3 | 4 | 0 |
| $C_2^3$ | 1 | 7 | 0 | 0 |
| $D_8$ | 1 | 5 | 2 | 0 |
| $Q_8$ | 1 | 1 | 6 | 0 |

Thus the list is both exhaustive and pairwise non-isomorphic.

## 7E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7e/a">a</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/a/solution">Solution</h4>

↑ **Parent:** [A](#7e/a)

For a [group action](../../../group-theory.md#group-action), the [orbit of a group action](../../../group-theory.md#orbit-of-a-group-action) of $x$ is $Gx=\{gx:g\in G\}$, and its [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) is $G_x=\{g:gx=x\}$. The [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) gives $|Gx||G_x|=|G|$: the map $gG_x\mapsto gx$ is a well-defined [bijection](../../../function.md#bijection) from stabilizer [cosets](../../../group-theory.md#coset) to the orbit.

Within one orbit, the [stabilizer subgroups](../../../group-theory.md#stabilizer-subgroup) are conjugate, since $G_{hx}=hG_xh^{-1}$. Their sizes are therefore equal. Summing stabilizer sizes over a single orbit gives $|Gx||G_x|=|G|$, and summing over all $n$ orbits yields

$$
\boxed{\sum_{x\in X}|\operatorname{Stab}(x)|=n|G|.}
$$

Now count the pairs $(g,x)$ fixed by the action in two ways. Holding $x$ fixed gives $|G_x|$ choices of $g$, whereas holding $g$ fixed gives $|\operatorname{Fix}(g)|$ choices of $x$. Thus

$$
|S|=\sum_{x\in X}|G_x|=\sum_{g\in G}|\operatorname{Fix}(g)|.
$$

Combining the two identities proves [Burnside lemma](../../../representation-theory.md#burnside-s-lemma):

$$
\boxed{n=\frac1{|G|}\sum_{g\in G}|\operatorname{Fix}(g)|.}
$$

The finiteness hypotheses justify these cardinality sums. If $X$ is empty, every sum and the orbit count are zero, so the formula still applies.

<h3 id="7e/b">b</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/b/solution">Solution</h4>

↑ **Parent:** [B](#7e/b)

Centre the cube at the origin with faces having normals $\pm e_1,\pm e_2,\pm e_3$. Every rotational symmetry fixes the centre and permutes these normals, so its [rotation matrix](../../../linear-algebra.md#rotation-matrix) is a [signed permutation matrix](../../../vector-space.md#signed-permutation-matrix) of [determinant](../../../linear-algebra.md#determinant) one. Conversely any such [matrix](../../../vector-space.md#matrix) permutes the cube’s coordinates up to signs and preserves the cube. For each of $3!$ coordinate [permutations](../../../combinatorics.md#permutation), four of the eight choices of signs give [determinant](../../../linear-algebra.md#determinant) one. Consequently the [rotational symmetry group of a cube](../../../group-theory.md#rotational-symmetry-group-of-a-cube) has

$$
\boxed{|H|=3!\,2^2=24.}
$$

This counts the rotations directly, without an unverified stabilizer calculation. The TeX’s $2^k$ is damaged transcription: the PDF prints 24.

Let $X$ be the $3^6$ face colourings. A colouring fixed by a rotation must be constant on each [permutation cycle](../../../finite-group-theory.md#permutation-cycle) of faces, giving $3^c$ fixed colourings if the rotation has $c$ face cycles. The rotation types are:

| Rotation | Number | Face cycle type | Fixed colourings |
| --- | --- | --- | --- |
| Identity | 1 | $1^6$ | $3^6$ |
| Quarter-turn about opposite face centres | 6 | $1^2 4$ | $3^3$ |
| Half-turn about opposite face centres | 3 | $1^2 2^2$ | $3^4$ |
| Half-turn about opposite edge midpoints | 6 | $2^3$ | $3^3$ |
| Third-turn about opposite vertices | 8 | $3^2$ | $3^2$ |

There are three face axes, each with two quarter-turns and one half-turn; six edge axes, each with one half-turn; and four vertex axes, each with two nonidentity third-turns. These rotations are distinct and, with the identity, total 24, so the table is exhaustive. Face-axis rotations fix their two axial faces; the remaining four faces cycle or pair. Edge half-turns pair all faces, while vertex third-turns form two triples.

[Burnside lemma](../../../representation-theory.md#burnside-s-lemma) now gives

$$
\boxed{|X/H|=\frac{3^6+6\cdot3^3+3\cdot3^4+6\cdot3^3+8\cdot3^2}{24}=57.}
$$

The three colours are labelled, [orthogonal reflections](../../../linear-algebra.md#reflection-in-a-hyperplane) are excluded, and no condition requires every colour to appear.

## 8E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8e/a">a</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/a/solution">Solution</h4>

↑ **Parent:** [A](#8e/a)

With rightmost-first composition, a [permutation cycle](../../../finite-group-theory.md#permutation-cycle) satisfies

$$
(a_1\ a_2\ \cdots\ a_m)
=(a_1\ a_m)(a_1\ a_{m-1})\cdots(a_1\ a_2).
$$

Tracing each $a_j$ verifies the equality, and every other letter is fixed. Thus every cycle is a product of [transpositions](../../../combinatorics.md#transposition-permutation); decomposing a [permutation](../../../combinatorics.md#permutation) into [disjoint permutation cycles](../../../finite-group-theory.md#disjoint-permutation-cycles) proves that every element of $S_n$ is such a product. The identity is the empty product.

To establish that parity is well defined, use the [permutation matrix](../../../vector-space.md#permutation-matrix) $P_\sigma$ defined by $P_\sigma e_i=e_{\sigma(i)}$. Its [determinant](../../../linear-algebra.md#determinant) is $\pm1$, and $P_{\sigma\tau}=P_\sigma P_\tau$. A [transposition](../../../combinatorics.md#transposition-permutation) swaps two columns of the [identity matrix](../../../vector-space.md#identity-matrix) and has [determinant](../../../linear-algebra.md#determinant) $-1$. Therefore if $\sigma$ is expressed as a product of $r$ [transpositions](../../../combinatorics.md#transposition-permutation),

$$
\det P_\sigma=(-1)^r.
$$

The left side depends only on $\sigma$, so any two decompositions have the same parity. Define

$$
\boxed{\operatorname{sgn}(\sigma)=\det P_\sigma=(-1)^r.}
$$

Multiplicativity of the [determinant](../../../linear-algebra.md#determinant) makes this the [sign homomorphism](../../../finite-group-theory.md#sign-homomorphism). Its [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) is the [alternating group](../../../finite-group-theory.md#alternating-group)

$$
\boxed{A_n=\{\sigma\in S_n:\operatorname{sgn}(\sigma)=1\}.}
$$

It is a [normal subgroup](../../../group-theory.md#normal-subgroup) consisting of the [even permutations](../../../finite-group-theory.md#even-permutation). For $n\geq2$ the sign map is surjective because a [transposition](../../../combinatorics.md#transposition-permutation) has sign $-1$, so $[S_n:A_n]=2$. For $n=1$ both [groups](../../../group.md) are trivial.

<h3 id="8e/b">b</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/b/solution">Solution</h4>

↑ **Parent:** [B](#8e/b)

Write $c=(1\ 2\ \cdots\ n)$, with $n\geq2$. [Conjugation](../../../group-theory.md#conjugation) relabels a [transposition](../../../combinatorics.md#transposition-permutation), so

$$
c^j(1\ 2)c^{-j}=(1+j\ 2+j),
$$

where labels are read modulo $n$. In particular the [subgroup](../../../group.md#subgroup) contains $(1\ 2),(2\ 3),\ldots,(n-1\ n)$. These are the edge [transpositions](../../../combinatorics.md#transposition-permutation) of a path through all letters; [transpositions on a connected graph generate the symmetric group](../../../finite-group-theory.md#transpositions-on-a-connected-graph-generate-the-symmetric-group), so the two original generators generate $S_n$.

For the general separation $k$, conjugating $t=(1\ 1+k)$ produces every edge [transposition](../../../combinatorics.md#transposition-permutation) $(i\ i+k)$ modulo $n$. The components of this [graph](../../../graph.md) are precisely the residue classes modulo $d=\gcd(n,k)$: moving along an edge adds or subtracts $k$, and the [subgroup](../../../group.md#subgroup) of $\mathbb Z/n\mathbb Z$ generated by $k$ consists of multiples of $d$. Hence, if $d=1$, the [graph](../../../graph.md) is connected and the same [graph](../../../graph.md) argument gives the whole [symmetric group](../../../finite-group-theory.md#symmetric-group).

For completeness, the [graph](../../../graph.md) argument can be proved without assuming a generating-set theorem. On a simple path $v_0,\ldots,v_\ell$, put $t_j=(v_{j-1}\ v_j)$. Then

$$
(v_0\ v_\ell)=t_1\cdots t_{\ell-1}t_\ell t_{\ell-1}\cdots t_1.
$$

This is a conjugate of the last edge [transposition](../../../combinatorics.md#transposition-permutation); connectivity therefore supplies every [transposition](../../../combinatorics.md#transposition-permutation), and part (a) supplies every [permutation](../../../combinatorics.md#permutation).

If $d>1$, there are $d$ residue blocks of size $n/d>1$, since $1\leq k<n$. The cycle $c$ permutes these blocks, and $t$ swaps two letters in the same block. Both preserve this [block system](../../../group-theory.md#block-system), so their generated [subgroup](../../../group.md#subgroup) does too. The full $S_n$ does not: a [transposition](../../../combinatorics.md#transposition-permutation) exchanging one letter of two different blocks sends a block to a mixture of them. Thus the [subgroup](../../../group.md#subgroup) is proper. This proves

$$
\boxed{\langle(1\ 1+k),(1\ 2\ \cdots\ n)\rangle=S_n
\iff \gcd(n,k)=1.}
$$

Thus [a cycle and a transposition generate the symmetric group exactly at coprime separation](../../../finite-group-theory.md#a-cycle-and-a-transposition-generate-the-symmetric-group-exactly-at-coprime-separation). The obstruction is preservation of a partition, not failure of transitivity: the $n$-cycle already acts transitively even when $d>1$.

## 9B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9b/a">a</h3>

↑ **Parent:** [9B](#9b)

<h4 id="9b/a/solution">Solution</h4>

↑ **Parent:** [A](#9b/a)

Assume $B$ is [continuously differentiable](../../../calculus.md#continuously-differentiable-function). Apply the [chain rule](../../../calculus.md#chain-rule) to each component with $z_j=tx_j$:

$$
\partial_{x_j}F_i=t\partial_{z_j}B_i(tx),\qquad
\partial_tF_i=x_j\partial_{z_j}B_i(tx).
$$

Contracting the first identity with $x_j$ proves

$$
\boxed{(x\cdot\nabla)F=t\,\partial_tF.}
$$

Here $\nabla$ differentiates with respect to $x$ at fixed $t$, while the [time derivative](../../../calculus.md#time-derivative) holds $x$ fixed. The equality follows directly even at $t=0$; no division by $t$ is needed. It holds componentwise for the [vector field](../../../calculus.md#vector-field), so it is not restricted to [scalar](../../../vector-space.md#scalar) functions.

<h3 id="9b/b">b</h3>

↑ **Parent:** [9B](#9b)

<h4 id="9b/b/solution">Solution</h4>

↑ **Parent:** [B](#9b/b)

For a twice [continuously differentiable](../../../calculus.md#continuously-differentiable-function) [vector potential](../../../calculus.md#vector-potential) $A$, write the [curl](../../../calculus.md#curl) with the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol):

$$
\nabla\cdot B=\partial_i(\epsilon_{ijk}\partial_jA_k)
=\epsilon_{ijk}\partial_i\partial_jA_k.
$$

The second derivatives are symmetric in $i,j$, whereas $\epsilon_{ijk}$ is antisymmetric, so the contraction is zero. Equivalently, writing out the three components shows that each mixed derivative cancels its reversed-order partner. Thus

$$
\boxed{\nabla\cdot(\nabla\times A)=0.}
$$

This is [divergence of a curl is zero](../../../calculus.md#divergence-of-a-curl-is-zero). The regularity hypothesis is what licenses commutation of the mixed [partial derivatives](../../../calculus.md#partial-derivative); it must not be omitted for a singular potential without specifying a weaker derivative interpretation.

<h3 id="9b/c">c</h3>

↑ **Parent:** [9B](#9b)

<h4 id="9b/c/solution">Solution</h4>

↑ **Parent:** [C](#9b/c)

Use the usual setting of a [continuously differentiable](../../../calculus.md#continuously-differentiable-function) [solenoidal vector field](../../../calculus.md#solenoidal-vector-field) defined on all radial segments from the origin, including the origin. More generally an open [star-shaped set](../../../algebra.md#star-shaped-set) containing zero suffices. [Differentiation under the integral sign](../../../analysis.md#differentiation-under-the-integral-sign) gives

$$
\nabla\cdot D(x)=\int_0^1t^2(\nabla\cdot B)(tx)\,dt=0.
$$

Apply [divergence and curl of a cross product](../../../calculus.md#divergence-and-curl-of-a-cross-product) with the second field $x$, using $\nabla\cdot x=3$ and $(D\cdot\nabla)x=D$:

$$
\nabla\times(D\times x)=3D-x(\nabla\cdot D)+(x\cdot\nabla)D-D
=2D+(x\cdot\nabla)D.
$$

The scaling identity in part (a) now converts the last expression to a one-variable derivative:

$$
2D+(x\cdot\nabla)D
=\int_0^1\left(2tB(tx)+t^2\frac d{dt}B(tx)\right)dt
=\left[t^2B(tx)\right]_0^1=B(x).
$$

Continuity at the origin ensures the lower endpoint is zero. Hence the [radial vector potential of a solenoidal vector field](../../../calculus.md#radial-vector-potential-of-a-solenoidal-vector-field) is

$$
\boxed{A(x)=D(x)\times x,\qquad \nabla\times A=B.}
$$

The order of the [cross product](../../../vector-space.md#cross-product) matters: $x\times D$ would produce $-B$. This construction is not valid on every punctured or multiply connected domain. For example $B=x/|x|^3$ is solenoidal away from zero, but its radial integral diverges at zero and it has nonzero flux through a surrounding [sphere](../../../geometry-and-topology.md#sphere). The stated formula therefore implicitly needs the regular radial-domain hypothesis, rather than just local zero [divergence](../../../calculus.md#divergence).

## 10B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10b/solution">Solution</h3>

↑ **Parent:** [10B](#10b)

Let $a$ be any constant [vector](../../../vector-space.md#vector) and take $u=\phi a$. The [product rule for divergence](../../../calculus.md#product-rule-for-divergence) gives $\nabla\cdot u=a\cdot\nabla\phi$. The [divergence theorem](../../../calculus.md#divergence-theorem) on a bounded region with piecewise smooth boundary, oriented outward, therefore yields

$$
a\cdot\int_V\nabla\phi\,dV=a\cdot\int_S\phi\,d\mathbf S.
$$

Since $a$ is arbitrary, equality of all components proves

$$
\boxed{\int_V\nabla\phi\,dV=\int_S\phi\,d\mathbf S.}
$$

Here $\phi$ is [continuously differentiable](../../../calculus.md#continuously-differentiable-function) on a neighbourhood of the closed region.

For the side of this [right circular cone](../../../geometry-and-topology.md#right-circular-cone), the parameter tangents are $x_r=(\cos\theta,\sin\theta,\sqrt3)$ and $x_\theta=(-r\sin\theta,r\cos\theta,0)$. Their [cross product](../../../vector-space.md#cross-product) in the outward order is

$$
\boxed{d\mathbf S=(x_\theta\times x_r)\,dr\,d\theta
=(\sqrt3\cos\theta,\sqrt3\sin\theta,-1)r\,dr\,d\theta.}
$$

The sign is outward because the solid [right circular cone](../../../geometry-and-topology.md#right-circular-cone) lies at smaller cylindrical radius for fixed height. Reversing the parameter order reverses the [oriented surface element](../../../calculus.md#oriented-surface-element).

To check the integral identity, the closed boundary must include the top [Euclidean disk](../../../topology.md#disk-mathematics) $z=1$, radius $1/\sqrt3$, as well as the curved side. For $\phi=z^2$, horizontal components cancel on integrating $\theta$. The side contribution is

$$
\int_{\rm side}\phi\,d\mathbf S
=-2\pi\int_0^{1/\sqrt3}3r^3\,dr\,e_z
=-\frac\pi6e_z.
$$

On the top [Euclidean disk](../../../topology.md#disk-mathematics) $\phi=1$ and $d\mathbf S=e_z\,dA$, so its contribution is $(\pi/3)e_z$. The total is $(\pi/6)e_z$. Independently, the cross-section of the solid at height $z$ has area $\pi z^2/3$, and $\nabla\phi=2ze_z$, giving

$$
\int_V\nabla\phi\,dV
=\int_0^1 2z\frac{\pi z^2}{3}\,dz\,e_z
=\boxed{\frac\pi6e_z}.
$$

Thus the two sides agree. The curved side alone is not a closed surface and does not satisfy this volume identity. The apex has zero area; alternatively one can truncate at height $\varepsilon$ and let $\varepsilon\downarrow0$, with the extra boundary contribution vanishing.

## 11B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11b/a">a</h3>

↑ **Parent:** [11B](#11b)

<h4 id="11b/a/solution">Solution</h4>

↑ **Parent:** [A](#11b/a)

For an [arc-length parametrization](../../../differential-geometry.md#arc-length-parametrization), the [unit tangent vector](../../../differential-geometry.md#unit-tangent-vector) is $t=r'(s)$, with $|t|=1$. Its derivative is perpendicular to $t$. The [curvature of a space curve](../../../differential-geometry.md#curvature-of-a-space-curve) is $\kappa=|t'|$; where $\kappa>0$, its [principal normal vector](../../../differential-geometry.md#principal-normal-vector) is $n=t'/\kappa$, so $t'=\kappa n$. The [binormal vector](../../../differential-geometry.md#binormal-vector) $b=t\times n$ completes the positively oriented [Frenet frame](../../../differential-geometry.md#frenet-frame).

Differentiate $b\cdot b=1$ to get $b'\cdot b=0$. Also

$$
\frac d{ds}(b\cdot t)=0
\quad\Longrightarrow\quad b'\cdot t=-b\cdot t'=-\kappa b\cdot n=0.
$$

Thus $b'$ has only an $n$ component. Define the [torsion of a space curve](../../../differential-geometry.md#torsion-of-a-curve) by $\tau=-b'\cdot n$, giving $b'=-\tau n$.

Next, $n'\cdot n=0$, and differentiating the other inner products gives $n'\cdot t=-\kappa$ and $n'\cdot b=\tau$. Hence the [Frenet-Serret formulas](../../../differential-geometry.md#frenet-serret-formulas) are

$$
\boxed{t'=\kappa n,\qquad b'=-\tau n,\qquad n'=-\kappa t+\tau b.}
$$

These statements require enough smoothness, for example a $C^3$ [curve](../../../topology.md#curve) with positive curvature on the interval under discussion. If $\kappa=0$, the [unit tangent vector](../../../differential-geometry.md#unit-tangent-vector) is still defined, but the standard [principal normal vector](../../../differential-geometry.md#principal-normal-vector), [binormal vector](../../../differential-geometry.md#binormal-vector) and [torsion of a space curve](../../../differential-geometry.md#torsion-of-a-curve) need not be; their existence cannot be inferred just from smoothness of the [curve](../../../topology.md#curve).

<h3 id="11b/b">b</h3>

↑ **Parent:** [11B](#11b)

<h4 id="11b/b/solution">Solution</h4>

↑ **Parent:** [B](#11b/b)

Let $F=|\mathbf F|>0$ and choose an orientation of a [regular curve](../../../differential-geometry.md#regular-curve) following the [vector field](../../../calculus.md#vector-field). Its [unit tangent vector](../../../differential-geometry.md#unit-tangent-vector) is $t=\sigma\mathbf F/F$, where $\sigma=\pm1$ is constant along a connected regular segment. [Arc length](../../../riemannian-geometry.md#arc-length) differentiation along that [curve](../../../topology.md#curve) is $d/ds=(\sigma\mathbf F/F)\cdot\nabla$. Therefore

$$
\frac{dt}{ds}
=\frac1F(\mathbf F\cdot\nabla)\left(\frac{\mathbf F}{F}\right)
=\frac{(\mathbf F\cdot\nabla)\mathbf F}{F^2}
-\frac{\mathbf F(\mathbf F\cdot\nabla)F}{F^3}.
$$

Taking the [cross product](../../../vector-space.md#cross-product) with $t$ removes the term parallel to $\mathbf F$:

$$
t\times\frac{dt}{ds}
=\sigma\frac{\mathbf F\times(\mathbf F\cdot\nabla)\mathbf F}{F^3}.
$$

Where the [Frenet frame](../../../differential-geometry.md#frenet-frame) exists, $t\times t'=\kappa(t\times n)=\kappa b$. Thus

$$
\boxed{\frac{\mathbf F\times(\mathbf F\cdot\nabla)\mathbf F}{F^3}
=\sigma\kappa b.}
$$

The printed sign corresponds to orientation along or against the field. Taking magnitudes gives the orientation-independent [curvature of an integral curve of a vector field](../../../calculus.md#curvature-of-an-integral-curve-of-a-vector-field), $\kappa=|\mathbf F\times(\mathbf F\cdot\nabla)\mathbf F|/F^3$. This [scalar](../../../vector-space.md#scalar) formula also applies at zero curvature, where $b$ itself may be undefined.

<h3 id="11b/c">c</h3>

↑ **Parent:** [11B](#11b)

<h4 id="11b/c/solution">Solution</h4>

↑ **Parent:** [C](#11b/c)

The [directional derivative](../../../calculus.md#directional-derivative) along the specified [vector field](../../../calculus.md#vector-field) gives

$$
(\mathbf F\cdot\nabla)\mathbf F=(x,y,z),\qquad
\mathbf F\times(\mathbf F\cdot\nabla)\mathbf F=(2yz,-2xz,0).
$$

Use the magnitude formula for the [curvature of an integral curve of a vector field](../../../calculus.md#curvature-of-an-integral-curve-of-a-vector-field):

$$
\boxed{\kappa(x,y,z)=\frac{2|z|\sqrt{x^2+y^2}}{(x^2+y^2+z^2)^{3/2}},\qquad (x,y,z)\ne(0,0,0).}
$$

It vanishes on the [plane](../../../geometry-and-topology.md#plane) $z=0$ and on the $z$ axis away from the origin, consistent with straight field lines there. At the origin the [vector field](../../../calculus.md#vector-field) vanishes, so it fails the nowhere-zero hypothesis and this field-line curvature is not defined.

As an independent geometric check, an [integral curve of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) satisfies $\dot x=x$, $\dot y=y$, $\dot z=-z$, giving $(x,y,z)=(ae^u,be^u,ce^{-u})$. Its velocity is $(x,y,-z)$ and acceleration $(x,y,z)$; the ordinary [curvature of a space curve](../../../differential-geometry.md#curvature-of-a-space-curve) formula $|r'\times r''|/|r'|^3$ gives the same expression.

## 12B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12b/a">a</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/a/solution">Solution</h4>

↑ **Parent:** [A](#12b/a)

Work with real-valued smooth functions on the bounded region enclosed by $S$, with the [oriented surface element](../../../calculus.md#oriented-surface-element) pointing outward. Set $\psi=\phi-\phi_1$. It is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) in $V$ and has zero [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition) on $S$. Applying [Green's first identity](../../../partial-differential-equation.md#green-s-first-identity) to $\psi$ with itself gives

$$
\int_V|\nabla\psi|^2\,dV
=\int_S\psi\,\partial_n\psi\,dS-\int_V\psi\Delta\psi\,dV=0.
$$

Both terms on the right vanish by the boundary condition and harmonicity. The integrand is nonnegative and continuous, so $\nabla\psi=0$ throughout $V$. Consequently $\psi$ is constant on each [connected component](../../../geometry-and-topology.md#connected-component); every bounded component meets the prescribed boundary, where that constant is zero. Therefore

$$
\boxed{\phi_1=\phi\text{ throughout }V.}
$$

This is the energy proof of [Uniqueness of the Dirichlet problem](../../../analysis.md#uniqueness-of-the-dirichlet-problem). Connectedness of $V$ is not essential if the boundary values are prescribed on every component. Boundedness, or suitable decay and integrability at infinity, is needed for the boundary/energy argument; the finite enclosed-volume interpretation is used here.

<h3 id="12b/b">b</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/b/solution">Solution</h4>

↑ **Parent:** [B](#12b/b)

Put $h=u-\phi-C$. Then $h=0$ on $S$, and the constant does not change a [gradient](../../../calculus.md#gradient), so $\nabla u=\nabla\phi+\nabla h$. Expand the unnormalized [Dirichlet energy](../../../differential-geometry.md#dirichlet-energy):

$$
\int_V|\nabla u|^2\,dV
=\int_V|\nabla\phi|^2\,dV
+2\int_V\nabla\phi\cdot\nabla h\,dV
+\int_V|\nabla h|^2\,dV.
$$

The cross term is zero by [Green's first identity](../../../partial-differential-equation.md#green-s-first-identity):

$$
\int_V\nabla\phi\cdot\nabla h\,dV
=\int_Sh\,\partial_n\phi\,dS-\int_Vh\Delta\phi\,dV=0.
$$

Thus the useful stronger identity is

$$
\boxed{\int_V|\nabla u|^2\,dV-\int_V|\nabla\phi|^2\,dV
=\int_V|\nabla(u-\phi-C)|^2\,dV\geq0.}
$$

Equality holds exactly when $h$ has zero [gradient](../../../calculus.md#gradient). It is then constant on every [connected component](../../../geometry-and-topology.md#connected-component) and zero on that component’s boundary, hence $h=0$. Therefore **equality holds precisely when $u=\phi+C$ throughout $V$.** This is the [Dirichlet principle](../../../calculus-of-variations.md#dirichlet-principle); an additive boundary constant does not alter the minimizing energy. The energy here omits the optional factor $1/2$, which does not affect minimizers or the inequality.

<h3 id="12b/c">c</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/c/solution">Solution</h4>

↑ **Parent:** [C](#12b/c)

Let $E(t)=\int_V|\nabla w|^2\,dV$, using real-valued smooth $w$ and a fixed bounded region. [Differentiation under the integral sign](../../../analysis.md#differentiation-under-the-integral-sign) and [Green's first identity](../../../partial-differential-equation.md#green-s-first-identity) yield

$$
\begin{aligned}
E'(t)&=2\int_V\nabla w\cdot\nabla w_t\,dV\\
&=2\int_Sw_t\partial_nw\,dS-2\int_Vw_t\Delta w\,dV.
\end{aligned}
$$

The boundary term vanishes because $w_t=0$ on $S$, and the [heat equation](../../../diffusion-equation.md#heat-equation) gives $w_t=\Delta w$ in $V$. Consequently

$$
\boxed{E'(t)=-2\int_V(\Delta w)^2\,dV\leq0.}
$$

The integrand is continuous and nonnegative. Thus at any fixed time, equality is equivalent to $\Delta w=0$ everywhere in $V$, also giving $w_t=0$ there at that time. This proves [Dirichlet energy dissipation for the heat equation](../../../diffusion-equation.md#dirichlet-energy-dissipation-for-the-heat-equation).

The boundary condition fixes the boundary temperature in time; it is not a zero normal derivative condition. No sign condition on $\partial_nw$ is used. The stated smoothness licenses the time derivative, spatial [integration by parts](../../../calculus.md#integration-by-parts) and boundary trace; without that regularity an appropriate weak energy argument would be required.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
