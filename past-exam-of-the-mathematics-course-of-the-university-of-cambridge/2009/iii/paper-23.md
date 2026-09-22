# Paper 23

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper23.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper23.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
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
- [6](#6)
  - [Solution](#6/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
  - [c](#7/c)
    - [Solution](#7/c/solution)
- [8](#8)
  - [a](#8/a)
    - [Solution](#8/a/solution)
  - [b](#8/b)
    - [Solution](#8/b/solution)
  - [c](#8/c)
    - [Solution](#8/c/solution)

## 1

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $D:I\to\mathcal C$ be a finite diagram. Form the finite [categorical products](../../../category.md#product-category-theory)

$$
P=\prod_{i\in\operatorname{Ob}I}D(i),\qquad Q=\prod_{u:i\to j\in\operatorname{Mor}I}D(j).
$$

There are two [morphisms](../../../algebra.md#morphism) $s,t:P\rightrightarrows Q$: their components at $u:i\to j$ are $D(u)\pi_i$ and $\pi_j$, respectively. Let $e:L\to P$ be their [equaliser](../../../category.md#equaliser). Then $\ell_i=\pi_i e$ satisfy $D(u)\ell_i=\ell_j$, so they constitute a [cone over a diagram](../../../category.md#cone-over-a-diagram).

Any other cone $x_i:X\to D(i)$ uniquely determines $x:X\to P$. Its cone equations say precisely that $sx=tx$. The [equaliser](../../../category.md#equaliser) therefore gives a unique $h:X\to L$ with $eh=x$, and thus $\ell_i h=x_i$. Conversely these component equations force $eh=x$ by the [categorical product](../../../category.md#product-category-theory) [universal property](../../../category-theory.md#universal-property), so there is exactly one such mediator. This proves that $(L,\ell_i)$ is a [categorical limit](../../../category.md#categorical-limit) of $D$.

The empty [categorical products](../../../category.md#product-category-theory) are included: if $I$ is empty, $P$ and $Q$ are terminal and the construction gives the empty [categorical limit](../../../category.md#categorical-limit). Thus **finite [categorical products](../../../category.md#product-category-theory) and [equalisers](../../../category.md#equaliser) give every finite [categorical limit](../../../category.md#categorical-limit)**, as a special case of the [construction of small limits from products and equalizers](../../../category.md#construction-of-small-limits-from-products-and-equalizers).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $1$ be a [terminal object](../../../category.md#terminal-object). The [pullback](../../../category.md#pullback-category-theory) of the unique arrows $A\to1\leftarrow B$ is a binary [categorical product](../../../category.md#product-category-theory): maps $X\to A$ and $X\to B$ automatically have equal composites into $1$, so the [pullback](../../../category.md#pullback-category-theory) [universal property](../../../category-theory.md#universal-property) is exactly the [categorical product](../../../category.md#product-category-theory) [universal property](../../../category-theory.md#universal-property).

For parallel arrows $f,g:A\rightrightarrows B$, form $B\times B$ and take the [pullback](../../../category.md#pullback-category-theory) of $\langle f,g\rangle:A\to B\times B$ along the diagonal $\delta:B\to B\times B$. Write the resulting projections as $e:E\to A$ and $b:E\to B$. The [pullback](../../../category.md#pullback-category-theory) equation gives

$$
fe=b=ge.
$$

If $u:X\to A$ satisfies $fu=gu$, the pair $(u,fu)$ is a [pullback](../../../category.md#pullback-category-theory) cone, producing a unique $v:X\to E$ with $ev=u$ and $bv=fu$. The second condition is forced by the first, since $b=fe$. Thus $e$ is the [equaliser](../../../category.md#equaliser) of $f,g$.

The [terminal object](../../../category.md#terminal-object) and iterated binary [categorical products](../../../category.md#product-category-theory) give all finite [categorical products](../../../category.md#product-category-theory), including the nullary one. Part (a) therefore proves **[pullbacks](../../../category.md#pullback-category-theory) and a [terminal object](../../../category.md#terminal-object) give all finite [categorical limits](../../../category.md#categorical-limit)**.

## 2

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a diagram shape $I$, a [functor](../../../category.md#functor) $F:\mathcal C\to\mathcal D$ preserves [categorical limits](../../../category.md#categorical-limit) of shape $I$ if every limiting cone $(L,\ell_i)$ over every diagram $D:I\to\mathcal C$ is carried to a limiting cone $(FL,F\ell_i)$ over $FD$. It reflects [categorical limits](../../../category.md#categorical-limit) of that shape if a cone in $\mathcal C$ is limiting whenever its image cone is limiting. These properties concern cones which are given; reflection is not an assertion that every cone in the target lifts.

Suppose $F$ is a [full and faithful functor](../../../category.md#full-and-faithful-functor) and the image of $(L,\ell_i)$ is limiting. A cone $(X,x_i)$ in $\mathcal C$ becomes a cone in $\mathcal D$, so there is a unique $h:FX\to FL$ with $(F\ell_i)h=Fx_i$. Fullness writes $h=Fk$ for some $k:X\to L$. Faithfulness gives $\ell_i k=x_i$, and also ensures uniqueness: two such $k$ would have the same image, by uniqueness of $h$. Hence the original cone is limiting. This proves **every [full and faithful functor](../../../category.md#full-and-faithful-functor) reflects [categorical limits](../../../category.md#categorical-limit)**, the [limits reflected by full and faithful functors](../../../category.md#limits-reflected-by-full-and-faithful-functors) criterion, with no essential-surjectivity requirement.

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Take any limiting cone $\ell_i:L\to D(i)$ in $\mathcal C$ of the given shape. Since $GF$ preserves such [categorical limits](../../../category.md#categorical-limit), the cone $GF\ell_i:GFL\to GFD(i)$ is limiting in $\mathcal E$. It is the image under $G$ of the cone $F\ell_i$ in $\mathcal D$. Reflection by $G$ therefore says that $F\ell_i$ is limiting in $\mathcal D$. Since this works for every diagram and every limiting cone of the specified shape, **$F$ preserves [categorical limits](../../../category.md#categorical-limit) of that shape**.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Write an object of the [slice category](../../../category.md#slice-category) $\mathcal D/X$ as $a:A\to X$. Its [morphisms](../../../algebra.md#morphism) are arrows in $\mathcal D$ commuting with these structure maps, and the [forgetful functor](../../../category.md#forgetful-functor) $U_X$ removes the structure map.

Suppose a square in the slice becomes a [pullback](../../../category.md#pullback-category-theory) square in $\mathcal D$, with vertex $p:P\to X$. Given a compatible pair of slice arrows $u:Z\to A$ and $v:Z\to B$, the underlying [pullback](../../../category.md#pullback-category-theory) gives a unique $h:Z\to P$ with the required projection equations. If $r:P\to A$ is one projection, then

$$
ph=arh=au=z,
$$

where $z:Z\to X$ is the structure map. Thus $h$ is automatically a slice [morphism](../../../algebra.md#morphism), and underlying uniqueness gives uniqueness in the slice. Hence **$U_X$ reflects [pullbacks](../../../category.md#pullback-category-theory)**.

Now let $e:(E,c)\to(A,a)$ be an [equaliser](../../../category.md#equaliser) of slice arrows $f,g:(A,a)\rightrightarrows(B,b)$. Consider any underlying arrow $u:Z\to A$ with $fu=gu$. Give $Z$ the structure map $au:Z\to X$. Then $u$ is a slice arrow into $(A,a)$, and the slice [equaliser](../../../category.md#equaliser) gives a unique $h:Z\to E$ with $eh=u$. Conversely any underlying $h$ with that equation automatically obeys $ch=aeh=au$, so there are no additional factorization possibilities outside the slice. Therefore $U_Xe$ has the ordinary [equaliser](../../../category.md#equaliser) [universal property](../../../category-theory.md#universal-property) in $\mathcal D$. This proves **$U_X$ preserves [equalisers](../../../category.md#equaliser)**.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $!_A:A\to1$ be the unique arrow to the [terminal object](../../../category.md#terminal-object) of $\mathcal C$. Define

$$
\widehat F(A)=(FA\xrightarrow{F!_A}F1),\qquad \widehat F(f)=Ff.
$$

This is a [functor](../../../category.md#functor) into the [slice category](../../../category.md#slice-category) $\mathcal D/F1$, because $!_Bf=!_A$, and $U_{F1}\widehat F=F$. The [terminal object](../../../category.md#terminal-object) of this slice is $1_{F1}:F1\to F1$, exactly $\widehat F(1)$, so $\widehat F$ preserves the [terminal object](../../../category.md#terminal-object).

The composite $U_{F1}\widehat F$ preserves [pullbacks](../../../category.md#pullback-category-theory) by hypothesis, and $U_{F1}$ reflects [pullbacks](../../../category.md#pullback-category-theory) by part (b). Part (a), restricted to the [pullback](../../../category.md#pullback-category-theory) shape, therefore shows that $\widehat F$ preserves [pullbacks](../../../category.md#pullback-category-theory). The allowed finite-limit criterion now gives that $\widehat F$ preserves all finite [categorical limits](../../../category.md#categorical-limit), and hence [equalisers](../../../category.md#equaliser). Since $U_{F1}$ preserves [equalisers](../../../category.md#equaliser), their composite does too. Thus

$$
\boxed{F\text{ preserves equalisers.}}
$$

This is [equalizer preservation by pullback-preserving functors](../../../category.md#equalizer-preservation-by-pullback-preserving-functors). The factorization supplies terminal-object preservation only in the slice; none is asserted for the original $F$.

## 3

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Write $H_c=\mathcal C(-,c)$. The [category of elements](../../../category.md#category-of-elements) $\int P$ of a [categorical presheaf](../../../category.md#presheaf-category-theory) $P$ has objects $(c,x)$ with $x\in P(c)$; a [morphism](../../../algebra.md#morphism) $(c,x)\to(d,y)$ is $u:c\to d$ satisfying $P(u)y=x$. It is a [small category](../../../category.md#small-category) because $\mathcal C$ is small and each $P(c)$ is a [set](../../../set.md). Consider the diagram sending $(c,x)$ to $H_c$ and $u$ to the [natural transformation](../../../category.md#natural-transformation) given by postcomposition with $u$.

There is a canonical cocone $\alpha_{c,x}:H_c\to P$ with

$$
(\alpha_{c,x})_a(v)=P(v)x\qquad(v:a\to c).
$$

Functoriality makes it a [natural transformation](../../../category.md#natural-transformation), and the equation $P(u)y=x$ makes these transformations a cocone.

To prove its [universal property](../../../category-theory.md#universal-property), let $Q$ be any [categorical presheaf](../../../category.md#presheaf-category-theory) with a compatible cocone $\beta_{c,x}:H_c\to Q$. Define

$$
t_c(x)=(\beta_{c,x})_c(1_c).
$$

For $u:c\to d$ and $y\in P(d)$, compatibility with the arrow $(c,P(u)y)\to(d,y)$ gives

$$
t_c(P(u)y)=(\beta_{d,y})_c(u)=Q(u)(\beta_{d,y})_d(1_d)=Q(u)t_d(y).
$$

Thus $t:P\to Q$ is natural. [Naturality](../../../category.md#naturality) of each $\beta_{c,x}$ shows $t\alpha_{c,x}=\beta_{c,x}$. Conversely any transformation with these equations must have the displayed values $t_c(x)$, so it is unique. We have proved the [canonical colimit presentation of a presheaf](../../../category.md#canonical-colimit-presentation-of-a-presheaf):

$$
\boxed{P\cong\operatorname{colim}_{(c,x)\in\int P}H_c.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A [Cartesian closed category](../../../category.md#cartesian-closed-category) has finite [categorical products](../../../category.md#product-category-theory) and, for every $P,Q$, an [exponential object](../../../category.md#exponential-object) $Q^P$ with an evaluation [morphism](../../../algebra.md#morphism) $\operatorname{ev}:Q^P\times P\to Q$ such that composition with evaluation gives [natural bijections](../../../category.md#natural-bijection)

$$
\mathcal E(R,Q^P)\cong\mathcal E(R\times P,Q).
$$

Finite [categorical products](../../../category.md#product-category-theory) in the [presheaf category](../../../category.md#presheaf-category) are pointwise; in particular its [terminal object](../../../category.md#terminal-object) is the constant singleton [categorical presheaf](../../../category.md#presheaf-category-theory). For [categorical presheaves](../../../category.md#presheaf-category-theory) $P,Q$ define

$$
\boxed{(Q^P)(c)=\operatorname{Nat}(H_c\times P,Q).}
$$

For $u:d\to c$, restriction sends $\alpha$ to $\alpha\circ(H_u\times1_P)$. Composition and identity laws follow from those of the [Yoneda embedding](../../../category.md#yoneda-embedding), so this is a [categorical presheaf](../../../category.md#presheaf-category-theory).

Define evaluation at $c$ by $\operatorname{ev}_c(\alpha,x)=\alpha_c(1_c,x)$. For $u:d\to c$, [naturality](../../../category.md#naturality) of $\alpha$ gives $Q(u)\alpha_c(1_c,x)=\alpha_d(u,P(u)x)$, which is the evaluation of the restricted pair. Hence evaluation is a [natural transformation](../../../category.md#natural-transformation).

Given $t:R\times P\to Q$, its [currying](../../../category.md#currying) sends $z\in R(c)$ to the transformation whose component at $a$ is

$$
(\widehat t_c(z))_a(v,x)=t_a(R(v)z,x)\qquad(v:a\to c,\ x\in P(a)).
$$

[Naturality](../../../category.md#naturality) in $a$ follows from that of $t$, and [naturality](../../../category.md#naturality) in $c$ follows by composing $v$ with the relevant arrow. Evaluating $\widehat t$ at $(1_c,x)$ recovers $t_c(z,x)$. Conversely, if $s:R\to Q^P$, [naturality](../../../category.md#naturality) of $s$ along $v:a\to c$ says that evaluating $s_a(R(v)z)$ at $(1_a,x)$ gives $(s_c(z))_a(v,x)$. Thus [currying](../../../category.md#currying) the evaluation of $s$ recovers $s$. These constructions are inverse and natural, proving the [universal property](../../../category-theory.md#universal-property). This is the [exponential in a presheaf category](../../../category.md#exponential-in-a-presheaf-category), and proves **the [presheaf category](../../../category.md#presheaf-category) is [Cartesian closed](../../../category.md#cartesian-closed-category)**.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [Yoneda embedding](../../../category.md#yoneda-embedding) preserves [categorical products](../../../category.md#product-category-theory): for any $a$, maps $a\to c\times Y$ correspond naturally to pairs of maps $a\to c$ and $a\to Y$. Hence $H_{c\times Y}\cong H_c\times H_Y$. Using the [exponential in a presheaf category](../../../category.md#exponential-in-a-presheaf-category), the [Yoneda lemma](../../../category.md#yoneda-lemma) and the exponential [universal property](../../../category-theory.md#universal-property) in $\mathcal C$ gives

$$
\begin{aligned}
((H_Z)^{H_Y})(c)
&=\operatorname{Nat}(H_c\times H_Y,H_Z)\\
&\cong\operatorname{Nat}(H_{c\times Y},H_Z)\\
&\cong\mathcal C(c\times Y,Z)\\
&\cong\mathcal C(c,Z^Y)=H_{Z^Y}(c).
\end{aligned}
$$

Every [bijection](../../../function.md#bijection) is natural in $c$, since it is given by precomposition or the natural exponential [adjunction](../../../category.md#adjoint-functors). Thus these component [bijections](../../../function.md#bijection) are a [natural isomorphism](../../../category.md#natural-isomorphism) of [categorical presheaves](../../../category.md#presheaf-category-theory):

$$
\boxed{(H_Z)^{H_Y}\cong H_{Z^Y}.}
$$

## 4

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [Yoneda embedding](../../../category.md#yoneda-embedding) sends $c$ to the [representable presheaf](../../../category.md#representable-functor) $H_c=\mathcal C(-,c)$. On a [morphism](../../../algebra.md#morphism) $f:c\to d$, it sends a map $u:a\to c$ to $fu:a\to d$, giving $H_f:H_c\to H_d$.

The [Yoneda lemma](../../../category.md#yoneda-lemma) states that for every [categorical presheaf](../../../category.md#presheaf-category-theory) $P$ there is a [bijection](../../../function.md#bijection), natural in both variables,

$$
\operatorname{Nat}(H_c,P)\cong P(c),\qquad \alpha\longmapsto\alpha_c(1_c).
$$

Its inverse sends $x\in P(c)$ to the transformation $u:a\to c\mapsto P(u)x$. Apply it to $P=H_d$ to obtain

$$
\operatorname{Nat}(H_c,H_d)\cong H_d(c)=\mathcal C(c,d).
$$

Under this [bijection](../../../function.md#bijection) $H_f$ corresponds exactly to $f$, so the map induced by the embedding on each [hom-set](../../../category.md#hom-set) is bijective. Therefore **the [Yoneda embedding](../../../category.md#yoneda-embedding) is [full and faithful](../../../category.md#full-and-faithful-functor)**.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The equations $pi=1_A$ give $(ip)i=i$, so $i$ equalizes $ip$ and $1_B$. If $h:X\to B$ satisfies $(ip)h=h$, put $k=ph:X\to A$. Then $ik=iph=h$. If $k'$ is another such factorization, applying $p$ gives $k'=pik'=ph=k$. This proves

$$
\boxed{i:A\to B\text{ is the equaliser of }ip\text{ and }1_B.}
$$

In particular the inclusion in a [retract in a category](../../../category.md#retract-in-a-category) is a [monomorphism](../../../category.md#monomorphism).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

By part (b), $i:P\to H_B$ is the [equaliser](../../../category.md#equaliser) of $ip$ and $1_{H_B}$. Full faithfulness of the [Yoneda embedding](../../../category.md#yoneda-embedding) writes $ip=H_b$ for a unique [endomorphism](../../../algebra.md#endomorphism) $b:B\to B$. Choose an [equaliser](../../../category.md#equaliser) $e:A\to B$ of $b$ and $1_B$ in $\mathcal C$.

For each $c$, the maps $c\to A$ are precisely the maps $u:c\to B$ with $bu=u$. Thus $H_e:H_A\to H_B$ is the pointwise [equaliser](../../../category.md#equaliser) of $H_b$ and $1_{H_B}$, hence their [equaliser](../../../category.md#equaliser) in the [presheaf category](../../../category.md#presheaf-category). Both $i$ and $H_e$ have the same [universal property](../../../category-theory.md#universal-property), so their vertices are isomorphic. This proves the [representable retract criterion](../../../category.md#representable-retract-criterion):

$$
\boxed{P\cong H_A.}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Use [0-presentable object](../../../category.md#small-projective-object) in the specified sense: its hom-functor preserves all small [colimits](../../../category.md#colimit). For a [representable](../../../category.md#representable-functor) $H_c$, the [Yoneda lemma](../../../category.md#yoneda-lemma) identifies this hom-functor with evaluation at $c$. Given any small diagram $P_j$, pointwise [colimits](../../../category.md#colimit) give

$$
\begin{aligned}
\operatorname{Nat}\left(H_c,\operatorname{colim}_j P_j\right)
&\cong\left(\operatorname{colim}_jP_j\right)(c)\\
&=\operatorname{colim}_jP_j(c)\\
&\cong\operatorname{colim}_j\operatorname{Nat}(H_c,P_j).
\end{aligned}
$$

These are the canonical comparison [bijections](../../../function.md#bijection), including for an empty diagram. Therefore **every [representable presheaf](../../../category.md#representable-functor) is 0-presentable**, or a [small projective object](../../../category.md#small-projective-object) in this sense.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

By the [canonical colimit presentation of a presheaf](../../../category.md#canonical-colimit-presentation-of-a-presheaf), write

$$
P=\operatorname{colim}_{(c,x)\in\int P}H_c
$$

with structure maps $\alpha_{c,x}:H_c\to P$. Since $P$ is a [0-presentable object](../../../category.md#small-projective-object), the canonical map

$$
\operatorname{colim}_{(c,x)}\operatorname{Nat}(P,H_c)\longrightarrow\operatorname{Nat}(P,P)
$$

is bijective. Every element of a set-valued [colimit](../../../category.md#colimit) has a representative in some component. In particular $1_P$ is the image of a transformation $s:P\to H_c$ for some $(c,x)$, so

$$
\alpha_{c,x}s=1_P.
$$

Thus $P$ is a retract of $H_c$. The [representable retract criterion](../../../category.md#representable-retract-criterion) from part (c), using the assumed [equalisers](../../../category.md#equaliser) in $\mathcal C$, now gives **$P$ is [representable](../../../category.md#representable-functor)**. Only existence of the representative of $1_P$ is needed; no stronger uniqueness-of-factorization assertion about individual [colimit](../../../category.md#colimit) injections has been assumed.

## 5

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

A [poset](../../../set.md#partially-ordered-set) becomes a [category](../../../category.md) whose objects are its elements and whose [hom-set](../../../category.md#hom-set) $X(x,y)$ is a singleton if $x\le y$ and empty otherwise. Reflexivity supplies identity arrows and transitivity supplies composition; all possible composites are unique, so the [category](../../../category.md) axioms hold. Antisymmetry says that isomorphic objects are equal. A [functor](../../../category.md#functor) between such [categories](../../../category.md) is exactly an [order-preserving function](../../../set.md#order-preserving-function): an inequality must be sent to an inequality, and there is no further choice of arrow map.

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Since the [hom-sets](../../../category.md#hom-set) in these [categories](../../../category.md) are either empty or singleton, an [adjunction](../../../category.md#adjoint-functors) $f\dashv g$ is precisely the condition

$$
\boxed{f(x)\le y\quad\Longleftrightarrow\quad x\le g(y)\qquad(x\in X,\ y\in Y).}
$$

The [hom-set](../../../category.md#hom-set) [bijections](../../../function.md#bijection) are then the unique possible ones, and [naturality](../../../category.md#naturality) is automatic. This is a [Galois connection](../../../category.md#galois-connection) between the two [posets](../../../set.md#partially-ordered-set).

Equivalently, the monotone [functions](../../../function.md) satisfy the unit and counit inequalities $x\le gf(x)$ and $fg(y)\le y$. The equivalence implies these by taking $y=f(x)$ and $x=g(y)$. Conversely, if the inequalities hold, $f(x)\le y$ implies $x\le gf(x)\le g(y)$, while $x\le g(y)$ implies $f(x)\le fg(y)\le y$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For $X\subseteq A$, define

$$
\exists_p(X)=p[X],\qquad \forall_p(X)=\{b\in B:p^{-1}\{b\}\subseteq X\}=B\setminus p[A\setminus X].
$$

Both are monotone maps $PA\to PB$. For $Y\subseteq B$,

$$
p[X]\subseteq Y\quad\Longleftrightarrow\quad X\subseteq p^{-1}[Y],
$$

so [direct image](../../../ringed-space.md#direct-image-sheaf) is a [left adjoint](../../../category.md#adjoint-functors) to inverse image. Also,

$$
p^{-1}[Y]\subseteq X\quad\Longleftrightarrow\quad Y\subseteq\{b:p^{-1}\{b\}\subseteq X\},
$$

so the fiberwise universal condition gives the [right adjoint](../../../category.md#adjoint-functors). Therefore

$$
\boxed{\exists_p\dashv p^*\dashv\forall_p.}
$$

An empty fiber satisfies the universal condition vacuously, so every point outside $p[A]$ belongs to $\forall_p(X)$, regardless of $X$. This is essential when $p$ is not surjective.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

For a [categorical presheaf](../../../category.md#presheaf-category-theory) $P$ on the open subsets, define the [functors](../../../category.md#functor) on objects by

$$
L(P)=P(\varnothing),\qquad R(P)=P(S).
$$

To prove $L\dashv\Delta$, a [natural transformation](../../../category.md#natural-transformation) $t:P\to\Delta A$ must satisfy

$$
t_U=t_{\varnothing}\circ\operatorname{res}^{U}_{\varnothing}
$$

for every open $U$, since the restrictions of $\Delta A$ are identities. Thus it is determined by the [function](../../../function.md) $P(\varnothing)\to A$. Conversely such a [function](../../../function.md) defines all $t_U$ by that equation, and the [categorical presheaf](../../../category.md#presheaf-category-theory) restriction laws make the components compatible. Hence

$$
\operatorname{Nat}(P,\Delta A)\cong\operatorname{Set}(P(\varnothing),A).
$$

For the other [adjunction](../../../category.md#adjoint-functors), a transformation $s:\Delta A\to P$ is determined by its component $s_S:A\to P(S)$, since

$$
s_U=\operatorname{res}^{S}_U\circ s_S.
$$

Every [function](../../../function.md) $A\to P(S)$ supplies compatible components by this formula. Therefore $\operatorname{Nat}(\Delta A,P)\cong\operatorname{Set}(A,P(S))$, giving the [adjoints to constant presheaves on open sets](../../../category.md#adjoints-to-constant-presheaves-on-open-sets):

$$
\boxed{\operatorname{ev}_{\varnothing}\dashv\Delta\dashv\operatorname{ev}_S.}
$$

These are adjoints of the stated constant-presheaf [functor](../../../category.md#functor), with its value at every [open set](../../../topology.md#open-set) including the empty one; no sheafification is involved.

## 6

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

The [Freyd general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem) is as follows. Let $G:\mathcal D\to\mathcal C$, with $\mathcal D$ a [complete category](../../../category.md#complete-category) which is [locally small](../../../category.md#locally-small-category). Then $G$ has a [left adjoint](../../../category.md#adjoint-functors) if and only if it preserves all small [categorical limits](../../../category.md#categorical-limit) and satisfies the [solution-set condition](../../../category.md#solution-set-condition): for each $c\in\mathcal C$, there is a set-indexed family

$$
u_i:c\to Gd_i
$$

such that every $u:c\to Gd$ can be written $u=G(h)u_i$ for some $i$ and some $h:d_i\to d$. The target [category](../../../category.md) need not be complete. We prove all the existence steps.

First establish the [initial-object lemma for complete categories with a weakly initial set](../../../category.md#initial-object-lemma-for-complete-categories-with-a-weakly-initial-set). Let $\mathcal E$ be [locally small](../../../category.md#locally-small-category) and complete, with a [weakly initial set](../../../category.md#weakly-initial-set) $\{w_i\}$, meaning every object receives a map from at least one $w_i$. Its [categorical product](../../../category.md#product-category-theory) $w=\prod_iw_i$ is weakly initial: compose a [categorical product](../../../category.md#product-category-theory) projection with the map from the appropriate $w_i$. Local smallness makes $\mathcal E(w,w)$ a [set](../../../set.md). Let $e:v\to w$ be the simultaneous [equaliser](../../../category.md#equaliser) of every [endomorphism](../../../algebra.md#endomorphism) of $w$ and the identity. Explicitly it is the [equaliser](../../../category.md#equaliser) of the two arrows

$$
w\rightrightarrows\prod_{k\in\mathcal E(w,w)}w
$$

with components $k$ and $1_w$. Thus $ke=e$ for every [endomorphism](../../../algebra.md#endomorphism) $k$, and $e$ is monic.

Every object $x$ receives a [morphism](../../../algebra.md#morphism) from $v$, by composing $e$ with a map $w\to x$. To prove uniqueness, take parallel maps $a,b:v\to x$ and their [equaliser](../../../category.md#equaliser) $m:y\to v$. Weak initiality of $w$ gives $t:w\to y$. The composite $emt$ is an [endomorphism](../../../algebra.md#endomorphism) of $w$, so $(emt)e=e$. Cancelling the [monomorphism](../../../category.md#monomorphism) $e$ gives $mte=1_v$. Hence $m$ is both monic and a [split epimorphism](../../../category.md#split-epimorphism), and is therefore invertible. Since $am=bm$, this forces $a=b$. We have proved $v$ is initial, without using a class-sized [categorical product](../../../category.md#product-category-theory) or [equaliser](../../../category.md#equaliser).

For sufficiency in the theorem, fix $c$ and consider the [comma category](../../../category.md#comma-category) $(c\downarrow G)$. Its objects are pairs $(d,u:c\to Gd)$; a [morphism](../../../algebra.md#morphism) $h:(d,u)\to(d',u')$ satisfies $G(h)u=u'$. This [category](../../../category.md) is [locally small](../../../category.md#locally-small-category) because each [hom-set](../../../category.md#hom-set) is a subset of $\mathcal D(d,d')$. It is complete: for a small diagram of such pairs, take the underlying [categorical limit](../../../category.md#categorical-limit) $d$ in $\mathcal D$. The arrows from $c$ form a cone to its image under $G$, and preservation of the [categorical limit](../../../category.md#categorical-limit) gives a unique $u:c\to Gd$ inducing them. The same [universal property](../../../category-theory.md#universal-property) gives all mediators in the [comma category](../../../category.md#comma-category). The solution-set family is a [weakly initial set](../../../category.md#weakly-initial-set) in this [comma category](../../../category.md#comma-category), so the lemma supplies an initial pair

$$
(Fc,\eta_c:c\to GFc).
$$

For $f:c\to c'$, initiality defines a unique $Ff:Fc\to Fc'$ satisfying $G(Ff)\eta_c=\eta_{c'}f$. Uniqueness proves the identity and composition laws, making $F$ a [functor](../../../category.md#functor). Initiality also gives [bijections](../../../function.md#bijection)

$$
\boxed{\mathcal D(Fc,d)\cong\mathcal C(c,Gd),\qquad h\longmapsto G(h)\eta_c.}
$$

The definition of $Ff$ proves [naturality](../../../category.md#naturality) in $c$, and postcomposition proves [naturality](../../../category.md#naturality) in $d$. These [bijections](../../../function.md#bijection) are the required [adjunction](../../../category.md#adjoint-functors) $F\dashv G$.

For necessity, if $F\dashv G$, the single arrow $\eta_c:c\to GFc$ is a solution [set](../../../set.md): the transpose of any $u:c\to Gd$ gives its factorization through $\eta_c$. If $d$ is a limiting cone vertex of a small diagram $D_j$ in $\mathcal D$, then, naturally in $c$,

$$
\mathcal C(c,Gd)\cong\mathcal D(Fc,d)
\cong\lim_j\mathcal D(Fc,D_j)
\cong\lim_j\mathcal C(c,GD_j).
$$

These are the canonical cone-factorization [bijections](../../../function.md#bijection), so $Gd$ with its image projections is a [categorical limit](../../../category.md#categorical-limit) of $GD_j$. Thus $G$ preserves all small [categorical limits](../../../category.md#categorical-limit), completing both directions of the theorem.

## 7

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

A [monad](../../../category-theory.md#monad) on $\mathcal C$ consists of an [endofunctor](../../../category.md#endofunctor) $T:\mathcal C\to\mathcal C$ and [natural transformations](../../../category.md#natural-transformation) $\eta:1_{\mathcal C}\Rightarrow T$ and $\mu:T^2\Rightarrow T$ satisfying, at every object $A$,

$$
\boxed{\mu_A T\eta_A=1_{TA}=\mu_A\eta_{TA},\qquad
\mu_A T\mu_A=\mu_A\mu_{TA}.}
$$

These are the unit and associativity laws for the [unit and multiplication of a monad](../../../category-theory.md#unit-and-multiplication-of-a-monad).

An [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) is a pair $(A,a)$ with $a:TA\to A$ satisfying

$$
\boxed{a\eta_A=1_A,\qquad a\mu_A=aT a.}
$$

A [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad) $f:(A,a)\to(B,b)$ is a [morphism](../../../algebra.md#morphism) $f:A\to B$ with $fa=bT f$. Identities satisfy this condition, and composing two such maps preserves it by functoriality of $T$. The resulting [Eilenberg-Moore category](../../../category-theory.md#eilenberg-moore-category) is denoted $\mathcal C^T$. Its [forgetful functor](../../../category.md#forgetful-functor) $U:\mathcal C^T\to\mathcal C$ sends $(A,a)$ to $A$ and leaves the underlying arrows unchanged.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Write the [adjunction unit](../../../category.md#unit-of-an-adjunction) as $\eta:1_{\mathcal C}\Rightarrow GF$ and the [adjunction counit](../../../category.md#counit-of-an-adjunction) as $\varepsilon:FG\Rightarrow1_{\mathcal D}$. Define the [monad induced by an adjunction](../../../category-theory.md#monad-induced-by-an-adjunction) by

$$
\boxed{T=GF,\qquad \mu_A=G\varepsilon_{FA}:GFGFA\to GFA,}
$$

with unit $\eta$. [Naturality](../../../category.md#naturality) of $\varepsilon$ makes $\mu$ a [natural transformation](../../../category.md#natural-transformation).

The [triangle identities for an adjunction](../../../category.md#triangle-identities-for-an-adjunction) give the two unit laws:

$$
\mu_A\eta_{TA}=G\varepsilon_{FA}\eta_{GFA}=1_{GFA},\qquad
\mu_A T\eta_A=G(\varepsilon_{FA}F\eta_A)=1_{GFA}.
$$

For associativity, apply [naturality](../../../category.md#naturality) of $\varepsilon$ to the arrow $\varepsilon_{FA}:FGFA\to FA$ in $\mathcal D$:

$$
\varepsilon_{FA}FG\varepsilon_{FA}=\varepsilon_{FA}\varepsilon_{FGFA}.
$$

Applying $G$ yields

$$
\mu_A T\mu_A=\mu_A\mu_{TA}.
$$

Thus the induced data satisfy all the [monad](../../../category-theory.md#monad) laws, rather than merely supplying an [endofunctor](../../../category.md#endofunctor) and two transformations.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

Define the [free algebra functor](../../../category-theory.md#free-algebra-functor) by

$$
F^T(X)=(TX,\mu_X),\qquad F^T(f)=Tf.
$$

The [monad](../../../category-theory.md#monad) laws say precisely that $\mu_X$ defines an [monad algebra](../../../category-theory.md#algebra-for-a-monad) structure on $TX$, while [naturality](../../../category.md#naturality) of $\mu$ makes $Tf$ an [monad algebra](../../../category-theory.md#algebra-for-a-monad) [morphism](../../../algebra.md#morphism). We construct the [adjunction](../../../category.md#adjoint-functors) explicitly.

For an [monad algebra](../../../category-theory.md#algebra-for-a-monad) $(A,a)$ and a [morphism](../../../algebra.md#morphism) $f:X\to A$, put $\overline f=aTf:TX\to A$. It is an [monad algebra](../../../category-theory.md#algebra-for-a-monad) [morphism](../../../algebra.md#morphism) because

$$
\overline f\mu_X=aTf\mu_X=a\mu_A T^2f
=aTaT^2f=aT\overline f.
$$

Conversely, from an [monad algebra](../../../category-theory.md#algebra-for-a-monad) [morphism](../../../algebra.md#morphism) $h:(TX,\mu_X)\to(A,a)$ obtain $h\eta_X:X\to A$. These operations are inverse: [naturality](../../../category.md#naturality) of $\eta$ and the [monad algebra](../../../category-theory.md#algebra-for-a-monad) unit law give

$$
aTf\eta_X=a\eta_A f=f,
$$

and the algebra-morphism equation together with the [monad](../../../category-theory.md#monad) unit law gives

$$
aT(h\eta_X)=aThT\eta_X=h\mu_XT\eta_X=h.
$$

The formulas commute with precomposition in $X$ and composition with [monad algebra](../../../category-theory.md#algebra-for-a-monad) [morphisms](../../../algebra.md#morphism) in $(A,a)$, so the [bijections](../../../function.md#bijection) are natural. Therefore the [free-forgetful Eilenberg-Moore adjunction](../../../category-theory.md#free-forgetful-eilenberg-moore-adjunction) is

$$
\boxed{F^T\dashv U,\qquad\mathcal C^T(F^TX,(A,a))\cong\mathcal C(X,A).}
$$

Its unit is $\eta_X$ and its counit at $(A,a)$ is the [monad algebra](../../../category-theory.md#algebra-for-a-monad) action $a$.

## 8

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

With $T=GF$, unit $\eta$ and multiplication $G\varepsilon F$, the [Eilenberg-Moore comparison functor](../../../category-theory.md#eilenberg-moore-comparison-functor) is

$$
\boxed{K:\mathcal D\to\mathcal C^T,\qquad Kd=(Gd,G\varepsilon_d),\qquad K(h)=Gh.}
$$

Here $G\varepsilon_d:T(Gd)=GFGd\to Gd$ is the [monad algebra](../../../category-theory.md#algebra-for-a-monad) action, and the underlying [functor](../../../category.md#functor) satisfies $UK=G$. The triangle identities and counit [naturality](../../../category.md#naturality) provide the [monad algebra](../../../category-theory.md#algebra-for-a-monad) laws and the compatibility of $Gh$, as required for this definition.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

For each [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) $(A,a)$, consider the specific pair in $\mathcal D$

$$
FTA\mathrel{\substack{\xrightarrow{Fa}\\\xrightarrow[\varepsilon_{FA}]{} }}FA.
$$

Then the exact condition is

$$
\boxed{K\text{ has a left adjoint}\quad\Longleftrightarrow\quad
\text{each of these pairs has a coequalizer in }\mathcal D.}
$$

Each pair is reflexive, with common section $F\eta_A$: the two composite identities follow from $a\eta_A=1_A$ and $\varepsilon_{FA}F\eta_A=1_{FA}$. Thus existence of all [reflexive coequalizers](../../../category-theory.md#reflexive-coequalizer) is sufficient, but the displayed specified pairs give the necessary-and-sufficient condition.

To prove it, take $h:FA\to d$ and its adjoint transpose $x=Gh\eta_A:A\to Gd$. The transpose of $hFa$ is $xa$, by [naturality](../../../category.md#naturality) of $\eta$. The transpose of $h\varepsilon_{FA}$ is

$$
GhG\varepsilon_{FA}\eta_{TA}=Gh\mu_A\eta_{TA}=Gh.
$$

Moreover counit [naturality](../../../category.md#naturality) and a triangle identity give

$$
G\varepsilon_d T x
=G\varepsilon_d,GF(Gh\eta_A)
=Gh,G\varepsilon_{FA},GF\eta_A=Gh.
$$

Because transposition is bijective, the coequalizing equation is therefore equivalent to

$$
hFa=h\varepsilon_{FA}\quad\Longleftrightarrow\quad xa=G\varepsilon_d T x.
$$

The right side says exactly that $x:(A,a)\to Kd$ is a [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad).

For sufficiency, choose a [coequalizer](../../../category.md#coequalizer) $q_a:FA\to L(A,a)$ for every [monad algebra](../../../category-theory.md#algebra-for-a-monad). Its [universal property](../../../category-theory.md#universal-property) and the equivalence just proved give [natural bijections](../../../category.md#natural-bijection)

$$
\mathcal D(L(A,a),d)\cong
\{h:FA\to d:hFa=h\varepsilon_{FA}\}
\cong\mathcal C^T((A,a),Kd).
$$

To see explicitly that the chosen objects form a [functor](../../../category.md#functor), an [monad algebra](../../../category-theory.md#algebra-for-a-monad) [morphism](../../../algebra.md#morphism) $u:(A,a)\to(B,b)$ makes $q_bFu$ coequalize the pair for $a$: use $ua=bTu$ and [naturality](../../../category.md#naturality) of the counit. Hence there is a unique $Lu$ with $Lu\,q_a=q_bFu$. Uniqueness proves its identity and composition laws and the [naturality](../../../category.md#naturality) of the displayed [bijections](../../../function.md#bijection). Thus $L\dashv K$.

Conversely, suppose $L\dashv K$ with unit $\lambda_{(A,a)}:(A,a)\to KL(A,a)$. Transpose its underlying arrow $A\to GL(A,a)$ through $F\dashv G$ to obtain $q_a:FA\to L(A,a)$. Since the unit is an [monad algebra](../../../category-theory.md#algebra-for-a-monad) [morphism](../../../algebra.md#morphism), the equivalence above shows that $q_a$ coequalizes the specified pair. Any coequalizing $h:FA\to d$ transposes to an [monad algebra](../../../category-theory.md#algebra-for-a-monad) map $(A,a)\to Kd$, which factors uniquely through the unit by $L\dashv K$. Transposing back gives a unique factorization of $h$ through $q_a$. Thus $q_a$ is the required [coequalizer](../../../category.md#coequalizer). This proves both directions of the [Left adjoint to the Eilenberg-Moore comparison functor](../../../category-theory.md#left-adjoint-to-the-eilenberg-moore-comparison-functor) criterion.

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

Assume the [coequalizers](../../../category.md#coequalizer) from part (b) exist and write them $q_a:FA\to L(A,a)$. The underlying arrow of the comparison-adjunction unit is

$$
\lambda_a=Gq_a\eta_A:A\to GL(A,a).
$$

We first relate it to the [monad algebra](../../../category-theory.md#algebra-for-a-monad) action. [Naturality](../../../category.md#naturality) of $\eta$, the [coequalizer](../../../category.md#coequalizer) equation and a [monad](../../../category-theory.md#monad) unit law give

$$
\begin{aligned}
\lambda_a a
&=Gq_a\eta_A a=Gq_a,Ta\,\eta_{TA}\\
&=G(q_aFa)\eta_{TA}=G(q_a\varepsilon_{FA})\eta_{TA}\\
&=Gq_a\mu_A\eta_{TA}=Gq_a.
\end{aligned}
$$

In $\mathcal C$, $a:TA\to A$ is itself a [split coequalizer](../../../category.md#split-coequalizer) of $Ta,\mu_A:T^2A\rightrightarrows TA$. Indeed,

$$
aTa=a\mu_A,\quad a\eta_A=1_A,\quad
\mu_A\eta_{TA}=1_{TA},\quad Ta\eta_{TA}=\eta_Aa.
$$

For an explicit universal-property proof, if $r:TA\to X$ satisfies $rTa=r\mu_A$, then $s=r\eta_A$ obeys

$$
sa=r\eta_Aa=rTa\eta_{TA}=r\mu_A\eta_{TA}=r.
$$

Its uniqueness follows by composing any equation $sa=r$ with $\eta_A$.

Now $Gq_a$ equalizes $Ta$ and $\mu_A$. If it is a [coequalizer](../../../category.md#coequalizer), then $a$ and $Gq_a$ are [coequalizers](../../../category.md#coequalizer) of the same pair. Their unique comparison map is $\lambda_a$, since $\lambda_a a=Gq_a$, and is therefore invertible. Conversely, if $\lambda_a$ is invertible, $Gq_a=\lambda_a a$ is an isomorphic copy of the [coequalizer](../../../category.md#coequalizer) $a$, so it is a [coequalizer](../../../category.md#coequalizer) too.

The [forgetful functor](../../../category.md#forgetful-functor) $\mathcal C^T\to\mathcal C$ reflects [isomorphisms](../../../algebra.md#isomorphism): if an [monad algebra](../../../category-theory.md#algebra-for-a-monad) [morphism](../../../algebra.md#morphism) $u$ has an inverse as an underlying arrow, the equation $ua=bTu$ rearranges to $u^{-1}b=aT(u^{-1})$, making that inverse an [monad algebra](../../../category-theory.md#algebra-for-a-monad) [morphism](../../../algebra.md#morphism). Thus underlying invertibility here is exactly invertibility of the unit component. For all [monad algebras](../../../category-theory.md#algebra-for-a-monad) together, the [comparison-adjunction unit criterion](../../../category-theory.md#comparison-adjunction-unit-criterion) is

$$
\boxed{\lambda\text{ is invertible}\quad\Longleftrightarrow\quad
G\text{ preserves every specified coequalizer }q_a.}
$$

Equivalently, the necessary-and-sufficient conditions for a [left adjoint](../../../category.md#adjoint-functors) with invertible unit are existence of the [coequalizers](../../../category.md#coequalizer) in part (b) and their preservation by $G$. No preservation of arbitrary [coequalizers](../../../category.md#coequalizer) is required.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
