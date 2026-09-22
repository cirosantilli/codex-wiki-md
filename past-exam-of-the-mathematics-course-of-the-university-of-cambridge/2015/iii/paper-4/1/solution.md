<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Choose a [projective presentation](../../../../../projective-presentation.md) $0\to K\xrightarrow{j}P\xrightarrow{\pi}C\to0$, with $P$ a [projective module](../../../../../projective-module.md). Continuing it to a [projective resolution](../../../../../projective-resolution.md) shows

$$
\operatorname{Ext}_R^1(C,A)\cong\frac{\operatorname{Hom}_R(K,A)}{\{\ell j:\ell\in\operatorname{Hom}_R(P,A)\}}.
$$

Indeed a degree-one cocycle in the [Hom functor](../../../../../hom-functor.md) applied to the [projective resolution](../../../../../projective-resolution.md) descends to $K$, while the degree-one coboundaries are exactly restrictions of maps from $P$. This establishes the description of the [Ext functor](../../../../../ext-functor.md) without first assuming the extension classification.

For a [module extension](../../../../../module-extension.md) with inclusion $i:A\to B$ and quotient map $r:B\to C$, projectivity lifts $\pi$ to $s:P\to B$. Since $rsj=0$, there is a unique map $h:K\to A$ with $ih=sj$. A different lift changes $h$ by $\ell j$ for some $\ell:P\to A$. An [equivalence of module extensions](../../../../../equivalence-of-module-extensions.md), which is the identity on both end modules, also preserves this class. We have therefore defined a map from extension classes to $\operatorname{Ext}_R^1(C,A)$.

Conversely, for $h:K\to A$, form the [pushout of a module extension](../../../../../pushout-of-a-module-extension.md)

$$
B_h=(A\oplus P)/\{(h(k),-j(k)):k\in K\}.
$$

The map $A\to B_h$ sends $a$ to $[a,0]$, and $B_h\to C$ sends $[a,p]$ to $\pi(p)$. The first is injective because $j$ is injective. If $\pi(p)=0$, write $p=j(k)$; then $[a,p]=[a+h(k),0]$, proving exactness in the middle. The last map is surjective. Thus $B_h$ is a [module extension](../../../../../module-extension.md). If $h'=h+\ell j$, the map $[a,p]\mapsto[a-\ell(p),p]$ is an [equivalence of module extensions](../../../../../equivalence-of-module-extensions.md) from $B_h$ to $B_{h'}$. Finally $[a,p]\mapsto i(a)+s(p)$ identifies the [pushout of a module extension](../../../../../pushout-of-a-module-extension.md) built from an existing extension with its middle module. These two constructions are inverse, proving **the classification**:

$$
\boxed{\mathcal E(C,A)\ \cong\ \operatorname{Ext}_R^1(C,A).}
$$

The zero class corresponds to a [split short exact sequence](../../../../../split-short-exact-sequence.md). Fixed end modules matter: equivalence does not permit arbitrary automorphisms of $A$ or $C$.

In the second calculation the acting group is the infinite cyclic group. Its modules are modules over the [group ring](../../../../../group-ring.md) $S=\mathbb Z[z,z^{-1}]$, not merely over the underlying ring $\mathbb Z$. The [trivial representation](../../../../../trivial-representation.md) has $z$ acting as the identity. Its [projective resolution](../../../../../projective-resolution.md) is

$$
0\longrightarrow S\xrightarrow{z-1}S\longrightarrow\mathbb Z\longrightarrow0.
$$

Multiplication by $z-1$ is injective, and the augmentation quotient is $\mathbb Z$. Applying the [Hom functor](../../../../../hom-functor.md) into the trivial module makes the differential zero, so $\operatorname{Ext}_S^1(\mathbb Z,\mathbb Z)\cong\mathbb Z$. Taking two copies gives **$\boxed{\mathcal E(\mathbb Z^2,\mathbb Z)\cong\mathbb Z^2}$**.

An explicit representative of this [extension of trivial modules for an infinite cyclic group](../../../../../extension-of-trivial-modules-for-an-infinite-cyclic-group.md) is the abelian group $B_{m,n}=\mathbb Zu\oplus\mathbb Zv\oplus\mathbb Zw$, with injection $1\mapsto u$, quotient $v\mapsto(1,0)$, $w\mapsto(0,1)$, and action

$$
\boxed{zu=u,\qquad zv=v+mu,\qquad zw=w+nu,\qquad(m,n)\in\mathbb Z^2.}
$$

This is an invertible action: the inverse subtracts the same multiples of $u$. Every underlying abelian-group extension splits because $\mathbb Z^2$ is free, so any group-module extension has this form after choosing lifts of the quotient basis. Replacing those lifts by multiples of $u$ does not alter $m,n$. An equivalence fixing the ends has exactly such changes of lifts, so two representatives are equivalent precisely when their ordered pairs agree. Only $(0,0)$ splits as a group-module extension; overlooking the group action would incorrectly give a single class.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
