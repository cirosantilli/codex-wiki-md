# Paper 3

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2013/PaperIA_3.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2013/PaperIA_3.pdf)

**Table of contents**

- [1D](#1d)
  - [Solution](#1d/solution)
  - [i](#1d/i)
  - [ii](#1d/ii)
  - [iii](#1d/iii)
- [2D](#2d)
  - [Solution](#2d/solution)
- [3C](#3c)
  - [i](#3c/i)
    - [Solution](#3c/i/solution)
  - [ii](#3c/ii)
    - [Solution](#3c/ii/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5D](#5d)
  - [a](#5d/a)
    - [Solution](#5d/a/solution)
  - [b](#5d/b)
    - [Solution](#5d/b/solution)
- [6D](#6d)
  - [a](#6d/a)
    - [i](#6d/a/i)
      - [Solution](#6d/a/i/solution)
    - [ii](#6d/a/ii)
      - [Solution](#6d/a/ii/solution)
  - [b](#6d/b)
    - [Solution](#6d/b/solution)
- [7D](#7d)
  - [a](#7d/a)
    - [Solution](#7d/a/solution)
  - [b](#7d/b)
    - [i](#7d/b/i)
      - [Solution](#7d/b/i/solution)
    - [ii](#7d/b/ii)
      - [Solution](#7d/b/ii/solution)
- [8D](#8d)
  - [Solution](#8d/solution)
- [9C](#9c)
  - [Solution](#9c/solution)
- [10C](#10c)
  - [Solution](#10c/solution)
- [11C](#11c)
  - [Solution](#11c/solution)
- [12C](#12c)
  - [a](#12c/a)
    - [Solution](#12c/a/solution)
  - [b](#12c/b)
    - [Solution](#12c/b/solution)

## 1D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1d/solution">Solution</h3>

↑ **Parent:** [1D](#1d)

[Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem) states that for a [subgroup](../../../group.md#subgroup) $L$ of a [finite group](../../../group.md#finite-group) $G$, $|G|=[G:L]|L|$. In particular $|L|$ divides $|G|$; the equal-sized [cosets](../../../group-theory.md#coset) partition $G$.

Apply the theorem to $H\cap K$ inside both [subgroups](../../../group.md#subgroup). Its order divides both coprime orders, so **$H\cap K=\{1\}$**. For $h\in H$ and $k\in K$, the [group commutator](../../../group.md#group-commutator) $hkh^{-1}k^{-1}$ lies in $K$ by $K$ being a [normal subgroup](../../../group-theory.md#normal-subgroup), and in $H$ because $kh^{-1}k^{-1}\in H$. It is therefore the identity. Thus **every element of $H$ commutes with every element of $K$**.

Define $\theta:H\times K\to G$ by $\theta(h,k)=hk$. The cross-commutation just proved gives $\theta(h,k)\theta(h',k')=hh'kk'=\theta(hh',kk')$, so this is a [group homomorphism](../../../group-theory.md#group-homomorphism) from the [direct product of groups](../../../group-theory.md#direct-product-of-groups). The product assumption makes it surjective. If $hk=1$, then $h=k^{-1}\in H\cap K$, so both entries are the identity and the [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) is trivial. Hence

$$
\boxed{G\cong H\times K,\qquad(h,k)\longmapsto hk.}
$$

This proves the [internal direct product theorem](../../../group-theory.md#internal-direct-product-theorem) in the present coprime-order setting, rather than merely matching the numbers of elements.

<h3 id="1d/i">i</h3>

↑ **Parent:** [1D](#1d)

Coprimality makes the intersection trivial by the subgroup-order divisibility theorem.

<h3 id="1d/ii">ii</h3>

↑ **Parent:** [1D](#1d)

The product hypothesis supplies surjectivity of the multiplication map.

<h3 id="1d/iii">iii</h3>

↑ **Parent:** [1D](#1d)

Both factors being [normal subgroups](../../../group-theory.md#normal-subgroup) places cross-commutators in their intersection, forcing cross-commutation.

## 2D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2d/solution">Solution</h3>

↑ **Parent:** [2D](#2d)

A [cyclic group](../../../group.md#cyclic-group) has one [generator of a group](../../../group.md#generator-of-a-group): $G=\langle a\rangle=\{a^j:j\in\mathbb Z\}$. An [abelian group](../../../group.md#abelian-group) has $xy=yx$ for every pair of elements. Powers of one element commute because $a^ra^s=a^{r+s}=a^{s+r}=a^sa^r$, so **every [cyclic group](../../../group.md#cyclic-group) is [Abelian](../../../group.md#abelian-group)**. The [Klein four-group](../../../finite-group-theory.md#klein-four-group) $C_2\times C_2$ is [Abelian](../../../group.md#abelian-group) but is not a [cyclic group](../../../group.md#cyclic-group): every nonidentity element has order two, whereas a [generator of a group](../../../group.md#generator-of-a-group) for a four-element [cyclic group](../../../group.md#cyclic-group) would have order four.

Fix a [generator of a group](../../../group.md#generator-of-a-group) $x$ of $C_n$. A [group homomorphism](../../../group-theory.md#group-homomorphism) is determined by $g=\phi(x)$ because $\phi(x^j)=g^j$, and the relation $x^n=1$ forces $g^n=1$. Conversely, such a $g$ defines $\phi(x^j)=g^j$: exponents differing by a multiple of $n$ give the same value, and addition of exponents verifies the [group homomorphism](../../../group-theory.md#group-homomorphism) law. Thus the [homomorphism from a finite cyclic group](../../../group.md#homomorphism-from-a-finite-cyclic-group) correspondence is

$$
\boxed{\operatorname{Hom}(C_n,G)\ \longleftrightarrow\ \{g\in G:g^n=1\}.}
$$

For $S_4$, the order of a [permutation](../../../combinatorics.md#permutation) is the [least common multiple](../../../number-theory.md#least-common-multiple) of its disjoint cycle lengths. The condition $\sigma^4=1$ allows identity, [transpositions](../../../combinatorics.md#transposition-permutation), two disjoint [transpositions](../../../combinatorics.md#transposition-permutation), and four-cycles. The **sixteen homomorphisms** are $\phi_\sigma(x^j)=\sigma^j$, with the full list of possible generator images

$$
\boxed{\begin{gathered}
1;\\
(12),(13),(14),(23),(24),(34);\\
(12)(34),(13)(24),(14)(23);\\
(1234),(1243),(1324),(1342),(1423),(1432).
\end{gathered}}
$$

The remaining eight elements of the [symmetric group](../../../finite-group-theory.md#symmetric-group) are [three-cycles](../../../finite-group-theory.md#three-cycle) and do not qualify.

## 3C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3c/i">i</h3>

↑ **Parent:** [3C](#3c)

<h4 id="3c/i/solution">Solution</h4>

↑ **Parent:** [I](#3c/i)

[Differentiation](../../../calculus.md#differentiation) gives $\mathbf r'=e^t(\sqrt2,-\sin t-\cos t,\cos t-\sin t)$. The squared [speed](../../../classical-mechanics.md#speed) is $4e^{2t}$, so the [arc length](../../../riemannian-geometry.md#arc-length) is

$$
\boxed{\int_0^1|\mathbf r'|\,dt=2(e-1).}
$$

The [speed](../../../classical-mechanics.md#speed) never vanishes, so this is a [regular curve](../../../differential-geometry.md#regular-curve) throughout its parameter range.

<h3 id="3c/ii">ii</h3>

↑ **Parent:** [3C](#3c)

<h4 id="3c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3c/ii)

Use the [arc length](../../../riemannian-geometry.md#arc-length) coordinate oriented in the direction of increasing $t$: $s(t)=\int_0^t2e^\tau\,d\tau=2(e^t-1)$, with $s>-2$. Also $\mathbf r''=e^t(\sqrt2,-2\cos t,-2\sin t)$, giving $|\mathbf r''|^2=6e^{2t}$ and $\mathbf r'\cdot\mathbf r''=4e^{2t}$. The [Lagrange identity for the cross product](../../../calculus.md#lagrange-identity-for-the-cross-product) yields

$$
|\mathbf r'\times\mathbf r''|^2=|\mathbf r'|^2|\mathbf r''|^2-(\mathbf r'\cdot\mathbf r'')^2=8e^{4t}.
$$

The [curvature of a space curve](../../../differential-geometry.md#curvature-of-a-space-curve) is therefore

$$
\boxed{\kappa(t)=\frac{|\mathbf r'\times\mathbf r''|}{|\mathbf r'|^3}
=\frac{e^{-t}}{2\sqrt2},\qquad
\kappa(s)=\frac1{\sqrt2(s+2)}.}
$$

For the forward portion $t\ge0$, this has ordinary nonnegative [arc length](../../../riemannian-geometry.md#arc-length) $s\ge0$. If instead nonnegative distance is measured backwards from $t=0$, put $s_b=2(1-e^t)$ for $t\le0$; that branch has $\kappa=1/[\sqrt2(2-s_b)]$, $0\le s_b<2$. Choosing orientation avoids confusing the two points at the same unoriented distance.

## 4C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

For a continuously differentiable [vector field](../../../calculus.md#vector-field) on all of $\mathbb R^3$, the necessary and sufficient condition for a [conservative vector field](../../../calculus.md#conservative-vector-field) is **$\nabla\times\mathbf F=0$**. Necessity follows from equality of [mixed partial derivatives](../../../calculus.md#mixed-partial-derivative) of a potential; sufficiency uses the $\mathbb R^3$ being a [simply connected space](../../../algebraic-topology.md#simply-connected-space). On a general domain the [topology](../../../topology.md) cannot be omitted.

Here the relevant [mixed partial derivatives](../../../calculus.md#mixed-partial-derivative) are

$$
\partial_yF_z=\partial_zF_y=2ye^z,\quad
\partial_zF_x=\partial_xF_z=-6z^2,\quad
\partial_xF_y=\partial_yF_x=-2x\sin y.
$$

Thus the [curl](../../../calculus.md#curl) vanishes. Integrating the first component in $x$ gives $\Phi=x^2\cos y-2xz^3+A(y,z)$. Matching the second component gives $A_y=3+2ye^z$, hence $A=3y+y^2e^z+B(z)$. Matching the last component forces $B'=0$. A [potential of a conservative vector field](../../../calculus.md#potential-of-a-conservative-vector-field) with the convention $\mathbf F=\nabla\Phi$ is consequently

$$
\boxed{\Phi=x^2\cos y-2xz^3+3y+y^2e^z+C.}
$$

If a physical potential is defined instead through $\mathbf F=-\nabla V$, it is $V=-\Phi$.

## 5D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5d/a">a</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/a/solution">Solution</h4>

↑ **Parent:** [A](#5d/a)

Take $X=G$ and let $g$ act by left multiplication $L_g(x)=gx$. Each $L_g$ is a [permutation](../../../combinatorics.md#permutation), with inverse $L_{g^{-1}}$. Associativity gives $L_gL_h=L_{gh}$, so $g\mapsto L_g$ is a [group homomorphism](../../../group-theory.md#group-homomorphism) into $\operatorname{Sym}(G)$. If $L_g$ is the identity [permutation](../../../combinatorics.md#permutation), evaluating it at the identity element gives $g=1$. Thus

$$
\boxed{G\hookrightarrow\operatorname{Sym}(G),\qquad g\longmapsto L_g.}
$$

This is the [Cayley theorem](../../../group-theory.md#cayley-s-theorem), realized by the [left regular action](../../../group-theory.md#left-regular-action), which is a [faithful group action](../../../group-theory.md#faithful-group-action).

<h3 id="5d/b">b</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/b/solution">Solution</h4>

↑ **Parent:** [B](#5d/b)

Place the cube's vertices at $(\pm1,\pm1,\pm1)$. Its full [symmetry group of a cube](../../../group-theory.md#symmetry-group-of-a-cube) consists of [signed permutation matrices](../../../vector-space.md#signed-permutation-matrix). To see completeness, a cube symmetry fixes its [center of a group](../../../group-theory.md#center-of-a-group) and permutes the six face normals, so it sends coordinate axes to signed coordinate axes; conversely every such matrix preserves the cube. Coordinate [permutations](../../../combinatorics.md#permutation) and sign changes take any edge to any other edge, so this is a [transitive group action](../../../group-theory.md#transitive-group-action) on edges.

Choose the edge $e=\{(1,1,z):-1\le z\le1\}$. A symmetry stabilizing it must preserve its axis direction and its midpoint $(1,1,0)$. It can swap the first two coordinates and independently reverse the third coordinate, but cannot change the signs of the two fixed coordinates. Hence

$$
\boxed{\operatorname{Stab}_H(e)=\langle (x,y,z)\mapsto(y,x,z),\ (x,y,z)\mapsto(x,y,-z)\rangle
\cong C_2\times C_2.}
$$

There are twelve edges and four elements of the [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup). The [orbit-stabiliser theorem](../../../group-theory.md#orbit-stabilizer-theorem) therefore gives **$|H|=48$**, including orientation-reversing symmetries, not just the twenty-four rotations.

The action defines a [group homomorphism](../../../group-theory.md#group-homomorphism) $H\to S_{12}$. If an element fixes every edge as a set, it fixes every vertex, since each vertex is the unique common point of its three incident edges. A cube isometry fixing all vertices is the identity. Thus this is a [faithful group action](../../../group-theory.md#faithful-group-action), and the [cube symmetry action on edges](../../../group-theory.md#cube-symmetry-action-on-edges) embeds $H$ as a [subgroup](../../../group.md#subgroup) with

$$
\boxed{[S_{12}:H]=\frac{12!}{48}=9\,979\,200.}
$$

It is **not a [normal subgroup](../../../group-theory.md#normal-subgroup)**. Central inversion $\mathbf x\mapsto-\mathbf x$ belongs to $H$ and swaps the twelve edges in six opposite pairs. In $S_{12}$, all [permutations](../../../combinatorics.md#permutation) of cycle type $2^6$ are conjugate, and their number is

$$
\frac{12!}{2^6\,6!}=10\,395>48.
$$

If $H$ were a [normal subgroup](../../../group-theory.md#normal-subgroup), it would contain this entire [conjugacy class](../../../group-theory.md#conjugacy-class), impossible for a [group](../../../group.md) of order forty-eight. This avoids relying on a classification of normal [subgroups](../../../group.md#subgroup) of the symmetric [group](../../../group.md).

## 6D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6d/a">a</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/a/i">i</h4>

↑ **Parent:** [A](#6d/a)

<h5 id="6d/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6d/a/i)

For $M=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ in the [special linear group over a finite field](../../../finite-group-theory.md#special-linear-group-over-a-finite-field), define the [Möbius transformation](../../../group-theory.md#mobius-transformation) $M\cdot x=(ax+b)/(cx+d)$ when the denominator is nonzero, and set $M\cdot x=\infty$ when it is zero. At the extra point, $M\cdot\infty=a/c$ for $c\ne0$, and $M\cdot\infty=\infty$ for $c=0$. [Determinant](../../../linear-algebra.md#determinant) one prevents simultaneous zero numerator and denominator.

The [orbit-stabiliser theorem](../../../group-theory.md#orbit-stabilizer-theorem) states $|G\cdot x|=[G:G_x]$, and for a [finite group](../../../group.md#finite-group) $|G|=|G\cdot x||G_x|$. The matrix $\begin{pmatrix}t&-1\\1&0\end{pmatrix}$ sends infinity to any chosen $t\in\mathbb F_p$, so **the orbit of infinity is the whole [projective line](../../../finite-group-theory.md#projective-line)**, of size $p+1$. Its [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) is

$$
\boxed{G_\infty=\left\{\begin{pmatrix}a&b\\0&a^{-1}\end{pmatrix}:a\in\mathbb F_p^*,\ b\in\mathbb F_p\right\},}
$$

which has $p(p-1)$ elements. Consequently

$$
\boxed{|\mathrm{SL}_2(p)|=(p+1)p(p-1)=p(p^2-1).}
$$

The [SL2 action on a finite projective line](../../../finite-group-theory.md#sl2-action-on-a-finite-projective-line) need not be faithful: scalar matrices can fix every projective point. Faithfulness is not needed for this orbit calculation.

<h4 id="6d/a/ii">ii</h4>

↑ **Parent:** [A](#6d/a)

<h5 id="6d/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6d/a/ii)

For $U_t=\begin{pmatrix}1&t\\0&1\end{pmatrix}$ and $D_r=\operatorname{diag}(r,r^{-1})$, direct multiplication gives $D_rU_1D_r^{-1}=U_{r^2}$. In $\mathbb F_{11}$, $5^2=3$ and $5^{-1}=9$, so

$$
\boxed{\begin{pmatrix}5&0\\0&9\end{pmatrix}A\begin{pmatrix}5&0\\0&9\end{pmatrix}^{-1}=B\quad\text{in }\mathrm{SL}_2(11).}
$$

To rule out all conjugators when $p=5$, suppose $PAP^{-1}=B$ and write $P=\begin{pmatrix}r&s\\t&u\end{pmatrix}$. Comparing $PA=BP$ gives $t=0$ and $r=3u$. Its [determinant](../../../linear-algebra.md#determinant) condition is $ru=1$, so $r^2=3$. The nonzero squares modulo five are $1$ and $4$, and therefore no such $P$ exists. **The two matrices are not conjugate in $\mathrm{SL}_2(5)$.** This is the square-class obstruction in [unipotent conjugacy in SL2 over a finite field](../../../finite-group-theory.md#unipotent-conjugacy-in-sl2-over-a-finite-field); checking only diagonal conjugators would not by itself exclude every possible conjugator.

<h3 id="6d/b">b</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/b/solution">Solution</h4>

↑ **Parent:** [B](#6d/b)

Write the matrix as $M(a,b,x)$. Direct multiplication and inversion give

$$
M(a,b,x)M(a',b',x')=M(a+a',b+b',x+x'+ab'),\qquad
M(a,b,x)^{-1}=M(-a,-b,ab-x).
$$

The identity is $M(0,0,0)$ and all determinants are one, so these formulas verify the [subgroup](../../../group.md#subgroup) criterion inside $\mathrm{GL}_3(\mathbb R)$. This is the [real Heisenberg group](../../../lie-algebra.md#heisenberg-group).

The map $M(a,b,x)\mapsto a$ is a surjective [group homomorphism](../../../group-theory.md#group-homomorphism) to the additive [group](../../../group.md) of real numbers; its kernel is exactly $H$. Hence $H$ is normal and the [first isomorphism theorem](../../../group-theory.md#first-isomorphism-theorem) gives

$$
\boxed{G/H\cong(\mathbb R,+).}
$$

Two matrices commute exactly when $ab'=a'b$. Requiring that relation for every $a',b'$ forces $a=b=0$, while $x$ is unrestricted. Therefore

$$
\boxed{Z(G)=\{M(0,0,x):x\in\mathbb R\}.}
$$

Finally $M(a,b,x)\mapsto(a,b)$ is a surjective [group homomorphism](../../../group-theory.md#group-homomorphism) to the additive [group](../../../group.md) $\mathbb R^2$ with precisely this [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism), giving **$G/Z(G)\cong(\mathbb R^2,+)$**. The central coordinate records noncommutativity: the [group commutator](../../../group.md#group-commutator) is $M(0,0,ab'-a'b)$.

## 7D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7d/a">a</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/a/solution">Solution</h4>

↑ **Parent:** [A](#7d/a)

Use the [dihedral group](../../../finite-group-theory.md#dihedral-group) presentation $G=\langle r,s:r^{2n}=s^2=1,\ srs=r^{-1}\rangle$. Every element is $r^j$ or $sr^j$. A nonidentity rotation has order two only when its exponent is $n$, while $(sr^j)^2=1$ for every $j$. Thus the complete list is

$$
\boxed{r^n,\quad sr^j\ (0\le j<2n).}
$$

The half-turn $r^n$ is central, so its [conjugacy class](../../../group-theory.md#conjugacy-class) is the singleton $\{r^n\}$ and its [normal closure](../../../group-theory.md#normal-closure) is **$\{1,r^n\}$**.

For reflections, $r^k(sr^j)r^{-k}=sr^{j-2k}$ and $s(sr^j)s^{-1}=sr^{-j}$. Hence the [conjugacy class](../../../group-theory.md#conjugacy-class) is exactly the $n$ reflections whose exponents have the same parity as $j$:

$$
\boxed{\{sr^{j+2k}:0\le k<n\}.}
$$

The [subgroup](../../../group.md#subgroup) generated by this class contains $r^2$, as the product of two consecutive listed reflections, and contains $sr^j$. Conversely those two generators contain every listed reflection. Their [subgroup](../../../group.md#subgroup) is invariant under [conjugation](../../../group-theory.md#conjugation) by both $r$ and $s$, so the smallest [normal subgroup](../../../group-theory.md#normal-subgroup) containing $sr^j$ is

$$
\boxed{\langle r^2,sr^j\rangle
=\{r^{2k},sr^{j+2k}:0\le k<n\},}
$$

of order $2n$ and index two. This [involutions in an even dihedral group](../../../finite-group-theory.md#involutions-in-an-even-dihedral-group) classification distinguishes the two reflection classes from the central half-turn.

<h3 id="7d/b">b</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/b/i">i</h4>

↑ **Parent:** [B](#7d/b)

<h5 id="7d/b/i/solution">Solution</h5>

↑ **Parent:** [I](#7d/b/i)

If one [subgroup](../../../group.md#subgroup) contains the other, their union is the larger [subgroup](../../../group.md#subgroup). Conversely, if neither contains the other, choose $h\in H\setminus K$ and $k\in K\setminus H$. If the union were a [subgroup](../../../group.md#subgroup) it would contain $hk$. If $hk\in H$, then $k=h^{-1}(hk)\in H$, a contradiction; if $hk\in K$, then $h=(hk)k^{-1}\in K$, again a contradiction. Thus

$$
\boxed{H\cup K\text{ is a subgroup}\ \Longleftrightarrow\ H\subseteq K\text{ or }K\subseteq H.}
$$

The [union of two subgroups](../../../group.md#union-of-two-subgroups) cannot generally be treated like their generated [subgroup](../../../group.md#subgroup).

<h4 id="7d/b/ii">ii</h4>

↑ **Parent:** [B](#7d/b)

<h5 id="7d/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7d/b/ii)

Choose $x\notin H$, possible because $H$ is proper. For any $h\in H$, the element $xh$ is also outside $H$, since otherwise multiplying by $h^{-1}$ would put $x$ inside $H$. Thus both $x$ and $xh$ belong to $K=\langle G\setminus H\rangle$, and $h=x^{-1}(xh)\in K$. So $K$ contains $H$ as well as its entire complement, proving

$$
\boxed{\langle G\setminus H\rangle=G.}
$$

The [complement of a proper subgroup generates the group](../../../group.md#complement-of-a-proper-subgroup-generates-the-group) argument does not actually require finiteness.

## 8D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8d/solution">Solution</h3>

↑ **Parent:** [8D](#8d)

For a nontrivial [finite p-group](../../../finite-group-theory.md#finite-p-group) $G$ of order $p^m$ with $m\ge1$, partition into [conjugacy classes](../../../group-theory.md#conjugacy-class). A noncentral class has size $[G:C_G(x)]$, a positive power of $p$ larger than one by [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem). The [class equation](../../../group-theory.md#class-equation) therefore says

$$
|G|=|Z(G)|+\sum_{\text{noncentral classes}}[G:C_G(x)],\qquad |Z(G)|\equiv0\pmod p.
$$

The [center of a group](../../../group-theory.md#center-of-a-group) contains the identity, so **$|Z(G)|\ge p$**, proving its nontriviality. The positive-exponent qualification matters: the one-element [group](../../../group.md) has no nonidentity central element.

If $|G|=p^2$, its [center of a group](../../../group-theory.md#center-of-a-group) has order $p$ or $p^2$. In the first case, the [quotient group](../../../group-theory.md#quotient-group) $G/Z(G)$ has prime order and is cyclic. Whenever a central [quotient group](../../../group-theory.md#quotient-group) is cyclic, writing all elements as $g^iz$ with $z$ central shows that they commute: $(g^iz)(g^jw)=g^{i+j}zw=(g^jw)(g^iz)$. Thus that case would already make $G$ [Abelian](../../../group.md#abelian-group) and its [center of a group](../../../group-theory.md#center-of-a-group) all of $G$, a contradiction. Hence **every [group](../../../group.md) of order $p^2$ is [Abelian](../../../group.md#abelian-group)**.

If there is an element of order $p^2$, it is a [generator of a group](../../../group.md#generator-of-a-group) for $G$, giving $C_{p^2}$. Otherwise every nonidentity element has order $p$. Pick $a\ne1$ and $b\notin\langle a\rangle$. Their [cyclic subgroups](../../../group.md#cyclic-subgroup) have trivial intersection, and they commute; the $p^2$ distinct products $a^ib^j$ exhaust $G$. Hence the [classification of groups of order p squared](../../../finite-group-theory.md#classification-of-groups-of-order-p-squared) is

$$
\boxed{G\cong C_{p^2}\quad\text{or}\quad G\cong C_p\times C_p.}
$$

Both [groups](../../../group.md) exist and are nonisomorphic, since only the first has an element of order $p^2$.

## 9C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9c/solution">Solution</h3>

↑ **Parent:** [9C](#9c)

For a smooth one-to-one coordinate transformation with nonsingular derivative, the [Jacobian determinant](../../../calculus.md#jacobian-determinant) is

$$
\boxed{J=\det\begin{pmatrix}x_u&x_v&x_w\\y_u&y_v&y_w\\z_u&z_v&z_w\end{pmatrix}.}
$$

Locally a small coordinate box maps, to first order, to a parallelepiped whose volume is the absolute [determinant](../../../linear-algebra.md#determinant) of the derivative times the original volume. Summing these local volume approximations gives the [change of variables formula](../../../calculus.md#change-of-variables-formula), with $|J|$ accounting for either orientation. The usual regularity and nonsingularity hypotheses are part of this substitution theorem.

The region is the upper half of the spherical shell between radii two and three, including its annular flat boundary in the equatorial plane. Use [spherical coordinates](../../../calculus.md#spherical-coordinate-system) $x=r\sin\theta\cos\phi$, $y=r\sin\theta\sin\phi$, $z=r\cos\theta$ with $2\le r\le3$, $0\le\theta\le\pi/2$, $0\le\phi<2\pi$. Their [Jacobian determinant](../../../calculus.md#jacobian-determinant) is $r^2\sin\theta$; the polar axis and azimuth seam have measure zero, so do not obstruct this integration.

<a id="9c/image-upper-hemispherical-shell-between-radii-two-and-three-with-a-meridian-cross-section-and-a-cutaway-view"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-3-hemispherical-shell.png)

**[Figure 1](#9c/image-upper-hemispherical-shell-between-radii-two-and-three-with-a-meridian-cross-section-and-a-cutaway-view). Upper hemispherical shell between radii two and three, with a meridian cross-section and a cutaway view**.

The integrand is $x^2+y^2=r^2\sin^2\theta$. Consequently

$$
\boxed{\int_D(x^2+y^2)\,dV
=\int_2^3r^4\,dr\int_0^{\pi/2}\sin^3\theta\,d\theta\int_0^{2\pi}d\phi
=\frac{211}{5}\frac23(2\pi)=\frac{844\pi}{15}.}
$$

## 10C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10c/solution">Solution</h3>

↑ **Parent:** [10C](#10c)

Take the [normal vector](../../../differential-geometry.md#normal-vector) outward from the cylinder-and-cone solid. The surface consists of the cylindrical side and conical roof, with no bottom disk; this convention fixes the otherwise unspecified [orientation of a surface](../../../differential-geometry.md#orientation-of-a-surface). The boundary is the radius-two circle at $z=-2$. Reversing every [normal vector](../../../differential-geometry.md#normal-vector) reverses the final sign.

<a id="10c/image-outward-oriented-cylindrical-side-and-conical-roof-with-the-open-bottom-circle-as-the-sole-boundary"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-3-cylinder-cone.png)

**[Figure 2](#10c/image-outward-oriented-cylindrical-side-and-conical-roof-with-the-open-bottom-circle-as-the-sole-boundary). Outward-oriented cylindrical side and conical roof, with the open bottom circle as the sole boundary**.

For $\mathbf F=(yz^2,0,0)$, its [curl](../../../calculus.md#curl) is $(0,2yz,-z^2)$. For the cylindrical [parametrized surface](../../../calculus.md#parametrized-surface), use $\mathbf r_c=(2\cos\theta,2\sin\theta,z)$, with $-2\le z\le2$, and use $\mathbf r_{c,\theta}\times\mathbf r_{c,z}=(2\cos\theta,2\sin\theta,0)$ as the outward area vector. Its flux is

$$
I_c=\int_{-2}^{2}\int_0^{2\pi}8z\sin^2\theta\,d\theta\,dz=0.
$$

For the cone, let $q=4-z$, $2\le z\le4$ and $\mathbf r_k=(q\cos\theta,q\sin\theta,z)$. Its outward area vector is $\mathbf r_{k,\theta}\times\mathbf r_{k,z}=(q\cos\theta,q\sin\theta,q)$. Thus

$$
\begin{aligned}
I_k&=\int_2^4\int_0^{2\pi}(2q^2z\sin^2\theta-qz^2)\,d\theta\,dz\\
&=2\pi\int_2^4(16z-12z^2+2z^3)\,dz=-16\pi.
\end{aligned}
$$

The total [surface integral](../../../calculus.md#surface-integral) is therefore **$-16\pi$ with the outward convention**, or $+16\pi$ for the opposite convention.

For [Stokes theorem](../../../calculus.md#stokes-theorem), the induced bottom-circle orientation is counterclockwise as viewed from above, opposite to the orientation of an outward bottom cap. Use $\mathbf r=(2\cos\theta,2\sin\theta,-2)$ with increasing $\theta$. Then

$$
\boxed{\oint_{\partial S}\mathbf F\cdot d\mathbf r
=\int_0^{2\pi}(8\sin\theta)(-2\sin\theta)\,d\theta=-16\pi,}
$$

agreeing with the two parametrized fluxes. The seam at $z=2$ is internal and cancels between the two pieces; the cone tip does not supply another boundary curve.

## 11C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11c/solution">Solution</h3>

↑ **Parent:** [11C](#11c)

For a Cartesian [change of basis](../../../linear-algebra.md#change-of-basis) represented by an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) $Q$, [vectors](../../../vector-space.md#vector) transform as $E'_i=Q_{ia}E_a$ and $B'_i=Q_{ia}B_a$. Their squared norms are invariant and $Q_{ia}Q_{jb}\delta_{ab}=\delta_{ij}$. Substitution into the given expression therefore gives

$$
\boxed{T'_{ij}=Q_{ia}Q_{jb}T_{ab},}
$$

the transformation law of a [Cartesian second-rank tensor](../../../linear-algebra.md#cartesian-second-rank-tensor). The [magnetic field](../../../electromagnetism.md#magnetic-field)'s extra axial sign under an improper physical reflection, if included, appears twice and cancels in its quadratic contribution.

Write the [Maxwell stress tensor](../../../electromagnetism.md#maxwell-stress-tensor) as $T=\mathbf E\mathbf E+\mathbf B\mathbf B-\tfrac12(E^2+B^2)I$. Its [divergence](../../../calculus.md#divergence) is

$$
\mathbf M=(\mathbf E\cdot\nabla)\mathbf E+\mathbf E\nabla\cdot\mathbf E
+(\mathbf B\cdot\nabla)\mathbf B+\mathbf B\nabla\cdot\mathbf B
-\tfrac12\nabla(E^2+B^2).
$$

The identity $(\mathbf A\cdot\nabla)\mathbf A-\tfrac12\nabla A^2=-\mathbf A\times(\nabla\times\mathbf A)$ follows by contracting two [Levi-Civita symbols](../../../calculus.md#levi-civita-symbol), or directly by differentiating components. Using [Maxwell's equations](../../../electromagnetism.md#maxwell-equations) consequently yields

$$
\begin{aligned}
\mathbf M
&=\rho\mathbf E-\mathbf E\times(\nabla\times\mathbf E)-\mathbf B\times(\nabla\times\mathbf B)\\
&=\rho\mathbf E+\mathbf E\times\mathbf B_t-\mathbf B\times(\mathbf J+\mathbf E_t)\\
&=\rho\mathbf E+\mathbf J\times\mathbf B+\partial_t(\mathbf E\times\mathbf B).
\end{aligned}
$$

Hence the [local conservation of electromagnetic momentum](../../../electromagnetism.md#local-conservation-of-electromagnetic-momentum) is

$$
\boxed{\partial_t(\mathbf E\times\mathbf B)=\mathbf M-\rho\mathbf E-\mathbf J\times\mathbf B,
\qquad M_i=\partial_jT_{ij}.}
$$

The two subtracted terms are the [Lorentz force density](../../../electromagnetism.md#lorentz-force-density), while $\mathbf E\times\mathbf B$ is the [electromagnetic momentum density](../../../electromagnetism.md#electromagnetic-momentum-density) in the units used here.

## 12C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12c/a">a</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/a/solution">Solution</h4>

↑ **Parent:** [A](#12c/a)

Use the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) and summation over repeated indices. Contracting the two symbols gives

$$
\begin{aligned}
[\nabla\times(\mathbf F\times\mathbf G)]_i
&=\epsilon_{ijk}\partial_j(\epsilon_{klm}F_lG_m)\\
&=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})\partial_j(F_lG_m)\\
&=\partial_j(F_iG_j-F_jG_i)\\
&=F_i\partial_jG_j-G_i\partial_jF_j+G_j\partial_jF_i-F_j\partial_jG_i.
\end{aligned}
$$

Thus the [curl of a cross product](../../../calculus.md#curl-of-a-cross-product) is

$$
\boxed{\nabla\times(\mathbf F\times\mathbf G)
=\mathbf F\nabla\cdot\mathbf G-\mathbf G\nabla\cdot\mathbf F
+(\mathbf G\cdot\nabla)\mathbf F-(\mathbf F\cdot\nabla)\mathbf G.}
$$

<h3 id="12c/b">b</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/b/solution">Solution</h4>

↑ **Parent:** [B](#12c/b)

Under the usual bounded-domain hypotheses, with piecewise smooth boundary and a sufficiently smooth [vector field](../../../calculus.md#vector-field), the [divergence theorem](../../../calculus.md#divergence-theorem) states

$$
\boxed{\int_\Omega\nabla\cdot\mathbf F\,dV=\int_{\partial\Omega}\mathbf F\cdot\mathbf n\,dS,}
$$

where $\mathbf n$ is outward. Apply it to $g\mathbf F$ and use the [product rule](../../../calculus.md#product-rule) $\nabla\cdot(g\mathbf F)=\mathbf F\cdot\nabla g+g\nabla\cdot\mathbf F$ to obtain

$$
\boxed{\int_\Omega(\mathbf F\cdot\nabla g+g\nabla\cdot\mathbf F)\,dV
=\int_{\partial\Omega}g\mathbf F\cdot\mathbf n\,dS.}
$$

For uniqueness, let $w=u_1-u_2$ for two [classical solutions](../../../partial-differential-equation.md#classical-solution) with the same [Dirichlet boundary data](../../../differential-equation.md#dirichlet-boundary-data). Then $\Delta w=0$ and $w=0$ on the boundary. Taking $\mathbf F=\nabla w$, $g=w$ gives [Green's first identity](../../../partial-differential-equation.md#green-s-first-identity) in the form

$$
\int_\Omega|\nabla w|^2\,dV
=\int_{\partial\Omega}w\partial_nw\,dS-\int_\Omega w\Delta w\,dV=0.
$$

The continuous nonnegative integrand must vanish, so $w$ is constant on each connected component. The zero boundary data make every such constant zero. Thus **the solution of the [Dirichlet problem](../../../analysis.md#dirichlet-problem) for the [Laplace equation](../../../partial-differential-equation.md#laplace-equation) is unique, if it exists**. This establishes [Uniqueness of the Dirichlet problem](../../../analysis.md#uniqueness-of-the-dirichlet-problem); existence is assumed. Boundedness, or suitable conditions at infinity, is needed: on an unbounded half-space the [harmonic function](../../../partial-differential-equation.md#harmonic-function) $w=z$ has zero boundary values but is not identically zero.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
