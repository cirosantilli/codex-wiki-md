# Paper 3

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2014/PaperIA_3.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2014/PaperIA_3.pdf)

**Table of contents**

- [1D](#1d)
  - [Solution](#1d/solution)
- [2D](#2d)
  - [Solution](#2d/solution)
- [3A](#3a)
  - [a](#3a/a)
    - [Solution](#3a/a/solution)
  - [b](#3a/b)
    - [i](#3a/b/i)
      - [Solution](#3a/b/i/solution)
    - [ii](#3a/b/ii)
      - [Solution](#3a/b/ii/solution)
  - [c](#3a/c)
    - [Solution](#3a/c/solution)
- [4A](#4a)
  - [a](#4a/a)
    - [Solution](#4a/a/solution)
  - [b](#4a/b)
    - [Solution](#4a/b/solution)
  - [c](#4a/c)
    - [Solution](#4a/c/solution)
- [5D](#5d)
  - [i](#5d/i)
    - [Solution](#5d/i/solution)
  - [ii](#5d/ii)
    - [Solution](#5d/ii/solution)
- [6D](#6d)
  - [i](#6d/i)
    - [Solution](#6d/i/solution)
  - [ii](#6d/ii)
    - [Solution](#6d/ii/solution)
  - [iii](#6d/iii)
    - [Solution](#6d/iii/solution)
- [7D](#7d)
  - [i](#7d/i)
    - [Solution](#7d/i/solution)
  - [ii](#7d/ii)
    - [Solution](#7d/ii/solution)
- [8D](#8d)
  - [a](#8d/a)
    - [Solution](#8d/a/solution)
  - [b](#8d/b)
    - [i](#8d/b/i)
      - [Solution](#8d/b/i/solution)
    - [ii](#8d/b/ii)
      - [Solution](#8d/b/ii/solution)
    - [iii](#8d/b/iii)
      - [Solution](#8d/b/iii/solution)
- [9A](#9a)
  - [a](#9a/a)
    - [Solution](#9a/a/solution)
  - [b](#9a/b)
    - [Solution](#9a/b/solution)
  - [c](#9a/c)
    - [Solution](#9a/c/solution)
  - [d](#9a/d)
    - [Solution](#9a/d/solution)
- [10A](#10a)
  - [a](#10a/a)
    - [Solution](#10a/a/solution)
  - [b](#10a/b)
    - [Solution](#10a/b/solution)
  - [c](#10a/c)
    - [Solution](#10a/c/solution)
- [11A](#11a)
  - [i](#11a/i)
    - [Solution](#11a/i/solution)
  - [ii](#11a/ii)
    - [Solution](#11a/ii/solution)
  - [iii](#11a/iii)
    - [Solution](#11a/iii/solution)
  - [iv](#11a/iv)
    - [Solution](#11a/iv/solution)
- [12A](#12a)
  - [a](#12a/a)
    - [Solution](#12a/a/solution)
  - [b](#12a/b)
    - [i](#12a/b/i)
      - [Solution](#12a/b/i/solution)
    - [ii](#12a/b/ii)
      - [Solution](#12a/b/ii/solution)
  - [c](#12a/c)
    - [i](#12a/c/i)
      - [Solution](#12a/c/i/solution)
    - [ii](#12a/c/ii)
      - [Solution](#12a/c/ii/solution)

## 1D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1d/solution">Solution</h3>

↑ **Parent:** [1D](#1d)

Choose a positive common denominator $d$ so that $x=a/d$ and $y=b/d$ with nonzero [integers](../../../number-theory.md#integer) $a,b$. Put $h=\gcd(a,b)>0$. Every element of the generated [subgroup](../../../group.md#subgroup) has the form $(ma+nb)/d$, so it lies in $(h/d)\mathbb Z$. Conversely, [Bezout identity](../../../algebra.md#bezout-identity) gives [integers](../../../number-theory.md#integer) $u,v$ with $ua+vb=h$, so $h/d$ belongs to the generated [subgroup](../../../group.md#subgroup). Consequently

$$
\boxed{N=(h/d)\mathbb Z\cong\mathbb Z,\qquad k\longmapsto kh/d.}
$$

This map is a bijective additive [group homomorphism](../../../group-theory.md#group-homomorphism). It is the two-generator instance of a [finitely generated subgroup of the rational additive group](../../../group.md#finitely-generated-subgroup-of-the-rational-additive-group) being an [infinite cyclic group](../../../group.md#infinite-cyclic-group).

For the real example, take $x=1$ and $y=\sqrt2$. The [group homomorphism](../../../group-theory.md#group-homomorphism) $(m,n)\mapsto m+n\sqrt2$ from $\mathbb Z^2$ onto the generated [subgroup](../../../group.md#subgroup) is injective because $\sqrt2$ is an [irrational number](../../../algebra.md#irrational-number). Thus this [subgroup](../../../group.md#subgroup) is isomorphic to $\mathbb Z^2$. More directly, if a single real number $t$ generated it, then $1=at$ and $\sqrt2=bt$ for [integers](../../../number-theory.md#integer) $a\ne0,b$, giving $\sqrt2=b/a$, a contradiction. **The choice $1,\sqrt2$ generates a noncyclic additive [subgroup](../../../group.md#subgroup).**

## 2D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2d/solution">Solution</h3>

↑ **Parent:** [2D](#2d)

For a [finite group](../../../group.md#finite-group), the [conjugacy classes](../../../group-theory.md#conjugacy-class) partition the [group](../../../group.md), and a class is a singleton exactly when its element belongs to the [centre of a group](../../../group-theory.md#center-of-a-group). Since the centre is trivial, the [class equation](../../../group-theory.md#class-equation) becomes

$$
|G|=1+\sum_j |\mathcal C_j|,
$$

where the $\mathcal C_j$ are all the nonidentity [conjugacy classes](../../../group-theory.md#conjugacy-class). If the [prime number](../../../number-theory.md#prime-number) $p$ divided every $|\mathcal C_j|$, reduction modulo $p$ would give $0=1$, because $p\mid |G|$. Therefore at least one of these class sizes is not divisible by $p$. Primality now gives

$$
\boxed{\gcd(|\mathcal C_j|,p)=1.}
$$

Its size is greater than one because the centre is trivial. This proves the [prime-to-p conjugacy class lemma](../../../group-theory.md#prime-to-p-conjugacy-class-lemma).

**The conclusion requires $p$ to be prime.** The printed question does not explicitly impose this hypothesis. If arbitrary composite divisors are allowed, take the [symmetric group](../../../finite-group-theory.md#symmetric-group) $S_3$ and $p=6$: its centre is trivial, its two nonidentity [conjugacy classes](../../../group-theory.md#conjugacy-class) have sizes $3$ and $2$, and neither is [coprime](../../../number-theory.md#coprime-integers) to $6$. Thus the argument proves the intended prime case and also identifies why the unrestricted literal reading is false.

## 3A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3a/a">a</h3>

↑ **Parent:** [3A](#3a)

<h4 id="3a/a/solution">Solution</h4>

↑ **Parent:** [A](#3a/a)

Away from the origin, differentiate $r^2=x_jx_j$ using [Einstein notation](../../../linear-algebra.md#einstein-notation):

$$
2r\,\partial_i r=2x_i.
$$

Hence

$$
\boxed{\partial_i r=x_i/r,\qquad \nabla r=\mathbf x/r.}
$$

This [gradient](../../../calculus.md#gradient) is the radial unit [vector](../../../vector-space.md#vector). Division by $r$ is legitimate on the punctured domain; the distance [function](../../../function.md) is not differentiable at the origin.

<h3 id="3a/b">b</h3>

↑ **Parent:** [3A](#3a)

<h4 id="3a/b/i">i</h4>

↑ **Parent:** [B](#3a/b)

<h5 id="3a/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3a/b/i)

Apply the [product rule](../../../calculus.md#product-rule) and the preceding [gradient](../../../calculus.md#gradient) formula to the [vector field](../../../calculus.md#vector-field) $F_i=f(r)x_i$. Summing over the repeated index gives

$$
\partial_iF_i=f'(r)\frac{x_i x_i}{r}+f(r)\delta_{ii}
=rf'(r)+nf(r).
$$

Here $\delta_{ii}=n$ for the [Kronecker delta](../../../linear-algebra.md#kronecker-delta). Thus the [divergence and curl of a radial vector field](../../../calculus.md#divergence-and-curl-of-a-radial-vector-field) give, in any dimension,

$$
\boxed{\nabla\cdot[f(r)\mathbf x]=rf'(r)+nf(r).}
$$

<h4 id="3a/b/ii">ii</h4>

↑ **Parent:** [B](#3a/b)

<h5 id="3a/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3a/b/ii)

In three dimensions the [curl](../../../calculus.md#curl) can be written with the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol):

$$
(\nabla\times\mathbf F)_i
=\epsilon_{ijk}\partial_j(f(r)x_k)
=\epsilon_{ijk}\left(\frac{f'(r)}r x_jx_k+f(r)\delta_{jk}\right)=0.
$$

Both terms contract an antisymmetric array with a symmetric one, and therefore vanish. **Every differentiable radial field of this form has zero [curl](../../../calculus.md#curl) away from the origin.** This is the three-dimensional part of the [divergence and curl of a radial vector field](../../../calculus.md#divergence-and-curl-of-a-radial-vector-field).

<h3 id="3a/c">c</h3>

↑ **Parent:** [3A](#3a)

<h4 id="3a/c/solution">Solution</h4>

↑ **Parent:** [C](#3a/c)

The [divergence](../../../calculus.md#divergence) formula reduces the problem to the [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) $rf'+nf=0$ on $r>0$. Multiplication by $r^{n-1}$ makes it an exact derivative:

$$
\frac{d}{dr}(r^nf(r))=r^{n-1}(rf'(r)+nf(r))=0.
$$

Since the interval $r>0$ is connected, $r^nf(r)$ is a single constant $C$. Conversely, substituting $f=Cr^{-n}$ into the [divergence](../../../calculus.md#divergence) formula gives zero. Thus

$$
\boxed{\mathbf F(\mathbf x)=C\,\frac{\mathbf x}{|\mathbf x|^n}\quad(\mathbf x\ne0).}
$$

This proves both existence and uniqueness up to the constant within the specified radial class. For $n=1$, the two punctured half-lines still share this same constant because the stipulated coefficient is one [function](../../../function.md) of $r=|x|$.

## 4A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4a/a">a</h3>

↑ **Parent:** [4A](#4a)

<h4 id="4a/a/solution">Solution</h4>

↑ **Parent:** [A](#4a/a)

Parametrize the smooth path by $\gamma:[0,1]\to G$. The [chain rule](../../../calculus.md#chain-rule) turns the [line integral](../../../calculus.md#line-integral) of the [gradient](../../../calculus.md#gradient) into a one-variable derivative:

$$
\int_\gamma\mathbf F\cdot d\mathbf x
=\int_0^1\nabla\phi(\gamma(t))\cdot\gamma'(t)\,dt
=\int_0^1\frac{d}{dt}\phi(\gamma(t))\,dt
=\boxed{\phi(\mathbf b)-\phi(\mathbf a)}.
$$

This is the [fundamental theorem for line integrals](../../../calculus.md#fundamental-theorem-for-line-integrals); in particular the integral has [path independence](../../../calculus.md#path-independence).

For a twice continuously differentiable [potential of a conservative vector field](../../../calculus.md#potential-of-a-conservative-vector-field), the [curl](../../../calculus.md#curl) of its [gradient](../../../calculus.md#gradient) vanishes because mixed [partial derivatives](../../../calculus.md#partial-derivative) commute:

$$
(\nabla\times\nabla\phi)_i=\epsilon_{ijk}\partial_j\partial_k\phi=0.
$$

**A smooth [gradient](../../../calculus.md#gradient) field is necessarily [curl](../../../calculus.md#curl)-free.**

<h3 id="4a/b">b</h3>

↑ **Parent:** [4A](#4a)

<h4 id="4a/b/solution">Solution</h4>

↑ **Parent:** [B](#4a/b)

A sufficient condition is that $G$ be an open [simply connected](../../../algebraic-topology.md#simply-connected-space) domain, with $\mathbf F$ continuously differentiable. Under this condition a [curl-free vector field](../../../calculus.md#irrotational-vector-field) has a global [potential of a conservative vector field](../../../calculus.md#potential-of-a-conservative-vector-field) and hence [path independence](../../../calculus.md#path-independence) by the [fundamental theorem for line integrals](../../../calculus.md#fundamental-theorem-for-line-integrals). One way to see the global step is to deform the closed loop formed by two paths into a point inside $G$: the integral is unchanged during the deformation because the [curl](../../../calculus.md#curl) is zero, as expressed by [Stokes theorem](../../../calculus.md#stokes-theorem). Therefore **simple connectivity is a sufficient domain hypothesis**. It is not a claim that every particular [curl](../../../calculus.md#curl)-free field needs such a domain; a given field can have a global potential on a domain with holes.

<h3 id="4a/c">c</h3>

↑ **Parent:** [4A](#4a)

<h4 id="4a/c/solution">Solution</h4>

↑ **Parent:** [C](#4a/c)

Use $\gamma(t)=(\cos t,\sin t,0)$ for $0\le t\le2\pi$. On this path $\mathbf F=(-\sin t,\cos t,0)=\gamma'(t)$, so its [line integral](../../../calculus.md#line-integral) is

$$
\boxed{\oint_\gamma\mathbf F\cdot d\mathbf x=\int_0^{2\pi}1\,dt=2\pi.}
$$

The first two components of the [curl](../../../calculus.md#curl) vanish because the field is independent of $z$ and has zero third component. Writing $q=x^2+y^2$, its third [curl](../../../calculus.md#curl) component is

$$
\partial_x(x/q)-\partial_y(-y/q)
=\frac{y^2-x^2}{q^2}-\frac{y^2-x^2}{q^2}=0.
$$

Thus this [azimuthal inverse-radius vector field](../../../calculus.md#azimuthal-inverse-radius-vector-field) is a [curl-free vector field](../../../calculus.md#irrotational-vector-field) on $G=\mathbb R^3\setminus\{(0,0,z):z\in\mathbb R\}$, but its [line integral](../../../calculus.md#line-integral) is not path independent. This domain is not [simply connected](../../../algebraic-topology.md#simply-connected-space): the circle links the removed axis. A spanning disk through the axis is inadmissible for [Stokes theorem](../../../calculus.md#stokes-theorem), since the [vector field](../../../calculus.md#vector-field) is undefined there. **Zero [curl](../../../calculus.md#curl) alone does not force global path independence.**

## 5D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5d/i">i</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/i/solution">Solution</h4>

↑ **Parent:** [I](#5d/i)

Conjugation in the [symmetric group](../../../finite-group-theory.md#symmetric-group) sends $(1\ 2)$ to $(\sigma(1)\ \sigma(2))$. Hence $\sigma$ commutes with $g$ exactly when it preserves the unordered pair $\{1,2\}$. It can independently swap that pair and arbitrarily permute the remaining points. Therefore the [centraliser of a transposition](../../../group-theory.md#centraliser-of-a-transposition) is

$$
\boxed{C_{S_n}(g)=\langle(1\ 2)\rangle\times S_{\{3,\ldots,n\}},\qquad |C_{S_n}(g)|=2(n-2)!.}
$$

Let $m=n/2$. The [orbits of a group action](../../../group-theory.md#orbit-of-a-group-action) generated by $h$ are its $m$ two-point blocks. Any [centraliser](../../../group-theory.md#centralizer) element must permute those blocks, and can choose independently whether to swap the two points in each image block. Conversely every such choice commutes with $h$, since it preserves the partner relation. This [centraliser of a fixed-point-free involution](../../../group-theory.md#centraliser-of-a-fixed-point-free-involution) is the [permutation wreath product](../../../group-theory.md#permutation-wreath-product) $C_2\wr S_m$, with

$$
\boxed{|C_{S_n}(h)|=2^m m! = 2^{n/2}(n/2)!.}
$$

<h3 id="5d/ii">ii</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5d/ii)

Place the [cube](../../../geometry-and-topology.md#cube) at the origin with face normals $\pm e_1,\pm e_2,\pm e_3$, and label opposite faces by $(1,2),(3,4),(5,6)$. Every cube symmetry is a [signed permutation matrix](../../../vector-space.md#signed-permutation-matrix): there are $2^3\,3!=48$ choices. Its [group action](../../../group-theory.md#group-action) on faces is faithful because fixing all faces fixes all their normal directions. Central inversion $-I$ exchanges every opposite pair and therefore acts as $h$. Since $-I$ commutes with every linear cube symmetry, the face-action image lies in $C_{S_6}(h)$. The preceding count gives $|C_{S_6}(h)|=48$, so the faithful face action is onto this [centraliser](../../../group-theory.md#centralizer):

$$
\boxed{G\cong C_{S_6}(h).}
$$

For the remaining isomorphism, let $R$ be the [rotational symmetry group of a cube](../../../group-theory.md#rotational-symmetry-group-of-a-cube). Half the signed permutation [matrices](../../../vector-space.md#matrix) have [determinant](../../../linear-algebra.md#determinant) $1$, so $|R|=24$. Central inversion has [determinant](../../../linear-algebra.md#determinant) $-1$, and every orientation-reversing symmetry is $(-I)r$ for a unique $r\in R$. Since $-I$ is central and $R\cap\{I,-I\}=\{I\}$, multiplication gives a [direct product of groups](../../../group-theory.md#direct-product-of-groups):

$$
G\cong C_2\times R.
$$

The [group action](../../../group-theory.md#group-action) of $R$ on the four body diagonals is faithful. To prove this, choose direction [vectors](../../../vector-space.md#vector) $(1,1,1),(1,-1,-1),(-1,1,-1),(-1,-1,1)$. They span $\mathbb R^3$, and their only linear relation is that their sum is zero. A rotation fixing all four diagonal lines sends each listed [vector](../../../vector-space.md#vector) to itself or its negative. Applying the relation forces all four signs to agree. The all-negative choice is $-I$, which is not in $R$, so the rotation is the identity. Thus $R$ embeds in $S_4$; both have order $24$, giving $R\cong S_4$. Finally $C_{S_6}(g)\cong C_2\times S_4$ from part (i). Consequently

$$
\boxed{G\cong C_2\times S_4\cong C_{S_6}(g).}
$$

The [direct-product decomposition of the cube symmetry group](../../../group-theory.md#direct-product-decomposition-of-the-cube-symmetry-group) supplies the second isomorphism, while the first comes from the specified face action.

## 6D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6d/i">i</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/i/solution">Solution</h4>

↑ **Parent:** [I](#6d/i)

We first prove the needed instance of [Cauchy theorem for groups](../../../finite-group-theory.md#cauchy-theorem-for-groups), rather than invoke it. Let a [prime number](../../../number-theory.md#prime-number) $q$ divide $|G|$ and consider the set

$$
\mathcal T=\{(g_1,\ldots,g_q):g_1\cdots g_q=1\}.
$$

There are $|G|^{q-1}$ such tuples: choose the first $q-1$ entries freely, and the last is forced. Cyclic rotation preserves this set, because moving the first entry to the end conjugates the product, which remains $1$. Each rotation [orbit of a group action](../../../group-theory.md#orbit-of-a-group-action) has either one or $q$ elements. Indeed a nontrivial shift fixing a tuple generates all shifts, since its step has an inverse modulo the prime $q$. The fixed tuples are precisely $(g,\ldots,g)$ with $g^q=1$.

Counting nonfixed orbits in multiples of $q$, and using $q\mid |G|^{q-1}$, shows that the number of solutions of $g^q=1$ is divisible by $q$. The identity supplies one solution, so there is a nonidentity solution. If its [order of a group element](../../../group-theory.md#order-of-a-group-element) is $d$, divide $q$ by $d$: the remainder would give a smaller positive exponent producing the identity, so $d\mid q$. Hence $d=q$. This proves the required prime-order existence result by the [cyclic-tuple proof of Cauchy theorem](../../../finite-group-theory.md#cyclic-tuple-proof-of-cauchy-theorem).

Our hypothesis says that this nonidentity element has order $p$, so $q=p$. Every prime divisor of $|G|$ is therefore $p$, which gives

$$
\boxed{|G|=p^n\quad\text{for some }n\ge0.}
$$

Thus a [finite group of prime exponent has prime-power order](../../../group-theory.md#finite-group-of-prime-exponent-has-prime-power-order). The case $n=0$ includes the trivial [group](../../../group.md). No [group](../../../group.md)-theoretic counting theorem was assumed in the tuple argument.

<h3 id="6d/ii">ii</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6d/ii)

If a nonidentity power $x^j$ belongs to $H$, reduce $j$ modulo $p$ so that $1\le j<p$. There is an integer $a$ with $aj\equiv1\pmod p$, and therefore $(x^j)^a=x\in H$, a contradiction. Thus

$$
\boxed{\langle x\rangle\cap H=\{1\}.}
$$

Now suppose that $G$ is abelian and finite. Start with $H_0=\{1\}$, and whenever $H_k\ne G$, choose $x_{k+1}\notin H_k$. The multiplication map

$$
H_k\times\langle x_{k+1}\rangle\longrightarrow H_{k+1}=H_k\langle x_{k+1}\rangle
$$

is a [group homomorphism](../../../group-theory.md#group-homomorphism) because all elements commute. It is surjective by construction and injective because the intersection of its two factors is trivial: $hx=h'x'$ implies $h'^{-1}h=x'x^{-1}$ lies in that intersection. Hence $H_{k+1}\cong H_k\times C_p$, and its order is $p$ times the previous order. Strict growth and finiteness ensure that the construction ends at $G$. Therefore

$$
\boxed{G\cong C_p^n,}
$$

where $n$ is the number of factors, possibly zero. This is an [elementary abelian group](../../../group.md#elementary-abelian-group), obtained by an explicit [direct product of groups](../../../group-theory.md#direct-product-of-groups) construction.

<h3 id="6d/iii">iii</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6d/iii)

Write a [matrix](../../../vector-space.md#matrix) in the [upper unitriangular group](../../../finite-group-theory.md#upper-unitriangular-group) as $M=I+A$. Here $A^3=0$, and its only potentially nonzero entry in $A^2$ is $(A^2)_{13}=ab$. The [binomial theorem](../../../combinatorics.md#binomial-theorem) therefore gives the [unitriangular matrix power formula](../../../finite-group-theory.md#unitriangular-matrix-power-formula)

$$
M^j=I+jA+\binom j2 A^2.
$$

For an odd [prime number](../../../number-theory.md#prime-number) $p$, both $p$ and $\binom p2=p(p-1)/2$ vanish in the [finite field](../../../algebra.md#finite-field) $\mathbb F_p$. Thus $M^p=I$. A nonidentity $M$ has order dividing the prime $p$ (by the same exponent-division argument as in part (i)), and so has order exactly $p$.

For $p=2$, take $a=b=1$ and $x=0$. Then $M^2=I+A^2\ne I$, while $M^4=(I+A^2)^2=I$. This element has order $4$, not $2$. Hence **every nonidentity element has order $p$ exactly for odd $p$**. The counterexample at $p=2$ accounts for the quadratic term in the [matrix](../../../vector-space.md#matrix) power formula.

## 7D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7d/i">i</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/i/solution">Solution</h4>

↑ **Parent:** [I](#7d/i)

Identify the [projective line](../../../finite-group-theory.md#projective-line) with one-dimensional subspaces of $\mathbb F_p^2$: use $v_t=(t,1)^T$ for finite $t$, and $v_\infty=(1,0)^T$. This convention turns the [matrix](../../../vector-space.md#matrix) action into the stipulated [Möbius transformation](../../../group-theory.md#mobius-transformation).

Since $x$ and $z$ are distinct projective points, $v_z,v_x$ are a [basis](../../../vector-space.md#basis). Write $v_y=A v_z+B v_x$. Both $A$ and $B$ are nonzero, because $y$ is different from $x,z$. The [matrix](../../../vector-space.md#matrix) with columns $A v_z$ and $B v_x$ is invertible and sends the lines of $(1,0)^T,(0,1)^T,(1,1)^T$ to those of $z,x,y$, respectively. This constructs the requested map without separate exceptional formulas at infinity.

A [matrix](../../../vector-space.md#matrix) fixing $0$ and $\infty$ is diagonal, say $\operatorname{diag}(a,d)$ with $a,d\ne0$. To fix $1$ it must also satisfy $a=d$, so the [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) of $(0,1,\infty)$ is precisely $\{\lambda I:\lambda\in\mathbb F_p^\times\}$. Any two solutions differ on the right by one of these [matrices](../../../vector-space.md#matrix). Thus

$$
\boxed{\text{There are exactly }p-1\text{ matrices for each distinct target triple.}}
$$

Equivalently, after dividing out [scalar matrices](../../../linear-algebra.md#scalar-matrix) the [projective general linear group action on the projective line](../../../finite-group-theory.md#projective-general-linear-group-action-on-the-projective-line) is [sharply three-transitive on a projective line](../../../finite-group-theory.md#sharply-three-transitive-on-a-projective-line).

<h3 id="7d/ii">ii</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7d/ii)

The [Möbius transformations](../../../group-theory.md#mobius-transformation) are bijections, so they preserve which coordinates of a triple are equal. Conversely, part (i) implies transitivity within each equality pattern. For a pattern with fewer than three distinct entries, extend the chosen distinct points to a triple before applying part (i); this works also for $p=2$, when the [projective line](../../../finite-group-theory.md#projective-line) has exactly three points. There are therefore five [orbits of a group action](../../../group-theory.md#orbit-of-a-group-action).

We first count $|GL_2(\mathbb F_p)|$. Its first column can be any nonzero [vector](../../../vector-space.md#vector), giving $p^2-1$ choices. The second must be outside the first column's one-dimensional span, giving $p^2-p$ choices. Hence

$$
|G|=(p^2-1)(p^2-p)=p(p-1)^2(p+1).
$$

For the all-equal pattern take $(\infty,\infty,\infty)$. Its [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) consists of upper triangular [matrices](../../../vector-space.md#matrix)

$$
\begin{pmatrix}a&b\\0&d\end{pmatrix},\qquad a,d\ne0,
$$

of order $p(p-1)^2$. Its [group orbit](../../../group-theory.md#orbit-of-a-group-action) has order $p+1$.

The three exactly-two-equal patterns have representatives $(\infty,\infty,0)$, $(\infty,0,\infty)$ and $(0,\infty,\infty)$. Each [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) fixes $0$ and $\infty$ individually, so it is the diagonal [subgroup](../../../group.md#subgroup) of order $(p-1)^2$. Each [group orbit](../../../group-theory.md#orbit-of-a-group-action) has order $p(p+1)$; their repeated-coordinate positions keep these three orbits distinct.

For the all-distinct pattern use $(0,1,\infty)$. Its [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) is the scalar [subgroup](../../../group.md#subgroup) of order $p-1$, and the [group orbit](../../../group-theory.md#orbit-of-a-group-action) has order $(p+1)p(p-1)$. Stabilizers of arbitrary triples are conjugates of the displayed representative stabilizers. In summary the [equality-pattern orbits of projective triples](../../../group-theory.md#equality-pattern-orbits-of-projective-triples) have

$$
\boxed{\begin{array}{c|c|c}
\text{pattern}&\text{orbit size}&\text{stabilizer order}\\\hline
\text{all equal}&p+1&p(p-1)^2\\
\text{each two-equal pattern}&p(p+1)&(p-1)^2\\
\text{all distinct}&p(p+1)(p-1)&p-1
\end{array}}
$$

The sizes add to $(p+1)^3$, and each orbit size times its stabilizer order is $|G|$, as in the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem).

## 8D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8d/a">a</h3>

↑ **Parent:** [8D](#8d)

<h4 id="8d/a/solution">Solution</h4>

↑ **Parent:** [A](#8d/a)

A [subgroup](../../../group.md#subgroup) $N$ is a [normal subgroup](../../../group-theory.md#normal-subgroup) of $G$ if $gNg^{-1}=N$ for every $g\in G$. Define multiplication on its left [cosets](../../../group-theory.md#coset) by

$$
(gN)(hN)=ghN.
$$

To check that this is well-defined, replace $g,h$ by $gn_1,hn_2$ with $n_1,n_2\in N$. Then

$$
(gn_1)(hn_2)=gh(h^{-1}n_1h)n_2\in ghN,
$$

because normality gives $h^{-1}n_1h\in N$. Thus the product depends only on the two [cosets](../../../group-theory.md#coset). Associativity follows from that of $G$, the identity is $N$, and the inverse of $gN$ is $g^{-1}N$. These are all the [group axioms](../../../group.md#group-axioms), so **$G/N$ is a [group](../../../group.md) under coset multiplication**. The natural projection $g\mapsto gN$ is a surjective [group homomorphism](../../../group-theory.md#group-homomorphism) with kernel $N$.

<h3 id="8d/b">b</h3>

↑ **Parent:** [8D](#8d)

<h4 id="8d/b/i">i</h4>

↑ **Parent:** [B](#8d/b)

<h5 id="8d/b/i/solution">Solution</h5>

↑ **Parent:** [I](#8d/b/i)

Take $G=C_2\times C_2$ and $N=C_2\times\{1\}$. Both are nontrivial, and $N$ is normal because $G$ is abelian. The second-coordinate projection identifies the [quotient group](../../../group-theory.md#quotient-group) $G/N$ with $C_2$. Swapping the two coordinates identifies $(G/N)\times N$ with $G$, so

$$
\boxed{G=C_2\times C_2,\quad N=C_2\times\{1\},\quad (G/N)\times N\cong G.}
$$

This is a [direct product of groups](../../../group-theory.md#direct-product-of-groups) with its first factor as the specified [normal subgroup](../../../group-theory.md#normal-subgroup).

<h4 id="8d/b/ii">ii</h4>

↑ **Parent:** [B](#8d/b)

<h5 id="8d/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8d/b/ii)

Use additive notation and take $G=\mathbb Z/4\mathbb Z$, $N=\{0,2\}$. Its [quotient group](../../../group-theory.md#quotient-group) is $C_2$. A [group homomorphism](../../../group-theory.md#group-homomorphism) from $C_2$ sends its generator to an element annihilated by $2$, so the image must be either $0$ or $2$. Both project to the identity coset $N$, and neither can project to the nonidentity generator of $G/N$. Therefore **this quotient projection has no homomorphic section**. It is a nonsplit [group extension](../../../group-theory.md#group-extension), despite both $G$ and $N$ being nontrivial finite [groups](../../../group.md).

<h4 id="8d/b/iii">iii</h4>

↑ **Parent:** [B](#8d/b)

<h5 id="8d/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#8d/b/iii)

Take $G=S_3$ and its [normal subgroup](../../../group-theory.md#normal-subgroup) $N=A_3=\langle r\rangle$, where $r=(1\ 2\ 3)$. Normality follows either from the [sign of a permutation](../../../finite-group-theory.md#sign-of-a-permutation) or directly from conjugation sending $r$ to $r$ or $r^{-1}$. The [quotient group](../../../group-theory.md#quotient-group) has order two, and $t=(1\ 2)$ provides a section $i:C_2\to S_3$ because $t^2=1$ and $tN$ is its nonidentity coset.

However, the map $\Phi(q,n)=i(q)n$ from the [direct product of groups](../../../group-theory.md#direct-product-of-groups) is not a [group homomorphism](../../../group-theory.md#group-homomorphism). In its domain $(1,r)$ commutes with $(tN,1)$, whereas their images $r$ and $t$ do not commute: $trt^{-1}=r^{-1}\ne r$. This is a [split group extension](../../../group-theory.md#split-group-extension) giving a genuine [semidirect product](../../../group-theory.md#semidirect-product) instead of a direct product. **The pair $S_3,A_3$ supplies the required split but non-direct example.**

For the general bijectivity assertion, let $\pi:G\to G/N$ be the quotient projection and assume $\pi\circ i$ is the identity. Given $g\in G$, put $q=\pi(g)$ and $n=i(q)^{-1}g$. Then $\pi(n)=q^{-1}q=1$, so $n\in N$ and $g=i(q)n$. This proves surjectivity of $\Phi$. If $i(q)n=i(q')n'$, applying $\pi$ gives $q=q'$, after which cancellation gives $n=n'$. Thus

$$
\boxed{\Phi:(G/N)\times N\longrightarrow G\text{ is always a bijection.}}
$$

This [section normal form for a split group extension](../../../group-theory.md#section-normal-form-for-a-split-group-extension) does not require finiteness. The obstruction to its being a homomorphism is the nontrivial conjugation action of the section on $N$.

## 9A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9a/a">a</h3>

↑ **Parent:** [9A](#9a)

<h4 id="9a/a/solution">Solution</h4>

↑ **Parent:** [A](#9a/a)

Away from the vertex, use the defining [function](../../../function.md) $H=z^2-x^2-y^2$. Its [gradient](../../../calculus.md#gradient) is normal to the smooth part of the [double circular cone](../../../geometry-and-topology.md#double-circular-cone), and

$$
\mathbf F\cdot\nabla H=(x,y,z)\cdot(-2x,-2y,2z)=2H=0
$$

on the surface. Hence **the field is tangent at every regular point of the cone**. At the origin the cone has no unique tangent plane, but $\mathbf F(0)=0$, which belongs to its tangent cone. An equivalent argument, valid also at the vertex, uses the [integral curves of a vector field](../../../calculus.md#integral-curve-of-a-vector-field): $\dot{\mathbf x}=\mathbf x$ has solution $\mathbf x(t)=e^t\mathbf x(0)$, and these dilations preserve $H=0$. This is an example of [radial dilation tangency to homogeneous zero sets](../../../calculus.md#radial-dilation-tangency-to-homogeneous-zero-sets).

<h3 id="9a/b">b</h3>

↑ **Parent:** [9A](#9a)

<h4 id="9a/b/solution">Solution</h4>

↑ **Parent:** [B](#9a/b)

At every regular point of the [double circular cone](../../../geometry-and-topology.md#double-circular-cone), its normal is perpendicular to $\mathbf F$ by part (a). Therefore the integrand of the [flux integral](../../../calculus.md#flux-integral) vanishes pointwise:

$$
\boxed{\int_S\mathbf F\cdot d\mathbf S=0.}
$$

The vertex, if included, is a single point of zero surface area and does not alter the [surface integral](../../../calculus.md#surface-integral). The answer is independent of both the subset and its orientation. Tangency, rather than a cancellation between different parts of the surface, explains the zero flux.

<h3 id="9a/c">c</h3>

↑ **Parent:** [9A](#9a)

<h4 id="9a/c/solution">Solution</h4>

↑ **Parent:** [C](#9a/c)

In [cylindrical coordinates](../../../calculus.md#cylindrical-coordinate-system) $r=\sqrt{x^2+y^2}$, the bounded solid enclosed by the two conical sheets and the [circular cylinder](../../../differential-geometry.md#circular-cylinder) is

$$
0\le r\le1,\qquad -r\le z\le r,\qquad 0\le\theta<2\pi.
$$

Its meridional section consists of two triangular regions; revolving them about the $z$-axis gives the solid. The two conical sheets meet at the origin and meet the [circular cylinder](../../../differential-geometry.md#circular-cylinder) in its circles at $z=\pm1$.

<a id="9a/c/image-the-bounded-solid-between-two-cones-and-a-unit-cylinder-with-its-meridional-section"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3-cone-cylinder.png)

**[Figure 1](#9a/c/image-the-bounded-solid-between-two-cones-and-a-unit-cylinder-with-its-meridional-section). The bounded solid between two cones and a unit cylinder, with its meridional section**.

Since $\mathbf F=(x,y,z)$, its [divergence](../../../calculus.md#divergence) is $3$. Integrate directly with the [cylindrical coordinates](../../../calculus.md#cylindrical-coordinate-system) volume element $r\,dz\,dr\,d\theta$:

$$
\int_V\nabla\cdot\mathbf F\,dV
=\int_0^{2\pi}\int_0^1\int_{-r}^r3r\,dz\,dr\,d\theta
=12\pi\int_0^1r^2\,dr
=\boxed{4\pi}.
$$

The same calculation gives $\operatorname{Vol}(V)=4\pi/3$.

<h3 id="9a/d">d</h3>

↑ **Parent:** [9A](#9a)

<h4 id="9a/d/solution">Solution</h4>

↑ **Parent:** [D](#9a/d)

Close the truncated two-sheet [double circular cone](../../../geometry-and-topology.md#double-circular-cone) by the lateral [circular cylinder](../../../differential-geometry.md#circular-cylinder) $r=1$, $-1\le z\le1$. Together these form the boundary of the solid in part (c); no planar caps are required because the cone meets the [circular cylinder](../../../differential-geometry.md#circular-cylinder) along both end circles. On the [circular cylinder](../../../differential-geometry.md#circular-cylinder) the outward unit normal is $(\cos\theta,\sin\theta,0)$, so $\mathbf F\cdot\mathbf n=1$, and $dS=d\theta\,dz$. Its [flux integral](../../../calculus.md#flux-integral) is

$$
\int_{-1}^1\int_0^{2\pi}1\,d\theta\,dz=4\pi.
$$

The [divergence theorem](../../../calculus.md#divergence-theorem) now gives $\int_S\mathbf F\cdot d\mathbf S+4\pi=4\pi$, using the volume integral from part (c). Hence

$$
\boxed{\int_S\mathbf F\cdot d\mathbf S=0,}
$$

agreeing with tangency. The isolated vertex can be handled by excising a ball of radius $\varepsilon$ and passing to the limit: since $|\mathbf F|=O(\varepsilon)$ there and the added area is $O(\varepsilon^2)$, its extra flux is $O(\varepsilon^3)$ and tends to zero.

## 10A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10a/a">a</h3>

↑ **Parent:** [10A](#10a)

<h4 id="10a/a/solution">Solution</h4>

↑ **Parent:** [A](#10a/a)

For an oriented piecewise smooth surface $S$ and a continuously differentiable [vector field](../../../calculus.md#vector-field) on a neighborhood of it, [Stokes theorem](../../../calculus.md#stokes-theorem) states

$$
\boxed{\int_S(\nabla\times\mathbf F)\cdot d\mathbf S
=\oint_{\partial S}\mathbf F\cdot d\mathbf x.}
$$

The [oriented surface element](../../../calculus.md#oriented-surface-element) and boundary direction must agree by the right-hand rule. Every boundary component is included; for an upward-oriented graph over an [annulus](../../../topology.md#annulus-mathematics) the outer boundary is anticlockwise and the inner boundary clockwise when viewed from above.

<h3 id="10a/b">b</h3>

↑ **Parent:** [10A](#10a)

<h4 id="10a/b/solution">Solution</h4>

↑ **Parent:** [B](#10a/b)

Use the positive graph $z=g(x,y)=\sqrt{1+x^2+y^2}$. The printed PDF bounds are $\sqrt2\le z\le\sqrt5$, so its projection is the [annulus](../../../topology.md#annulus-mathematics) $1\le r\le2$. The surface is the corresponding band of the upper sheet of a [two-sheeted hyperboloid](../../../differential-geometry.md#two-sheeted-hyperboloid), bounded by circles of radii $1$ and $2$ at heights $\sqrt2$ and $\sqrt5$.

<a id="10a/b/image-the-upper-hyperboloid-band-between-heights-square-root-of-two-and-square-root-of-five-with-annular-projection"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3-hyperboloid-annulus.png)

**[Figure 2](#10a/b/image-the-upper-hyperboloid-band-between-heights-square-root-of-two-and-square-root-of-five-with-annular-projection). The upper hyperboloid band between heights square root of two and square root of five, with annular projection**.

For the parametrization $\mathbf R(x,y)=(x,y,g(x,y))$, its tangent [vectors](../../../vector-space.md#vector) are $(1,0,x/z)$ and $(0,1,y/z)$. Their [cross product](../../../vector-space.md#cross-product) gives the upward [vector surface element of a graph](../../../calculus.md#vector-surface-element-of-a-graph):

$$
\boxed{d\mathbf S=\left(-\frac{x}{z},-\frac{y}{z},1\right)dx\,dy,
\qquad z=\sqrt{1+x^2+y^2}.}
$$

Its magnitude gives the scalar [surface area of a graph](../../../calculus.md#surface-area-of-a-graph):

$$
\boxed{dS=\sqrt{\frac{1+2(x^2+y^2)}{1+x^2+y^2}}\,dx\,dy.}
$$

Both formulas apply on $1\le\sqrt{x^2+y^2}\le2$. Reversing the orientation changes only the sign of the [vector](../../../vector-space.md#vector) element.

<h3 id="10a/c">c</h3>

↑ **Parent:** [10A](#10a)

<h4 id="10a/c/solution">Solution</h4>

↑ **Parent:** [C](#10a/c)

Direct use of [partial derivatives](../../../calculus.md#partial-derivative) gives

$$
\boxed{\nabla\times\mathbf F=(x^2+2xy,-2xy-y^2,2).}
$$

With the upward [oriented surface element](../../../calculus.md#oriented-surface-element) found in part (b), the [curl](../../../calculus.md#curl) flux integrand over the [annulus](../../../topology.md#annulus-mathematics) $A$ becomes

$$
2+\frac{-x^3-2x^2y+2xy^2+y^3}{\sqrt{1+x^2+y^2}}.
$$

Every term in the numerator is odd in $x$ or $y$, so its integral over the symmetric [annulus](../../../topology.md#annulus-mathematics) is zero. Thus the [surface integral](../../../calculus.md#surface-integral) is

$$
\int_S(\nabla\times\mathbf F)\cdot d\mathbf S
=2\operatorname{Area}(A)=2\pi(2^2-1^2)=6\pi.
$$

Each boundary circle has constant $z$, hence $dz=0$. Its [line integral](../../../calculus.md#line-integral) is therefore $\int(-y\,dx+x\,dy)$, with no contribution from the third field component. An anticlockwise radius-$r$ circle gives $2\pi r^2$. The outward boundary orientation is anticlockwise at $r=2$ and clockwise at $r=1$, so

$$
\oint_{\partial S}\mathbf F\cdot d\mathbf x=8\pi-2\pi=\boxed{6\pi}.
$$

The two computed values agree, verifying [Stokes theorem](../../../calculus.md#stokes-theorem) with both boundary components. A downward choice would give $-6\pi$ on both sides.

## 11A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11a/i">i</h3>

↑ **Parent:** [11A](#11a)

<h4 id="11a/i/solution">Solution</h4>

↑ **Parent:** [I](#11a/i)

For $\mathbf F=\nabla\phi$, the definition of the [Laplacian](../../../calculus.md#laplacian) gives $\nabla\cdot\mathbf F=\nabla^2\phi=f$. Integrating over $V$ and applying the [divergence theorem](../../../calculus.md#divergence-theorem) yields

$$
\boxed{\int_V f\,dV=\int_V\nabla\cdot\mathbf F\,dV
=\int_{\partial V}\mathbf F\cdot d\mathbf S.}
$$

This is the flux form of [Poisson equation](../../../partial-differential-equation.md#poisson-equation), for an outward-oriented piecewise smooth boundary and the usual smoothness of $\phi$ on a neighborhood of the volume. In particular, a singularity cannot be ignored when applying this identity.

<h3 id="11a/ii">ii</h3>

↑ **Parent:** [11A](#11a)

<h4 id="11a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11a/ii)

On the outward-oriented [sphere](../../../geometry-and-topology.md#sphere) of radius $R$, $\mathbf n=\mathbf x/R$, so $\mathbf x\cdot d\mathbf S=R\,dS$. Hence

$$
\boxed{I=\frac1{R^2}\operatorname{Area}(S_R)=4\pi.}
$$

Away from the origin, the [divergence and curl of a radial vector field](../../../calculus.md#divergence-and-curl-of-a-radial-vector-field) with $f(r)=r^{-3}$ give

$$
\nabla\cdot\left(\frac{\mathbf x}{r^3}\right)=r(-3r^{-4})+3r^{-3}=0.
$$

If the enclosed volume excludes the origin and its boundary avoids it, this field is smooth throughout the volume. The [divergence theorem](../../../calculus.md#divergence-theorem) then gives **$I=0$**. The nonzero [sphere](../../../geometry-and-topology.md#sphere) flux is compatible with zero [divergence](../../../calculus.md#divergence) away from the origin because the enclosed singularity prevents applying that smooth-volume theorem directly to the full ball.

<h3 id="11a/iii">iii</h3>

↑ **Parent:** [11A](#11a)

<h4 id="11a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#11a/iii)

The [electric field](../../../electromagnetism.md#electric-field) of this [point charge](../../../electromagnetism.md#point-charge) is a translated and scaled version of the radial field in part (ii). If $\mathbf a\notin V$ and $\mathbf a\notin\partial V$, its [divergence](../../../calculus.md#divergence) vanishes throughout $V$, so the [divergence theorem](../../../calculus.md#divergence-theorem) gives zero [flux integral](../../../calculus.md#flux-integral).

If $\mathbf a$ lies inside $V$, remove a small ball centered at $\mathbf a$. On the remaining volume the [divergence](../../../calculus.md#divergence) is zero. Its boundary is $\partial V$ together with the small [sphere](../../../geometry-and-topology.md#sphere), whose outward normal for the punctured volume points towards $\mathbf a$. That inner [sphere](../../../geometry-and-topology.md#sphere) contributes $-q/\epsilon_0$, by the $4\pi$ [sphere](../../../geometry-and-topology.md#sphere) flux computed in part (ii). Thus the exterior flux must be $q/\epsilon_0$:

$$
\boxed{\int_{\partial V}\mathbf E\cdot d\mathbf S
=\begin{cases}0,&\mathbf a\notin V,\\q/\epsilon_0,&\mathbf a\in V.\end{cases}}
$$

This is [Gauss's law](../../../electromagnetism.md#gauss-s-law) for a [point charge](../../../electromagnetism.md#point-charge). The assumption that the charge is not on the boundary is essential to these alternatives.

<h3 id="11a/iv">iv</h3>

↑ **Parent:** [11A](#11a)

<h4 id="11a/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#11a/iv)

Rotational symmetry of the [vector field](../../../calculus.md#vector-field) means $\mathbf F(r\mathbf n)=h(r)\mathbf n$: rotations fixing $\mathbf n$ force the field to be parallel to $\mathbf n$, and rotations between directions make its magnitude depend only on $r$. Its [flux integral](../../../calculus.md#flux-integral) over the radius-$r$ [sphere](../../../geometry-and-topology.md#sphere) is $4\pi r^2h(r)$. Applying the flux identity from part (i) to the ball, with the spherically symmetric source, gives

$$
4\pi r^2h(r)=4\pi\int_0^r f(s)s^2\,ds.
$$

Therefore the [origin-regular spherical Poisson flux law](../../../geometry-and-topology.md#origin-regular-spherical-poisson-flux-law) is

$$
\boxed{\mathbf F(\mathbf x)=\frac{\mathbf x}{|\mathbf x|^3}
\int_0^{|\mathbf x|}f(s)s^2\,ds.}
$$

Only source values at $s\le|\mathbf x|$ occur. Changing the exterior source can change the scalar potential by an interior constant, but cannot change this radial [gradient](../../../calculus.md#gradient). Regularity on all of $\mathbb R^3$, inherited from the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) setting, matters: on a punctured domain alone an additional $C\mathbf x/r^3$ would have zero [divergence](../../../calculus.md#divergence) away from the origin and would not be fixed by the local source. It is excluded here by the origin regularity needed for the ball flux identity.

## 12A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12a/a">a</h3>

↑ **Parent:** [12A](#12a)

<h4 id="12a/a/solution">Solution</h4>

↑ **Parent:** [A](#12a/a)

Define

$$
\boxed{s_{ij}=\frac{t_{ij}+t_{ji}}2,\qquad a_{ij}=\frac{t_{ij}-t_{ji}}2.}
$$

They sum to $t_{ij}$, with $s_{ji}=s_{ij}$ and $a_{ji}=-a_{ij}$. Interchanging two slots of a [tensor](../../../linear-algebra.md#tensor) still produces a [tensor](../../../linear-algebra.md#tensor), so these are a [symmetric second-rank tensor](../../../linear-algebra.md#symmetric-second-rank-tensor) and an [antisymmetric second-rank tensor](../../../linear-algebra.md#antisymmetric-second-rank-tensor), not merely symmetric and antisymmetric arrays in a selected frame.

For uniqueness, if $t=s+a=s'+a'$, then $s-s'=a'-a$. The common difference is both symmetric and antisymmetric, so each of its components equals its own negative and vanishes over $\mathbb R$. Thus **the decomposition is unique**. These are the [symmetric and antisymmetric parts of a matrix](../../../linear-algebra.md#symmetric-and-antisymmetric-parts-of-a-matrix), with their [tensor](../../../linear-algebra.md#tensor) transformation law preserved.

<h3 id="12a/b">b</h3>

↑ **Parent:** [12A](#12a)

<h4 id="12a/b/i">i</h4>

↑ **Parent:** [B](#12a/b)

<h5 id="12a/b/i/solution">Solution</h5>

↑ **Parent:** [I](#12a/b/i)

Under a proper [rotation matrix](../../../linear-algebra.md#rotation-matrix) $R$, invariance of a [Cartesian second-rank tensor](../../../linear-algebra.md#cartesian-second-rank-tensor) reads $T=RTR^T$, equivalently $TR=RT$. The half-turn $R_z(\pi)=\operatorname{diag}(-1,-1,1)$ forces all entries mixing the $z$ direction with the $xy$ plane to vanish. Thus $T$ consists of a planar $2\times2$ block $B$ and the entry $T_{33}=c$.

Commutation with the planar quarter-turn $J=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ gives $B=aI+bJ$. This block already commutes with every planar rotation. Now use the half-turn $R_x(\pi)=\operatorname{diag}(1,-1,-1)$: on the planar block its conjugation fixes $I$ and sends $J$ to $-J$, so invariance forces $b=0$. Therefore

$$
\boxed{T=\operatorname{diag}(a,a,c),\qquad
t_{ij}=\alpha\delta_{ij}+\beta\delta_{i3}\delta_{j3},\quad
\alpha=a,\ \beta=c-a.}
$$

The formula uses the [Kronecker delta](../../../linear-algebra.md#kronecker-delta) and is sufficient as well as necessary: rotations preserving the unoriented $z$-axis fix both $I$ and $e_3e_3^T$. This is an [axially invariant second-rank tensor](../../../linear-algebra.md#axially-invariant-second-rank-tensor) with the planar antisymmetric part removed by the horizontal half-turn.

<h4 id="12a/b/ii">ii</h4>

↑ **Parent:** [B](#12a/b)

<h5 id="12a/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#12a/b/ii)

Let $R$ be rotation through $2\pi/3$ about $z$, and let $S$ be rotation through $\pi$ about $x$. These generate the order-six [dihedral group](../../../finite-group-theory.md#dihedral-group) with relations

$$
R^3=S^2=I,\qquad SRS=R^{-1},
$$

namely $\{I,R,R^2,S,RS,R^2S\}$. We specify its order explicitly because dihedral notation has two conventions. It is a proper finite [subgroup](../../../group.md#subgroup) of the full axial rotation [group](../../../group.md).

To see that it is sufficient, write a general [matrix](../../../vector-space.md#matrix) in blocks $T=\begin{pmatrix}B&u\\v^T&c\end{pmatrix}$. Commutation with $R$ forces $u=v=0$, since a nontrivial planar $120$-degree rotation fixes no nonzero planar [vector](../../../vector-space.md#vector). Its planar part is $\cos(2\pi/3)I+\sin(2\pi/3)J$, with nonzero sine, so $B$ must commute with $J$ and has the form $aI+bJ$. Commutation with $S$ again kills $b$. Hence this six-element [subgroup](../../../group.md#subgroup) has precisely the required invariant [tensors](../../../linear-algebra.md#tensor).

It is also smallest by order. [Groups](../../../group.md) of orders $2,3,5$ are cyclic: a nonidentity element has order dividing the prime [group](../../../group.md) order by [Lagrange theorem](../../../group-theory.md#lagrange-s-theorem). For a cyclic rotation [subgroup](../../../group.md#subgroup), the nonzero antisymmetric [tensor](../../../linear-algebra.md#tensor) representing [cross product](../../../vector-space.md#cross-product) with its rotation-axis direction is invariant, so it cannot force the symmetric form above. The trivial [subgroup](../../../group.md#subgroup) plainly imposes no constraint. A [group](../../../group.md) of order four is either cyclic or has three nonidentity elements of order two; in the latter case they commute, since $(AB)^{-1}=AB$ and also equals $BA$. Commuting distinct half-turns in three dimensions have perpendicular axes: conjugation by one half-turn must preserve the other's axis, and a distinct preserved axis lies in its perpendicular plane. In the specified axial [group](../../../group.md), their three axes are consequently $z$ and two perpendicular horizontal directions. In coordinates along them every [diagonal matrix](../../../linear-algebra.md#diagonal-matrix) is invariant, including one with unequal horizontal entries. Such a [group](../../../group.md) again does not force the required form.

Thus **the smallest [subgroup](../../../group.md#subgroup) has six elements**, generated by the axial $120$-degree rotation and one horizontal half-turn. It is the [smallest axial rotation group forcing second-rank transverse isotropy](../../../linear-algebra.md#smallest-axial-rotation-group-forcing-second-rank-transverse-isotropy); conjugating the horizontal axis gives equally valid choices.

<h3 id="12a/c">c</h3>

↑ **Parent:** [12A](#12a)

<h4 id="12a/c/i">i</h4>

↑ **Parent:** [C](#12a/c)

<h5 id="12a/c/i/solution">Solution</h5>

↑ **Parent:** [I](#12a/c/i)

Split the array in its first two slots:

$$
d^s_{ijk}=\frac{d_{ijk}+d_{jik}}2,\qquad
d^a_{ijk}=\frac{d_{ijk}-d_{jik}}2.
$$

For every [symmetric second-rank tensor](../../../linear-algebra.md#symmetric-second-rank-tensor) $s$, antisymmetry gives $d^a_{ijk}s_{ij}=0$. Hence the stipulated [vector](../../../vector-space.md#vector) equals $d^s_{ijk}s_{ij}$.

Let $R$ change the orthonormal frame, so $s'_{ab}=R_{ai}R_{bj}s_{ij}$. The [vector](../../../vector-space.md#vector) transformation law gives

$$
d^{s\prime}_{abc}R_{ai}R_{bj}s_{ij}
=R_{ck}d^s_{ijk}s_{ij}
$$

for every symmetric test $s$. Both coefficient arrays in $i,j$ are symmetric, so equality against every symmetric [matrix](../../../vector-space.md#matrix) forces equality of the coefficients; one may test the individual diagonal entries and the symmetric off-diagonal [basis](../../../vector-space.md#basis) [matrices](../../../vector-space.md#matrix). Multiplying by $R_{ai}R_{bj}$ and using orthogonality yields

$$
\boxed{d^{s\prime}_{abc}=R_{ai}R_{bj}R_{ck}d^s_{ijk}.}
$$

This is exactly the rank-three [tensor](../../../linear-algebra.md#tensor) law. It is the [symmetric-test criterion for a third-rank Cartesian tensor](../../../linear-algebra.md#symmetric-test-criterion-for-a-third-rank-cartesian-tensor), a form of the [quotient theorem for Cartesian tensors](../../../linear-algebra.md#quotient-theorem-for-cartesian-tensors). Equivalently one may test $s_{ij}=(u_iv_j+v_iu_j)/2$ for arbitrary [vectors](../../../vector-space.md#vector) $u,v$ and apply the quotient theorem twice.

<h4 id="12a/c/ii">ii</h4>

↑ **Parent:** [C](#12a/c)

<h5 id="12a/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#12a/c/ii)

**The antisymmetric part need not be a [tensor](../../../linear-algebra.md#tensor).** Its contraction with every symmetric test is zero, so the premise imposes no transformation law on it. This is the [blindness of symmetric contraction tests to antisymmetric arrays](../../../linear-algebra.md#blindness-of-symmetric-contraction-tests-to-antisymmetric-arrays), now with a third free index.

For a concrete example, prescribe the same numerical array in every orthonormal frame, with only

$$
d^a_{121}=1,\qquad d^a_{211}=-1
$$

nonzero, and take $d^s=0$. Every contraction $d^a_{ijk}s_{ij}$ vanishes, and the zero result is a genuine [vector](../../../vector-space.md#vector) in every frame. But under $R=\operatorname{diag}(-1,-1,1)$ the rank-three [tensor](../../../linear-algebra.md#tensor) transformation law would send the $121$ component to $-1$, whereas our framewise prescription leaves it equal to $1$. Thus the array is not a [tensor](../../../linear-algebra.md#tensor) despite satisfying every stipulated contraction test. An antisymmetric part could be a [tensor](../../../linear-algebra.md#tensor) if an additional transformation law were supplied; it is simply not forced to be one.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
