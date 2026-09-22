# Paper 20

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper20.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper20.pdf)

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
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
  - [iii](#6/iii)
    - [Solution](#6/iii/solution)
- [7](#7)
  - [Solution](#7/solution)
  - [i](#7/i)
    - [Solution](#7/i/solution)
  - [ii](#7/ii)
    - [Solution](#7/ii/solution)
  - [iii](#7/iii)
    - [Solution](#7/iii/solution)
- [8](#8)
  - [Solution](#8/solution)
- [9](#9)
  - [Solution](#9/solution)
- [10](#10)
  - [i](#10/i)
    - [Solution](#10/i/solution)
  - [ii](#10/ii)
    - [Solution](#10/ii/solution)
  - [iii](#10/iii)
    - [Solution](#10/iii/solution)
- [11](#11)
  - [i](#11/i)
    - [Solution](#11/i/solution)
  - [ii](#11/ii)
    - [Solution](#11/ii/solution)
- [12](#12)
  - [i](#12/i)
    - [Solution](#12/i/solution)
  - [ii](#12/ii)
    - [Solution](#12/ii/solution)

## 1

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For a [categorical presheaf](../../../category.md#presheaf-category-theory) $X:\mathcal C^{\mathrm{op}}\to\mathbf{Set}$ and $A\in\mathcal C$, the [Yoneda lemma](../../../category.md#yoneda-lemma) gives a [natural bijection](../../../category.md#natural-bijection)

$$
\operatorname{Nat}(\mathcal C(-,A),X)\cong X(A),\qquad \theta\longmapsto\theta_A(1_A).
$$

To construct its inverse, take $x\in X(A)$ and [set](../../../set.md) $\theta^x_U(h)=X(h)x$ for $h:U\to A$. For $k:V\to U$, the [functor](../../../category.md#functor) law gives $X(k)\theta^x_U(h)=X(hk)x=\theta^x_V(hk)$, so $\theta^x$ is a [natural transformation](../../../category.md#natural-transformation). Conversely, [naturality](../../../category.md#naturality) of any $\theta$ at $h:U\to A$ gives $\theta_U(h)=X(h)\theta_A(1_A)$. Thus the two constructions are inverse, proving the [bijection](../../../function.md#bijection).

The [bijection](../../../function.md#bijection) is natural in $X$: a [natural transformation](../../../category.md#natural-transformation) $t:X\to Y$ sends the distinguished element $x$ to $t_A(x)$ on either side. It is natural in $A$: for $f:A\to B$, precomposing a transformation $\mathcal C(-,B)\to X$ with postcomposition by $f$ sends its distinguished element $x\in X(B)$ to $X(f)x$. These equations prove the claimed [naturality](../../../category.md#naturality), rather than just an objectwise correspondence. Reversing [morphisms](../../../algebra.md#morphism) gives the covariant form $\operatorname{Nat}(\mathcal C(A,-),Z)\cong Z(A)$ for $Z:\mathcal C\to\mathbf{Set}$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Define the [Yoneda embedding](../../../category.md#yoneda-embedding) $H_\bullet:\mathcal C\to[\mathcal C^{\mathrm{op}},\mathbf{Set}]$ by $H_A(U)=\mathcal C(U,A)$ and $H_A(k)(h)=hk$. For $f:A\to B$, define $H_\bullet(f)_U(h)=fh$. Associativity proves [naturality](../../../category.md#naturality) in $U$, and preservation of [identity morphisms](../../../algebra.md#identity-morphism) and [composition in a category](../../../category.md#composition-in-a-category) proves that $H_\bullet$ is a [functor](../../../category.md#functor).

Apply the [Yoneda lemma](../../../category.md#yoneda-lemma) to $X=H_B$. It gives

$$
\boxed{\operatorname{Nat}(H_A,H_B)\cong\mathcal C(A,B).}
$$

The [natural transformation](../../../category.md#natural-transformation) corresponding to $f$ has component $h\mapsto fh$, exactly $H_\bullet(f)$. Therefore the induced map on every [hom-set](../../../category.md#hom-set) is a [bijection](../../../function.md#bijection): **the Yoneda embedding is [full and faithful](../../../category.md#full-and-faithful-functor)**.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

If $f:A\to B$ is a [monomorphism](../../../category.md#monomorphism), each [function](../../../function.md) $\mathcal C(U,A)\to\mathcal C(U,B)$ given by postcomposition with $f$ is injective. Consequently, if two [natural transformations](../../../category.md#natural-transformation) into $H_A$ become equal after $H_\bullet(f)$, their components are equal, and the transformations themselves are equal. This proves that $H_\bullet(f)$ is a [monomorphism](../../../category.md#monomorphism) in the [presheaf category](../../../category.md#presheaf-category).

Conversely, suppose $H_\bullet(f)$ is a [monomorphism](../../../category.md#monomorphism) and $u,v:U\to A$ satisfy $fu=fv$. Then $H_\bullet(f)H_\bullet(u)=H_\bullet(f)H_\bullet(v)$. Cancellation gives $H_\bullet(u)=H_\bullet(v)$, and faithfulness of the [Yoneda embedding](../../../category.md#yoneda-embedding) gives $u=v$. Hence **$H_\bullet(f)$ is monic exactly when $f$ is monic**.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

We first justify the relevant [pointwise epimorphism in a functor category](../../../category.md#pointwise-epimorphism-in-a-functor-category) criterion. A componentwise [surjective function](../../../algebra.md#surjective-function) gives an [epimorphism](../../../category.md#epimorphism), because equality of two composites can be cancelled at each component. Conversely, for a [natural transformation](../../../category.md#natural-transformation) $t:X\to Y$, form the pointwise [pushout](../../../category.md#pushout) $P=Y\amalg_XY$. Restrictions of $Y$ preserve the identifications imposed by $t$, so these pointwise [sets](../../../set.md) and restrictions form a [categorical presheaf](../../../category.md#presheaf-category-theory). The two inclusions $j_1,j_2:Y\to P$ satisfy $j_1t=j_2t$. If $t$ is epic, $j_1=j_2$. At an object $U$, an element outside the image of $t_U$ would retain two distinct copies in $P(U)$, contradicting this equality. Thus every $t_U$ is surjective.

Apply this criterion to $H_\bullet(f)$ at $B$. Surjectivity of $\mathcal C(B,A)\to\mathcal C(B,B)$ supplies $g:B\to A$ with $fg=1_B$. Conversely, if $fg=1_B$, then $H_\bullet(f)H_\bullet(g)=1_{H_B}$, making $H_\bullet(f)$ a [split epimorphism](../../../category.md#split-epimorphism) and hence an [epimorphism](../../../category.md#epimorphism). Therefore

$$
\boxed{H_\bullet(f)\text{ epic}\iff f\text{ split epic}.}
$$

## 2

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Name the upper objects $A,B,C$ and the lower objects $D,E,F$, so the [morphisms](../../../algebra.md#morphism) are $b:A\to B$, $c:B\to C$, $a:A\to D$, $g:B\to E$, $d:C\to F$, $f:D\to E$, and $e:E\to F$. The [commutative diagram](../../../homology.md#commutative-diagram) gives $gb=fa$ and $dc=eg$.

Take $u:T\to D$ and $v:T\to C$ with $efu=dv$. The right [pullback in a category](../../../category.md#pullback-category-theory) gives a unique $w:T\to B$ with $gw=fu$ and $cw=v$. The left [pullback in a category](../../../category.md#pullback-category-theory) then gives a unique $z:T\to A$ with $az=u$ and $bz=w$. It follows that $cbz=v$, giving the required factorization through the outside rectangle. Any other factorization has the same middle [morphism](../../../algebra.md#morphism) by uniqueness in the right [pullback in a category](../../../category.md#pullback-category-theory), and therefore is the same $z$ by uniqueness in the left [pullback in a category](../../../category.md#pullback-category-theory). **The outside rectangle is a pullback**.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Keep the notation of the preceding part. For $u:T\to D$ and $w:T\to B$ satisfying $fu=gw$, we have $efu=egw=dcw$. The outside [pullback in a category](../../../category.md#pullback-category-theory) gives a unique $z:T\to A$ with $az=u$ and $cbz=cw$. Moreover $gbz=faz=fu=gw$. The [morphisms](../../../algebra.md#morphism) $bz,w:T\to B$ thus have the same composites with $g$ and $c$. Uniqueness in the right [pullback in a category](../../../category.md#pullback-category-theory) gives $bz=w$. Any factorization through the left square also factors through the outside rectangle, so it is unique there. **The left square is a pullback**. Together these two arguments prove the [pullback pasting lemma](../../../category.md#pullback-pasting-lemma).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Here is a precise [base change of a pullback square](../../../category.md#base-change-of-a-pullback-square) statement. Suppose $A=B\times_D C$ is a [pullback in a category](../../../category.md#pullback-category-theory) and $t:D'\to D$ is a [morphism](../../../algebra.md#morphism). Assume the [pullbacks in a category](../../../category.md#pullback-category-theory)

$$
A'=A\times_D D',\quad B'=B\times_D D',\quad C'=C\times_D D'
$$

exist, where $A\to D$ is the common composite. The induced square with vertices $A',B',C',D'$ is a [pullback in a category](../../../category.md#pullback-category-theory); equivalently,

$$
\boxed{(B\times_D C)\times_D D'\cong(B\times_D D')\times_{D'}(C\times_D D').}
$$

Indeed, compatible [morphisms](../../../algebra.md#morphism) $T\to B'$ and $T\to C'$ give [morphisms](../../../algebra.md#morphism) $b:T\to B$, $c:T\to C$, and a common $v:T\to D'$, with the composites of $b,c$ to $D$ both equal to $tv$. The original [pullback in a category](../../../category.md#pullback-category-theory) gives a unique [morphism](../../../algebra.md#morphism) $h:T\to A$ with projections $b,c$. Its composite to $D$ is $tv$, so the defining [pullback in a category](../../../category.md#pullback-category-theory) for $A'$ gives a unique [morphism](../../../algebra.md#morphism) $T\to A'$ above $h,v$. Its maps to $B'$ and $C'$ are the prescribed ones by uniqueness in those [pullbacks in a category](../../../category.md#pullback-category-theory). Conversely, these projections recover $b,c,v$, so every possible factorization is the same. This proves the [universal property](../../../category-theory.md#universal-property) without requiring arbitrary [categorical limits](../../../category.md#categorical-limit) in the ambient [category](../../../category.md).

## 3

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For a [functor](../../../category.md#functor) $D:\mathcal J\to\mathcal C$ with finite indexing [category](../../../category.md), form the finite [products in a category](../../../category.md#product-category-theory)

$$
P=\prod_{j\in\operatorname{Ob}\mathcal J}D(j),\qquad Q=\prod_{u:i\to j\text{ in }\mathcal J}D(j).
$$

Define $s,t:P\rightrightarrows Q$ by requiring the coordinate indexed by $u:i\to j$ to be $D(u)\pi_i$ for $s$ and $\pi_j$ for $t$. Let $e:L\to P$ be their [equalizer](../../../category.md#equaliser), and put $\lambda_j=\pi_j e$. The equality $se=te$ says exactly that $D(u)\lambda_i=\lambda_j$ for every [morphism](../../../algebra.md#morphism) $u$, so these [morphisms](../../../algebra.md#morphism) form a [categorical cone](../../../category.md#cone-over-a-diagram).

For any other [categorical cone](../../../category.md#cone-over-a-diagram) $(x_j:X\to D(j))$, the [product in a category](../../../category.md#product-category-theory) gives a unique $x:X\to P$ with $\pi_jx=x_j$. The [categorical cone](../../../category.md#cone-over-a-diagram) equations give $sx=tx$, so the [equalizer](../../../category.md#equaliser) gives a unique $\bar x:X\to L$ with $e\bar x=x$. This is exactly the [universal property](../../../category-theory.md#universal-property) of a [categorical limit](../../../category.md#categorical-limit). Empty indexing products are [terminal objects](../../../category.md#terminal-object), so the construction includes the empty [diagram in a category](../../../category.md#diagram-category-theory). Thus **finite products and [equalizers](../../../category.md#equaliser) give all [finite limits](../../../category.md#finite-limit)**.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Let $1$ be a [terminal object](../../../category.md#terminal-object). The [pullback in a category](../../../category.md#pullback-category-theory) of $X\to1\leftarrow Y$ has precisely the [universal property](../../../category-theory.md#universal-property) of the binary [product in a category](../../../category.md#product-category-theory) $X\times Y$: every pair of [morphisms](../../../algebra.md#morphism) to $X,Y$ is compatible over $1$. Repeated binary [products in a category](../../../category.md#product-category-theory), together with $1$ as the empty product, give all finite [products in a category](../../../category.md#product-category-theory).

For $f,g:X\rightrightarrows Y$, form the [pullback in a category](../../../category.md#pullback-category-theory) of the [categorical diagonal](../../../category.md#categorical-diagonal) $\Delta_Y:Y\to Y\times Y$ along $\langle f,g\rangle:X\to Y\times Y$. Its projection $e:E\to X$ satisfies $fe=ge$. If $h:T\to X$ satisfies $fh=gh$, the pair $h,fh$ gives a unique [morphism](../../../algebra.md#morphism) into this [pullback in a category](../../../category.md#pullback-category-theory). Conversely any such [morphism](../../../algebra.md#morphism) must project to that pair. Hence $e$ is the [equalizer](../../../category.md#equaliser) of $f,g$. The preceding construction now gives **all [finite limits](../../../category.md#finite-limit)**.

## 4

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

For $D:\mathcal I\to\mathcal C$, define the [functor](../../../category.md#functor) $\operatorname{Cone}(-,D):\mathcal C^{\mathrm{op}}\to\mathbf{Set}$ by

$$
\operatorname{Cone}(X,D)=\operatorname{Nat}(\Delta X,D),
$$

where $\Delta X$ is the [constant diagram functor](../../../category.md#constant-diagram-functor); a [morphism](../../../algebra.md#morphism) into $X$ acts by precomposition on every [categorical cone](../../../category.md#cone-over-a-diagram) leg. A [categorical limit](../../../category.md#categorical-limit) is a [representation of a functor](../../../category.md#representation-of-a-functor) of the form

$$
\boxed{\mathcal C(-,L)\cong\operatorname{Cone}(-,D).}
$$

The image of $1_L$ is the universal [categorical cone](../../../category.md#cone-over-a-diagram) $\lambda:\Delta L\to D$. By [naturality](../../../category.md#naturality) of the representing [isomorphism](../../../algebra.md#isomorphism), the image of $h:X\to L$ is $\lambda\circ\Delta h$. Thus this definition is exactly existence and uniqueness of factorization of every [categorical cone](../../../category.md#cone-over-a-diagram) through $\lambda$. Conversely that [universal property](../../../category-theory.md#universal-property) gives the representing [natural bijection](../../../category.md#natural-bijection).

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Choose for each $j\in\mathcal J$ a [categorical limit](../../../category.md#categorical-limit) $L_j$ of $F(-,j)$, with projections $\lambda_{i,j}:L_j\to F(i,j)$. For $v:j\to k$, the [morphisms](../../../algebra.md#morphism) $F(1_i,v)\lambda_{i,j}$ form a [categorical cone](../../../category.md#cone-over-a-diagram) over $F(-,k)$, since the two actions of the product [functor](../../../category.md#functor) $F$ commute. Define $L(v):L_j\to L_k$ by the equations

$$
\lambda_{i,k}L(v)=F(1_i,v)\lambda_{i,j}\qquad(i\in\mathcal I).
$$

Existence and uniqueness follow from the [universal property](../../../category-theory.md#universal-property). The [identity morphism](../../../algebra.md#identity-morphism) of $L_j$ satisfies the equations for $v=1_j$, and $L(w)L(v)$ satisfies those for $wv$, so uniqueness gives $L(1_j)=1_{L_j}$ and $L(wv)=L(w)L(v)$. Hence $L:\mathcal J\to\mathcal D$ is a [functor](../../../category.md#functor).

If $L'_j$ with projections $\lambda'_{i,j}$ are other choices, there is a unique [isomorphism](../../../algebra.md#isomorphism) $u_j:L_j\to L'_j$ carrying every projection to the corresponding projection. The same equations show $u_kL(v)=L'(v)u_j$, because their composites with all $\lambda'_{i,k}$ agree. Thus the choices give **a unique [natural isomorphism](../../../category.md#natural-isomorphism) compatible with the chosen [categorical limit](../../../category.md#categorical-limit) [categorical cones](../../../category.md#cone-over-a-diagram)**. Without the compatibility condition, uniqueness of an arbitrary [natural isomorphism](../../../category.md#natural-isomorphism) is not asserted.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Let $M$ be a [categorical limit](../../../category.md#categorical-limit) of $L:\mathcal J\to\mathcal D$, with projections $p_j:M\to L_j$. [Set](../../../set.md) $\gamma_{i,j}=\lambda_{i,j}p_j$. The equations for the [categorical cones](../../../category.md#cone-over-a-diagram) $\lambda$ and $p$, and the defining equations for $L(v)$, show that this family is a [categorical cone](../../../category.md#cone-over-a-diagram) over $F:\mathcal I\times\mathcal J\to\mathcal D$.

For any [categorical cone](../../../category.md#cone-over-a-diagram) $x_{i,j}:X\to F(i,j)$, fix $j$. Its $\mathcal I$-legs give a unique $h_j:X\to L_j$. For $v:j\to k$, both $L(v)h_j$ and $h_k$ have composite $x_{i,k}$ with every $\lambda_{i,k}$, so they are equal. Thus the $h_j$ form a [categorical cone](../../../category.md#cone-over-a-diagram) over $L$, which factors uniquely through $h:X\to M$. The equalities $\gamma_{i,j}h=x_{i,j}$ follow. Any other such $h$ has the same composites with every $p_j$, because the projections $\lambda_{i,j}$ detect equality; uniqueness for $M$ then makes it equal to $h$. Therefore **$M$ is a [categorical limit](../../../category.md#categorical-limit) of the whole product [diagram in a category](../../../category.md#diagram-category-theory)**.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

A precise [commutation of iterated categorical limits](../../../category.md#commutation-of-iterated-categorical-limits) statement is the following. For small [categories](../../../category.md) $\mathcal I,\mathcal J$ and $F:\mathcal I\times\mathcal J\to\mathcal D$, if every column [categorical limit](../../../category.md#categorical-limit) and the resulting $\mathcal J$-limit exist, then

$$
\lim_j\lim_iF(i,j)\cong\lim_{(i,j)}F(i,j).
$$

If every row [categorical limit](../../../category.md#categorical-limit) and the resulting $\mathcal I$-limit also exist, then

$$
\boxed{\lim_j\lim_iF(i,j)\cong\lim_{(i,j)}F(i,j)\cong\lim_i\lim_jF(i,j).}
$$

Each [isomorphism](../../../algebra.md#isomorphism) is the unique one identifying all projections to $F(i,j)$. Indeed, the preceding part proves that each iterated [categorical limit](../../../category.md#categorical-limit) has the [universal property](../../../category-theory.md#universal-property) of the whole product [diagram in a category](../../../category.md#diagram-category-theory). Its uniqueness gives the canonical [isomorphism](../../../algebra.md#isomorphism). Equivalently, [categorical cones](../../../category.md#cone-over-a-diagram) with vertex $X$ over the product [diagram in a category](../../../category.md#diagram-category-theory) are exactly compatible families, indexed by $j$, of [categorical cones](../../../category.md#cone-over-a-diagram) over $F(-,j)$; regrouping the same compatibility equations cannot change their representing object. In a [complete category](../../../category.md#complete-category) all the stated existence hypotheses hold for small $\mathcal I,\mathcal J$. The theorem is about [categorical limits](../../../category.md#categorical-limit) with [categorical limits](../../../category.md#categorical-limit), and makes no unconditional claim about commuting a [categorical limit](../../../category.md#categorical-limit) with a [colimit](../../../category.md#colimit).

## 5

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Let $T:\mathcal C^{\mathrm{op}}\times\mathcal C\to\mathcal D$. A [categorical end](../../../category.md#end-of-a-functor) is an object $E$ with [morphisms](../../../algebra.md#morphism) $e_A:E\to T(A,A)$ satisfying, for every $f:A\to B$,

$$
T(1_A,f)e_A=T(f,1_B)e_B.
$$

It is universal among such families: any $x_A:X\to T(A,A)$ satisfying the same equations is uniquely $e_Ah$ for one $h:X\to E$. This is a universal [dinatural transformation](../../../category.md#dinatural-transformation) from the constant value $E$, and is written $E=\int_A T(A,A)$.

Dually a [categorical coend](../../../category.md#coend-of-a-functor) is $Q$ with [morphisms](../../../algebra.md#morphism) $j_A:T(A,A)\to Q$ satisfying

$$
j_BT(1_B,f)=j_AT(f,1_A):T(B,A)\to Q.
$$

Any family $x_A:T(A,A)\to X$ satisfying these equations is uniquely $h j_A$ for one $h:Q\to X$. Write $Q=\int^A T(A,A)$. For small $\mathcal C$, the [categorical end](../../../category.md#end-of-a-functor) can be constructed as the [equalizer](../../../category.md#equaliser) of $\prod_AT(A,A)\rightrightarrows\prod_{f:A\to B}T(A,B)$ when these objects exist. The [categorical coend](../../../category.md#coend-of-a-functor) is the [coequalizer](../../../category.md#coequalizer) of $\coprod_{f:A\to B}T(B,A)\rightrightarrows\coprod_AT(A,A)$ when those objects exist. The two [morphisms](../../../algebra.md#morphism) impose exactly the displayed equations for a [dinatural transformation](../../../category.md#dinatural-transformation).

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Working with a [small category](../../../category.md#small-category) $\mathcal C$ (or in a fixed ambient universe), for a [categorical presheaf](../../../category.md#presheaf-category-theory) $X$ and fixed $U$, apply the [categorical coend](../../../category.md#coend-of-a-functor) construction to $T(A,B)=\mathcal C(U,B)\times X(A)$. It is the quotient of the [disjoint union](../../../set-theory.md#disjoint-union) of pairs $(h:U\to W,x\in X(W))$ by the relations

$$
(fh,x)\sim(h,X(f)x)\qquad(f:W\to V,\ x\in X(V)).
$$

Define $\Phi_U([h,x])=X(h)x$. It respects every relation because $X(fh)x=X(h)X(f)x$. Define $\Psi_U(y)=[1_U,y]$. Then $\Phi_U\Psi_U(y)=y$. Conversely the relation with $f=h:U\to W$ gives $[h,x]=[1_U,X(h)x]$, so $\Psi_U\Phi_U$ is the [identity morphism](../../../algebra.md#identity-morphism). Therefore

$$
\boxed{X(U)\cong\int^W\mathcal C(U,W)\times X(W).}
$$

For $k:V\to U$, restriction on the [categorical coend](../../../category.md#coend-of-a-functor) sends $[h,x]$ to $[hk,x]$, and $\Phi_V([hk,x])=X(k)\Phi_U([h,x])$. A [natural transformation](../../../category.md#natural-transformation) $X\to Y$ likewise acts on the second coordinate and commutes with $\Phi$. Thus the [density formula for presheaves](../../../category.md#density-formula-for-presheaves) is a [natural isomorphism](../../../category.md#natural-isomorphism), not just a family of unrelated [bijections](../../../function.md#bijection).

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

The [category of elements](../../../category.md#category-of-elements) $\int X$ has objects $(W,x)$ for $x\in X(W)$, and [morphisms](../../../algebra.md#morphism) $f:(W,x)\to(V,y)$ with $X(f)y=x$. Send $(W,x)$ to the [representable presheaf](../../../category.md#representable-functor) $H_W$, and a [morphism](../../../algebra.md#morphism) $f$ to $H_\bullet(f)$. The element $x$ supplies a [natural transformation](../../../category.md#natural-transformation) $H_W\to X$ with component $h\mapsto X(h)x$, by the [Yoneda lemma](../../../category.md#yoneda-lemma). These transformations form a [cocone](../../../category.md#cocone-under-a-diagram).

Pointwise at $U$, the [colimit](../../../category.md#colimit) of this [diagram in a category](../../../category.md#diagram-category-theory) has representatives $(W,x,h:U\to W)$, with relation $(W,X(f)y,h)\sim(V,y,fh)$. These are exactly the relations of the preceding [categorical coend](../../../category.md#coend-of-a-functor). Its proved [natural isomorphism](../../../category.md#natural-isomorphism) with $X(U)$ therefore identifies the [cocone](../../../category.md#cocone-under-a-diagram) with the universal [colimit](../../../category.md#colimit) [cocone](../../../category.md#cocone-under-a-diagram). More directly, every representative equals $(U,X(h)x,1_U)$ through the [morphism](../../../algebra.md#morphism) $h:(U,X(h)x)\to(W,x)$; two representatives with the same image therefore agree. As $\mathcal C$ is small, $\int X$ is small, so this is an ordinary small [colimit](../../../category.md#colimit). Consequently

$$
\boxed{X\cong\operatorname{colim}_{(W,x)\in\int X}H_W.}
$$

## 6

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

Write the [adjunction](../../../category.md#adjoint-functors) as a [natural bijection](../../../category.md#natural-bijection) $\alpha_{C,D}:\mathcal D(FC,D)\to\mathcal C(C,GD)$. The [adjunction unit](../../../category.md#unit-of-an-adjunction) and [adjunction counit](../../../category.md#counit-of-an-adjunction) are defined by

$$
\eta_C=\alpha_{C,FC}(1_{FC}),\qquad\varepsilon_D=\alpha^{-1}_{GD,D}(1_{GD}).
$$

[Naturality](../../../category.md#naturality) of $\alpha$ implies $GF(u)\eta_C=\eta_{C'}u$ for $u:C\to C'$ and $v\varepsilon_D=\varepsilon_{D'}FG(v)$ for $v:D\to D'$, so these are [natural transformations](../../../category.md#natural-transformation) $1_{\mathcal C}\to GF$ and $FG\to1_{\mathcal D}$. More explicitly, [naturality](../../../category.md#naturality) at $f:FC\to D$ and $g:C\to GD$ gives the two transpose formulas

$$
\alpha(f)=G(f)\eta_C,\qquad\alpha^{-1}(g)=\varepsilon_DF(g).
$$

These formulas will also prove the [triangle identities for an adjunction](../../../category.md#triangle-identities-for-an-adjunction).

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

Using the transpose formulas of the preceding part,

$$
\varepsilon_{FC}F(\eta_C)=\alpha^{-1}_{C,FC}(\alpha_{C,FC}(1_{FC}))=1_{FC}.
$$

Similarly,

$$
G(\varepsilon_D)\eta_{GD}=\alpha_{GD,D}(\alpha^{-1}_{GD,D}(1_{GD}))=1_{GD}.
$$

Thus the [adjunction unit](../../../category.md#unit-of-an-adjunction) and [adjunction counit](../../../category.md#counit-of-an-adjunction) satisfy **both [triangle identities for an adjunction](../../../category.md#triangle-identities-for-an-adjunction)**,

$$
\boxed{\varepsilon_F\circ F\eta=1_F,\qquad G\varepsilon\circ\eta_G=1_G.}
$$

<h3 id="6/iii">iii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6/iii)

Given the two [natural transformations](../../../category.md#natural-transformation), define

$$
\alpha(f)=Gf\,\eta_C,\qquad\beta(g)=\varepsilon_DFg.
$$

[Naturality](../../../category.md#naturality) of $\eta$ and the second [triangle identity for an adjunction](../../../category.md#triangle-identities-for-an-adjunction) give

$$
\alpha\beta(g)=G\varepsilon_D\,GFg\,\eta_C=G\varepsilon_D\,\eta_{GD}\,g=g.
$$

[Naturality](../../../category.md#naturality) of $\varepsilon$ and the first [triangle identity for an adjunction](../../../category.md#triangle-identities-for-an-adjunction) give

$$
\beta\alpha(f)=\varepsilon_D\,FGf\,F\eta_C=f\,\varepsilon_{FC}\,F\eta_C=f.
$$

The maps are natural in $C,D$, since the defining compositions commute with precomposition in $C$ and postcomposition in $D$ by [naturality](../../../category.md#naturality) of $\eta,\varepsilon$. They therefore define an [adjunction](../../../category.md#adjoint-functors) $F\dashv G$. Their values on [identity morphisms](../../../algebra.md#identity-morphism) recover precisely $\eta,\varepsilon$. Conversely any [adjunction](../../../category.md#adjoint-functors) with these [unit and counit of an adjunction](../../../category.md#unit-and-counit-of-an-adjunction) must have the same transpose formulas, so it is **unique with the prescribed unit and counit**.

## 7

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

A [poset](../../../set.md#partially-ordered-set) $P$ becomes a [category](../../../category.md) with the elements of $P$ as objects and exactly one [morphism](../../../algebra.md#morphism) $x\to y$ when $x\leq y$, with no [morphism](../../../algebra.md#morphism) otherwise. Reflexivity supplies the [identity morphisms](../../../algebra.md#identity-morphism) and transitivity supplies [composition in a category](../../../category.md#composition-in-a-category); uniqueness of [morphisms](../../../algebra.md#morphism) proves associativity. A [functor](../../../category.md#functor) $f:P\to Q$ is exactly a [monotone function](../../../calculus.md#monotonic-function): it must send $x\leq y$ to $f(x)\leq f(y)$, and this condition suffices because all the required [morphisms](../../../algebra.md#morphism) are unique. Antisymmetry says that isomorphic objects of this [category](../../../category.md) are equal.

<h3 id="7/i">i</h3>

↑ **Parent:** [7](#7)

<h4 id="7/i/solution">Solution</h4>

↑ **Parent:** [I](#7/i)

Each [hom-set](../../../category.md#hom-set) in a [poset](../../../set.md#partially-ordered-set) is either empty or a singleton. Thus a [natural bijection](../../../category.md#natural-bijection) $Y(fx,y)\cong X(x,gy)$ is precisely the condition

$$
\boxed{f(x)\leq y\iff x\leq g(y).}
$$

The [naturality](../../../category.md#naturality) squares commute automatically, because maps between the relevant singleton [hom-sets](../../../category.md#hom-set) are unique. This is a [Galois connection](../../../category.md#galois-connection). Equivalently, the [adjunction unit](../../../category.md#unit-of-an-adjunction) and [adjunction counit](../../../category.md#counit-of-an-adjunction) are the inequalities $x\leq gf(x)$ and $fg(y)\leq y$. These inequalities imply the displayed equivalence: $f(x)\leq y$ gives $x\leq gf(x)\leq g(y)$, and $x\leq g(y)$ gives $f(x)\leq fg(y)\leq y$.

<h3 id="7/ii">ii</h3>

↑ **Parent:** [7](#7)

<h4 id="7/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7/ii)

The two [adjoints of inverse image on power sets](../../../category.md#adjoints-of-inverse-image-on-power-sets) are

$$
\boxed{\exists_p(U)=p(U),\qquad\forall_p(U)=\{b\in B:p^{-1}(\{b\})\subseteq U\}.}
$$

These maps and $p^*(V)=p^{-1}(V)$ are [monotone functions](../../../calculus.md#monotonic-function) on the inclusion-ordered [power sets](../../../set.md#power-set). For $U\subseteq A$ and $V\subseteq B$,

$$
p(U)\subseteq V\iff U\subseteq p^{-1}(V),\qquad p^{-1}(V)\subseteq U\iff V\subseteq\forall_p(U).
$$

The first equivalence follows by following each element of $U$ through $p$. For the second, every [fiber](../../../function.md#fiber-of-a-function) over $b\in V$ must lie in $U$, which is precisely the defining condition for $b\in\forall_p(U)$. These are the two [Galois connections](../../../category.md#galois-connection), proving $\exists_p\dashv p^*\dashv\forall_p$. In particular, a point outside $p(A)$ has an empty [fiber](../../../function.md#fiber-of-a-function) and belongs to $\forall_p(U)$ even when $U$ is empty; omitting this case would give an incorrect [right adjoint](../../../category.md#adjoint-functors).

<h3 id="7/iii">iii</h3>

↑ **Parent:** [7](#7)

<h4 id="7/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#7/iii)

For a [presheaf of sets on a topological space](../../../algebraic-geometry.md#presheaf-of-sets-on-a-topological-space) $P$, define $LP=P(\varnothing)$ and $RP=P(S)$. Then the [adjoints to constant presheaves on open sets](../../../category.md#adjoints-to-constant-presheaves-on-open-sets) are

$$
\boxed{\operatorname{ev}_{\varnothing}\dashv\Delta\dashv\operatorname{ev}_S.}
$$

To prove the first [adjunction](../../../category.md#adjoint-functors), a [natural transformation](../../../category.md#natural-transformation) $a:P\to\Delta A$ must satisfy $a_U=a_{\varnothing}\circ\operatorname{res}_{U,\varnothing}$ by [naturality](../../../category.md#naturality) at the inclusion $\varnothing\subseteq U$. Hence it is uniquely determined by a [function](../../../function.md) $P(\varnothing)\to A$. Every such [function](../../../function.md) defines a [natural transformation](../../../category.md#natural-transformation) by this formula, because restriction maps compose. This gives $\operatorname{Nat}(P,\Delta A)\cong\mathbf{Set}(P(\varnothing),A)$.

For the second [adjunction](../../../category.md#adjoint-functors), a [natural transformation](../../../category.md#natural-transformation) $b:\Delta A\to P$ satisfies $b_U=\operatorname{res}_{S,U}\circ b_S$, so it is uniquely determined by a [function](../../../function.md) $A\to P(S)$. Every such [function](../../../function.md) defines the remaining components by restriction, giving $\operatorname{Nat}(\Delta A,P)\cong\mathbf{Set}(A,P(S))$. Evaluation acts on [presheaf morphisms](../../../algebraic-geometry.md#morphism-of-presheaves) componentwise, so these object assignments are indeed [functors](../../../category.md#functor). The use of $P(\varnothing)$ is essential: a [constant presheaf of sets](../../../algebraic-geometry.md#constant-presheaf-of-sets) has value $A$ there, whereas a [sheaf](../../../algebraic-geometry.md#sheaf-mathematics) has a singleton value there. No sheaf condition is imposed in this question.

## 8

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="8/solution">Solution</h3>

↑ **Parent:** [8](#8)

For $c\in\mathcal C$ and $d\in\mathcal D$, define maps of [hom-sets](../../../category.md#hom-set)

$$
\alpha(f)=Gf\,\eta_c:\mathcal D(Fc,d)\to\mathcal C(c,Gd),\qquad
\beta(g)=\varepsilon_dFg:\mathcal C(c,Gd)\to\mathcal D(Fc,d).
$$

They are natural in $c,d$, using [naturality](../../../category.md#naturality) of $\eta,\varepsilon$. The one supplied [triangle identity for an adjunction](../../../category.md#triangle-identities-for-an-adjunction) gives

$$
\alpha\beta(g)=G\varepsilon_d\,GFg\,\eta_c=G\varepsilon_d\,\eta_{Gd}g=g.
$$

[Naturality](../../../category.md#naturality) of $\varepsilon$ also gives

$$
\beta\alpha(f)=\varepsilon_dFGfF\eta_c=f\varepsilon_{Fc}F\eta_c=f e_c,
\qquad e_c=\varepsilon_{Fc}F\eta_c.
$$

Since $\alpha\beta=1$, the composite $\beta\alpha$ is idempotent. Evaluating its equation $(\beta\alpha)^2=\beta\alpha$ on $f=1_{Fc}$ gives $e_c^2=e_c$. As $e$ is a composite of [natural transformations](../../../category.md#natural-transformation), this proves that **$e$ is an idempotent in the [functor category](../../../category.md#functor-category)**, including the required [naturality](../../../category.md#naturality).

Suppose this [one-triangle adjunction idempotent](../../../category.md#one-triangle-adjunction-idempotent) splits as [natural transformations](../../../category.md#natural-transformation) $F\xrightarrow r H\xrightarrow i F$ with $ri=1_H$ and $ir=e$. The maps $h\mapsto hr$ and $f\mapsto fi$ give inverse [bijections](../../../function.md#bijection) between $\mathcal D(Hc,d)$ and the [subset](../../../set.md#subset) of $\mathcal D(Fc,d)$ consisting of maps with $fe_c=f$. Indeed $(hr)e_c=hrir=hr$, $(hr)i=h$, and $(fi)r=fe_c=f$. The maps $\alpha,\beta$ give inverse [bijections](../../../function.md#bijection) between that [subset](../../../set.md#subset) and $\mathcal C(c,Gd)$, since $\beta\alpha(f)=fe_c$ and $\alpha\beta=1$. Combining them gives the [natural bijection](../../../category.md#natural-bijection)

$$
\mathcal D(Hc,d)\cong\mathcal C(c,Gd),\qquad h\longmapsto G(hr)\eta_c,
$$

with inverse $g\mapsto\varepsilon_dF(g)i_c$. Hence $H\dashv G$. Its [adjunction unit](../../../category.md#unit-of-an-adjunction) is $Gr\,\eta$ and its [adjunction counit](../../../category.md#counit-of-an-adjunction) is $\varepsilon\,i_G$.

Conversely, suppose $H\dashv G$, with [natural bijection](../../../category.md#natural-bijection) $\theta:\mathcal D(Hc,d)\cong\mathcal C(c,Gd)$. Set $\tau=\theta^{-1}\alpha$ and $\sigma=\beta\theta$. Then $\tau\sigma=1$ and $\sigma\tau(f)=fe_c$. By the covariant [Yoneda lemma](../../../category.md#yoneda-lemma), the transformation $\tau:\mathcal D(Fc,-)\to\mathcal D(Hc,-)$ is precomposition with a unique [morphism](../../../algebra.md#morphism) $i_c:Hc\to Fc$, and $\sigma$ is precomposition with a unique [morphism](../../../algebra.md#morphism) $r_c:Fc\to Hc$. The equation $\tau\sigma=1$ evaluated at $1_{Hc}$ gives $r_ci_c=1_{Hc}$; the equation $\sigma\tau(f)=fe_c$ evaluated at $1_{Fc}$ gives $i_cr_c=e_c$. [Naturality](../../../category.md#naturality) in $c$ of $\tau,\sigma$ implies, again by the same [Yoneda lemma](../../../category.md#yoneda-lemma), that $i,r$ are [natural transformations](../../../category.md#natural-transformation). Thus they split $e$ in the whole [functor category](../../../category.md#functor-category), rather than merely at individual objects. We have proved

$$
\boxed{G\text{ has a left adjoint}\iff e=\varepsilon_FF\eta\text{ splits in }[\mathcal C,\mathcal D].}
$$

## 9

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="9/solution">Solution</h3>

↑ **Parent:** [9](#9)

For the general alternative, let $G:\mathcal D\to\mathcal C$ be a [functor](../../../category.md#functor) between [locally small categories](../../../category.md#locally-small-category), with $\mathcal D$ a [complete category](../../../category.md#complete-category). The [Freyd general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem) says that $G$ has a [left adjoint](../../../category.md#adjoint-functors) if and only if it preserves small [categorical limits](../../../category.md#categorical-limit) and satisfies the [solution-set condition](../../../category.md#solution-set-condition). Explicitly, for every $c\in\mathcal C$, there must be a [set](../../../set.md) of [morphisms](../../../algebra.md#morphism) $x_j:c\to Gd_j$ such that every $x:c\to Gd$ has the form $G(h)x_j$ for some $j$ and $h:d_j\to d$. Equivalently, each [comma category](../../../category.md#comma-category) $(c\downarrow G)$ has a [weakly initial set](../../../category.md#weakly-initial-set).

We prove the [initial-object lemma for complete categories with a weakly initial set](../../../category.md#initial-object-lemma-for-complete-categories-with-a-weakly-initial-set). Let $\mathcal E$ be a [locally small category](../../../category.md#locally-small-category) which is complete and has a [weakly initial set](../../../category.md#weakly-initial-set) $(w_j)_{j\in J}$. Its [product in a category](../../../category.md#product-category-theory) $p=\prod_jw_j$ is weakly initial: for each $z$, choose a [morphism](../../../algebra.md#morphism) $w_j\to z$ and compose with the projection $p\to w_j$. The [hom-set](../../../category.md#hom-set) $\mathcal E(p,p)$ is a [set](../../../set.md). Form $e:i\to p$ equalizing every [endomorphism](../../../algebra.md#endomorphism) of $p$ with $1_p$, by taking the [equalizer](../../../category.md#equaliser) of the two [morphisms](../../../algebra.md#morphism)

$$
p\rightrightarrows\prod_{v\in\mathcal E(p,p)}p,
$$

whose $v$-coordinates are $v$ and $1_p$. Then $ve=e$ for every [endomorphism](../../../algebra.md#endomorphism) $v$, and $e$ is monic. There is a [morphism](../../../algebra.md#morphism) $i\to z$ for every $z$, by composing $e$ with a weakly initial [morphism](../../../algebra.md#morphism) out of $p$.

To prove uniqueness, let $u,v:i\rightrightarrows z$ and take their [equalizer](../../../category.md#equaliser) $q:w\to i$. Weak initiality of $p$ gives $a:p\to w$. The composite $eqa:p\to p$ is an [endomorphism](../../../algebra.md#endomorphism), so $eqa e=e$. Cancel the [monomorphism](../../../category.md#monomorphism) $e$ to obtain $qa e=1_i$. Thus $q$ is both monic and split epic, hence an [isomorphism](../../../algebra.md#isomorphism): if $qk=1$, cancellation from $qkq=q$ gives $kq=1$. Since $uq=vq$, it follows that $u=v$. Therefore $i$ is an [initial object](../../../category.md#initial-object), proving the lemma fully.

Now assume [categorical limit](../../../category.md#categorical-limit) preservation and the [solution-set condition](../../../category.md#solution-set-condition). The [comma category](../../../category.md#comma-category) $(c\downarrow G)$ is locally small. It is complete: for a small [diagram in a category](../../../category.md#diagram-category-theory) $(d_j,x_j)$, take its underlying [categorical limit](../../../category.md#categorical-limit) $l$ in $\mathcal D$. Since $G$ preserves this [categorical limit](../../../category.md#categorical-limit), the compatible $x_j:c\to Gd_j$ give a unique $x:c\to Gl$. The same [universal property](../../../category-theory.md#universal-property) shows that $(l,x)$ is the [categorical limit](../../../category.md#categorical-limit) in the [comma category](../../../category.md#comma-category). Its [weakly initial set](../../../category.md#weakly-initial-set) and the proved lemma therefore supply an [initial object](../../../category.md#initial-object) $(Fc,\eta_c)$. For $t:c\to c'$, its [universal property](../../../category-theory.md#universal-property) defines a unique $Ft:Fc\to Fc'$ with $G(Ft)\eta_c=\eta_{c'}t$. Uniqueness proves the [identity morphism](../../../algebra.md#identity-morphism) and [composition in a category](../../../category.md#composition-in-a-category) laws and the [naturality](../../../category.md#naturality) of $\eta$. The same [universal property](../../../category-theory.md#universal-property) gives the [natural bijection](../../../category.md#natural-bijection) $\mathcal D(Fc,d)\cong\mathcal C(c,Gd)$, so $F\dashv G$.

For necessity, an [adjunction](../../../category.md#adjoint-functors) $F\dashv G$ supplies the singleton [weakly initial set](../../../category.md#weakly-initial-set) $(Fc,\eta_c)$ at $c$. It also proves that $G$ preserves [categorical limits](../../../category.md#categorical-limit): maps $c\to Gd$ correspond to maps $Fc\to d$, and compatible families of the latter factor uniquely through any [categorical limit](../../../category.md#categorical-limit) in $\mathcal D$. Hence the image [categorical cone](../../../category.md#cone-over-a-diagram) under $G$ has the required [universal property](../../../category-theory.md#universal-property). This proves both directions of the general alternative.

For the special alternative, the [limit form of the special adjoint functor theorem](../../../category.md#limit-form-of-the-special-adjoint-functor-theorem) says: if $\mathcal D$ is complete, locally small and [well-powered](../../../category.md#well-powered-category), with a [small cogenerating family](../../../category.md#cogenerating-set) $(Q_i)_{i\in I}$, and $\mathcal C$ is locally small, then $G:\mathcal D\to\mathcal C$ has a [left adjoint](../../../category.md#adjoint-functors) exactly when it preserves small [categorical limits](../../../category.md#categorical-limit). A [cogenerating set](../../../category.md#cogenerating-set) means that unequal parallel [morphisms](../../../algebra.md#morphism) $u,v:X\rightrightarrows Y$ are distinguished by some [morphism](../../../algebra.md#morphism) $Y\to Q_i$. We prove the needed [solution-set condition](../../../category.md#solution-set-condition), so that the general theorem applies.

Fix $x:c\to Gd$. A supporting [subobject](../../../category.md#subobject) of $d$ is a [monomorphism](../../../category.md#monomorphism) $m:d'\to d$ through whose image under $G$ the [morphism](../../../algebra.md#morphism) $x$ factors. There is at least one, namely $1_d$. Because $\mathcal D$ is [well-powered](../../../category.md#well-powered-category), choose a [set](../../../set.md) of representatives of all these supporting [subobjects](../../../category.md#subobject). A limit-preserving [functor](../../../category.md#functor) preserves [monomorphisms](../../../category.md#monomorphism): a map is monic exactly when its diagonal into its self-[pullback in a category](../../../category.md#pullback-category-theory) is an [isomorphism](../../../algebra.md#isomorphism), and both the [pullback in a category](../../../category.md#pullback-category-theory) and this [isomorphism](../../../algebra.md#isomorphism) are preserved. Consequently each factorization of $x$ through $Gm$ is unique. Form the [intersection of subobjects](../../../category.md#intersection-of-subobjects) of the supporting representatives, as a wide [pullback in a category](../../../category.md#pullback-category-theory) over $d$. The unique lifts of $x$ are compatible and, since $G$ preserves that [categorical limit](../../../category.md#categorical-limit), they give a factorization

$$
x=G(m_0)x_0,\qquad m_0:d_0\hookrightarrow d,\quad x_0:c\to Gd_0.
$$

This is a [minimal supported subobject](../../../category.md#minimal-supported-subobject). More explicitly, if $q:e\hookrightarrow d_0$ also supports $x_0$, then $m_0q$ is one of the supporting [subobjects](../../../category.md#subobject) of $d$. The intersection therefore factors through $m_0q$, giving $r:d_0\to e$ with $m_0qr=m_0$. Monicity of $m_0$ gives $qr=1_{d_0}$; monicity of $q$ then makes $q$ invertible.

For any $u,v:d_0\to Q_i$, if $G(u)x_0=G(v)x_0$, the [equalizer](../../../category.md#equaliser) of $u,v$ supports $x_0$, because $G$ preserves that [equalizer](../../../category.md#equaliser). Minimality makes it invertible, so $u=v$. We have therefore obtained [injective functions](../../../algebra.md#injective-function)

$$
\mathcal D(d_0,Q_i)\longrightarrow\mathcal C(c,GQ_i),\qquad u\longmapsto G(u)x_0.
$$

Let $S_i$ be the realized image [subset](../../../set.md#subset) of the fixed [set](../../../set.md) $\mathcal C(c,GQ_i)$. Use the unique [morphism](../../../algebra.md#morphism) corresponding to each $s\in S_i$ to form the [evaluation embedding into cogenerator products](../../../category.md#evaluation-embedding-into-cogenerator-products)

$$
d_0\longrightarrow P_S=\prod_{i\in I}\prod_{s\in S_i}Q_i.
$$

This [morphism](../../../algebra.md#morphism) is monic: if two [morphisms](../../../algebra.md#morphism) into $d_0$ have identical product composites, every [morphism](../../../algebra.md#morphism) from $d_0$ to every $Q_i$ gives identical composites, and the cogenerating property makes the two [morphisms](../../../algebra.md#morphism) equal. There is only a [set](../../../set.md) of possible families of [subsets](../../../set.md#subset) $(S_i)$, and hence a [set](../../../set.md) of possible products $P_S$. Each has only a [set](../../../set.md) of [subobjects](../../../category.md#subobject) by well-poweredness, and each chosen [subobject](../../../category.md#subobject) $a$ has only a [set](../../../set.md) of [morphisms](../../../algebra.md#morphism) $c\to Ga$ by local smallness. Take all these pairs $(a,z:c\to Ga)$ as a [weakly initial set](../../../category.md#weakly-initial-set). Every original $(d,x)$ receives a [morphism](../../../algebra.md#morphism) from a pair representing its $(d_0,x_0)$, through $m_0$. Thus the [set](../../../set.md) is weakly initial in $(c\downarrow G)$.

The general theorem now supplies a [left adjoint](../../../category.md#adjoint-functors). Necessity again follows from preservation of [categorical limits](../../../category.md#categorical-limit) by a [right adjoint](../../../category.md#adjoint-functors). This proves the special alternative, including its size argument. Using only the realized [subsets](../../../set.md#subset) $S_i$ avoids assuming that an arbitrary object admits a [morphism](../../../algebra.md#morphism) into every cogenerator. **Both adjoint [functor](../../../category.md#functor) theorem alternatives are proved.**

## 10

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="10/i">i</h3>

↑ **Parent:** [10](#10)

<h4 id="10/i/solution">Solution</h4>

↑ **Parent:** [I](#10/i)

A [monad](../../../category-theory.md#monad) on $\mathcal C$ consists of an [endofunctor](../../../category.md#endofunctor) $T$ and [natural transformations](../../../category.md#natural-transformation) $\eta:1\to T$, $\mu:T^2\to T$ satisfying, at every object $A$,

$$
\mu_A T\mu_A=\mu_A\mu_{TA},\qquad\mu_A\eta_{TA}=1_{TA}=\mu_A T\eta_A.
$$

These are the associativity and unit laws. An [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) is $(A,a:TA\to A)$ with

$$
a\eta_A=1_A,\qquad aT a=a\mu_A.
$$

A [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad) $h:(A,a)\to(B,b)$ is a [morphism](../../../algebra.md#morphism) $h:A\to B$ satisfying $ha=bTh$. [Identity morphisms](../../../algebra.md#identity-morphism) satisfy this equation, and if $h,k$ satisfy it, then $kha=kbTh=cTkTh=cT(kh)$. Hence these objects and [morphisms](../../../algebra.md#morphism) form the [Eilenberg-Moore category](../../../category-theory.md#eilenberg-moore-category) $\mathcal C^T$, with the [forgetful functor](../../../category.md#forgetful-functor) $U(A,a)=A$ and $Uh=h$.

<h3 id="10/ii">ii</h3>

↑ **Parent:** [10](#10)

<h4 id="10/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10/ii)

Define the [free algebra functor](../../../category-theory.md#free-algebra-functor) $F^T$ by $F^T X=(TX,\mu_X)$ and $F^T f=Tf$. The [monad](../../../category-theory.md#monad) laws make $\mu_X$ an algebra action, and [naturality](../../../category.md#naturality) of $\mu$ makes $Tf$ a [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad). For an [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) $(A,a)$, define

$$
\mathcal C^T(F^TX,(A,a))\longrightarrow\mathcal C(X,A),\quad h\longmapsto h\eta_X,
$$

with proposed inverse $g\mapsto aTg$. This inverse is a [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad), since

$$
(aTg)\mu_X=a\mu_A T^2g=aTa\,T^2g=aT(aTg).
$$

One composite is $aTg\eta_X=a\eta_Ag=g$. For a [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad) $h$, the other is $aT(h\eta_X)=aTh\,T\eta_X=h\mu_X T\eta_X=h$. Both formulas commute with [composition in a category](../../../category.md#composition-in-a-category) in $X$ and with [monad algebra morphisms](../../../category-theory.md#morphism-of-algebras-for-a-monad) in $(A,a)$, so the [bijection](../../../function.md#bijection) is natural. Thus

$$
\boxed{F^T\dashv U.}
$$

<h3 id="10/iii">iii</h3>

↑ **Parent:** [10](#10)

<h4 id="10/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#10/iii)

For $(A,a)$, consider the [reflexive free-algebra presentation of a monad algebra](../../../category-theory.md#reflexive-free-algebra-presentation-of-a-monad-algebra)

$$
F^T(TA)\ \substack{\xrightarrow{\mu_A}\\[-2pt]\xrightarrow[T a]{}}\ F^T(A)\xrightarrow{a}(A,a).
$$

Both parallel [morphisms](../../../algebra.md#morphism) are [monad algebra morphisms](../../../category-theory.md#morphism-of-algebras-for-a-monad): $\mu_A$ satisfies the [monad](../../../category-theory.md#monad) associativity law, while $Ta$ is the image under $F^T$ of $a$. The map $a$ is a [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad) because $a\mu_A=aTa$, and the same equation says it equalizes the pair.

Suppose $h:F^T(A)\to(B,b)$ is a [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad) with $h\mu_A=hTa$. Put $k=h\eta_A:A\to B$. [Naturality](../../../category.md#naturality) of $\eta$ and the unit law give

$$
ka=h\eta_Aa=hTa\eta_{TA}=h\mu_A\eta_{TA}=h.
$$

Moreover, since $h$ is a [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad),

$$
bTk=bTh\,T\eta_A=h\mu_A T\eta_A=h=ka.
$$

Thus $k$ is a [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad) and factors $h$ through $a$. If $k'a=h$, then $k'=k'a\eta_A=h\eta_A=k$, proving uniqueness. Therefore **every [monad](../../../category-theory.md#monad) algebra is the stated [coequalizer](../../../category.md#coequalizer) of free algebras**.

The underlying fork is a [split coequalizer](../../../category.md#split-coequalizer): take $q=a$, $s=\eta_A$ and $t=\eta_{TA}$. Then $qs=1_A$, $\mu_A t=1_{TA}$, and $(Ta)t=sa$. Its splitting maps need not be [monad algebra morphisms](../../../category-theory.md#morphism-of-algebras-for-a-monad); the preceding argument separately proves the [coequalizer](../../../category.md#coequalizer) in $\mathcal C^T$.

## 11

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="11/i">i</h3>

↑ **Parent:** [11](#11)

<h4 id="11/i/solution">Solution</h4>

↑ **Parent:** [I](#11/i)

For $G:\mathcal D\to\mathcal C$, a [functor-split coequalizer pair](../../../category.md#functor-split-coequalizer-pair) is a parallel pair $f,g:Y\rightrightarrows Z$ such that its image admits a [split coequalizer](../../../category.md#split-coequalizer) in $\mathcal C$. In one orientation this means [morphisms](../../../algebra.md#morphism) $q:GZ\to Q$, $s:Q\to GZ$ and $t:GZ\to GY$ satisfy

$$
qGf=qGg,\quad qs=1_Q,\quad (Gf)t=1_{GZ},\quad(Gg)t=sq.
$$

These equations prove that $q$ is a [coequalizer](../../../category.md#coequalizer): if $hGf=hGg$, then $h=hGf\,t=hGg\,t=hsq$, so $hs$ factors $h$; uniqueness follows from $qs=1$. They remain true under every [functor](../../../category.md#functor), making a [split coequalizer](../../../category.md#split-coequalizer) an absolute [colimit](../../../category.md#colimit).

To say that $G$ reflects such [coequalizers](../../../category.md#coequalizer) means that any fork $Y\rightrightarrows Z\xrightarrow{p}W$ in $\mathcal D$ whose image is a [split coequalizer](../../../category.md#split-coequalizer) is itself a [coequalizer](../../../category.md#coequalizer) in $\mathcal D$. This is a reflection assertion about an existing fork; it does not by itself require lifting every split fork from $\mathcal C$, or creating its splitting maps in $\mathcal D$.

<h3 id="11/ii">ii</h3>

↑ **Parent:** [11](#11)

<h4 id="11/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11/ii)

Write the [adjunction unit](../../../category.md#unit-of-an-adjunction) and [adjunction counit](../../../category.md#counit-of-an-adjunction) of $F\dashv G$ as $\eta,\varepsilon$. Its induced [monad](../../../category-theory.md#monad) is $T=GF$, with multiplication $\mu=G\varepsilon_F$. The [Eilenberg-Moore comparison functor](../../../category-theory.md#eilenberg-moore-comparison-functor) is

$$
K(d)=(Gd,a_d),\qquad a_d=G\varepsilon_d:T(Gd)\to Gd,\qquad K(h)=Gh.
$$

The unit law for $a_d$ is $G\varepsilon_d\eta_{Gd}=1_{Gd}$, a [triangle identity for an adjunction](../../../category.md#triangle-identities-for-an-adjunction). [Naturality](../../../category.md#naturality) of $\varepsilon$ at $\varepsilon_d$ gives $\varepsilon_dFG\varepsilon_d=\varepsilon_d\varepsilon_{FGd}$; applying $G$ gives $a_dTa_d=a_d\mu_{Gd}$. [Naturality](../../../category.md#naturality) at $h$ gives the [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad) equation for $Gh$. Thus $K$ is well-defined.

For each $d$, consider the fork in $\mathcal D$

$$
FGFGd\ \substack{\xrightarrow{\varepsilon_{FGd}}\\[-2pt]\xrightarrow[FG\varepsilon_d]{}}\ FGd\xrightarrow{\varepsilon_d}d.
$$

It commutes by the [naturality](../../../category.md#naturality) equation just used. Its image under $G$ is the fork $T^2(Gd)\rightrightarrows T(Gd)\to Gd$ of the preceding question, with parallel [morphisms](../../../algebra.md#morphism) $\mu_{Gd},Ta_d$ and final map $a_d$. It is split using $s=\eta_{Gd}$ and $t=\eta_{T(Gd)}$. By the assumed reflection, **$\varepsilon_d$ is the [coequalizer](../../../category.md#coequalizer) of this pair in $\mathcal D$**.

For faithfulness, if $Gh=Gk$ for $h,k:d\to e$, [naturality](../../../category.md#naturality) gives $h\varepsilon_d=\varepsilon_eFGh=\varepsilon_eFGk=k\varepsilon_d$. A [coequalizer](../../../category.md#coequalizer) is an [epimorphism](../../../category.md#epimorphism), so $h=k$.

For fullness, let $u:K(d)\to K(e)$ be a [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad). Thus $u:Gd\to Ge$ satisfies $u a_d=a_eTu$. [Set](../../../set.md) $v=\varepsilon_eF u:FGd\to e$. We verify explicitly that $v$ equalizes the two [morphisms](../../../algebra.md#morphism) of the displayed fork. The [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad) equation gives

$$
vFG\varepsilon_d=\varepsilon_eF(uG\varepsilon_d)
=\varepsilon_eFG\varepsilon_e\,FGF u.
$$

[Naturality](../../../category.md#naturality) of $\varepsilon$ first at $Fu$ and then at $\varepsilon_e$ gives

$$
v\varepsilon_{FGd}=\varepsilon_e\varepsilon_{FGe}\,FGF u
=\varepsilon_eFG\varepsilon_e\,FGF u.
$$

The [coequalizer](../../../category.md#coequalizer) therefore supplies a unique $h:d\to e$ with $h\varepsilon_d=v$. Applying $G$ yields $Gh\,a_d=Gv=a_eTu=u a_d$. The map $a_d$ is split epic with section $\eta_{Gd}$, so cancellation gives $Gh=u$. This proves fullness, and the earlier cancellation proves faithfulness. Hence

$$
\boxed{K:\mathcal D\to\mathcal C^T\text{ is full and faithful}.}
$$

No claim that $K$ is essentially surjective is needed; that stronger conclusion needs the corresponding existence hypotheses.

## 12

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="12/i">i</h3>

↑ **Parent:** [12](#12)

<h4 id="12/i/solution">Solution</h4>

↑ **Parent:** [I](#12/i)

A [monoidal category](../../../category-theory.md#monoidal-category) consists of a [category](../../../category.md) $\mathcal C$, a [bifunctor](../../../category.md#bifunctor) $\otimes:\mathcal C\times\mathcal C\to\mathcal C$, a [monoidal unit object](../../../category-theory.md#monoidal-unit-object) $I$, and [natural isomorphisms](../../../category.md#natural-isomorphism)

$$
\alpha_{A,B,C}:(A\otimes B)\otimes C\to A\otimes(B\otimes C),\quad
\lambda_A:I\otimes A\to A,\quad\rho_A:A\otimes I\to A.
$$

The [associator](../../../category-theory.md#associator) obeys the [pentagon identity for a monoidal category](../../../category-theory.md#pentagon-identity-for-a-monoidal-category),

$$
\alpha_{A,B,C\otimes D}\,\alpha_{A\otimes B,C,D}
=(1_A\otimes\alpha_{B,C,D})\,\alpha_{A,B\otimes C,D}\,(\alpha_{A,B,C}\otimes1_D),
$$

and the [unitors](../../../category-theory.md#unitor) obey the [triangle identity for a monoidal category](../../../category-theory.md#triangle-identity-for-a-monoidal-category),

$$
(1_A\otimes\lambda_B)\,\alpha_{A,I,B}=\rho_A\otimes1_B.
$$

[Composition in a category](../../../category.md#composition-in-a-category) here acts from right to left. The first equation compares two paths from $((A\otimes B)\otimes C)\otimes D$ to $A\otimes(B\otimes(C\otimes D))$; the second compares two ways of removing the intervening unit.

It is precisely a [bicategory](../../../category-theory.md#bicategory) with one object $*$. The [category](../../../category.md) $\mathcal B(*,*)$ is $\mathcal C$: its objects are the 1-morphisms and its [morphisms](../../../algebra.md#morphism) are the 2-morphisms. Horizontal [composition in a category](../../../category.md#composition-in-a-category) is $\otimes$, the identity 1-morphism is $I$, and the [associator](../../../category-theory.md#associator) and [unitors](../../../category-theory.md#unitor) give the weak associativity and unit constraints. Vertical [composition in a category](../../../category.md#composition-in-a-category) is ordinary [composition in a category](../../../category.md#composition-in-a-category) in $\mathcal C$; the interchange law follows because $\otimes$ is a [bifunctor](../../../category.md#bifunctor). The bicategory pentagon and triangle axioms are exactly the two equations above. Conversely the sole hom-category of any one-object [bicategory](../../../category-theory.md#bicategory) gives these data, with the convention that horizontal [composition in a category](../../../category.md#composition-in-a-category) uses the indicated ordering of tensor factors.

<h3 id="12/ii">ii</h3>

↑ **Parent:** [12](#12)

<h4 id="12/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#12/ii)

For the [Category of sets](../../../category.md#category-of-sets), take the [monoidal tensor product](../../../category-theory.md#monoidal-tensor-product) to be the [Cartesian product](../../../set-theory.md#cartesian-product), $A\otimes B=A\times B$, with unit a singleton $1$. On [morphisms](../../../algebra.md#morphism) use $(f\times g)(a,b)=(f(a),g(b))$. Define the [associator](../../../category-theory.md#associator) by $((a,b),c)\mapsto(a,(b,c))$ and the [unitors](../../../category-theory.md#unitor) by $(*,a)\mapsto a$ and $(a,*)\mapsto a$. These are [natural isomorphisms](../../../category.md#natural-isomorphism), with inverses obtained by rebracketing or adjoining $*$. Both paths in the pentagon send $(((a,b),c),d)$ to $(a,(b,(c,d)))$, and both paths in the triangle send $((a,*),b)$ to $(a,b)$. This proves the axioms elementwise.

There is a second structure: use [disjoint union](../../../set-theory.md#disjoint-union) $A\amalg B$ and unit $\varnothing$. Define the [associator](../../../category-theory.md#associator) by preserving each element and its summand while changing the nested tags, and define the [unitors](../../../category-theory.md#unitor) by removing the empty summand. These are natural and invertible. In the pentagon, either path takes an element in any of the four summands to that same element in the same summand of $A\amalg(B\amalg(C\amalg D))$; the triangle removes an empty intermediate summand on either path. Thus both axioms hold.

These [product and coproduct monoidal structures on sets](../../../category-theory.md#product-and-coproduct-monoidal-structures-on-sets) have different units, $1$ and $\varnothing$, which are not isomorphic. They are even inequivalent as [monoidal categories](../../../category-theory.md#monoidal-category): an equivalence of the underlying [Category of sets](../../../category.md#category-of-sets) preserves [terminal objects](../../../category.md#terminal-object), so it cannot take the singleton unit of the product structure to the empty unit of the coproduct structure. Hence **the monoidal structure on [sets](../../../set.md) is not unique**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
