<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [preadditive category](../../../../../preadditive-category.md) has an abelian-group structure on every [hom-set](../../../../../hom-set.md) and bilinear composition. One equivalent definition of an [additive category](../../../../../additive-category.md) is a [preadditive category](../../../../../preadditive-category.md) with a [zero object](../../../../../zero-object.md) and finite [products in a category](../../../../../product-category-theory.md); the following argument proves that these [products in a category](../../../../../product-category-theory.md) are automatically [coproducts in a category](../../../../../coproduct.md). An [abelian category](../../../../../abelian-category.md) is an [additive category](../../../../../additive-category.md) with kernels and cokernels in which every [monomorphism](../../../../../monomorphism.md) is a kernel and every [epimorphism](../../../../../epimorphism.md) is a cokernel. Equivalently, for every arrow the canonical map from its coimage to its image is invertible.

Let $P=\prod_{i=1}^nA_i$, with projections $p_i$. Define $\iota_i:A_i\to P$ by $p_j\iota_i=\delta_{ji}$, where the diagonal entry is the identity and the others are zero. Since its composites with all projections are identities,

$$
\sum_i\iota_ip_i=1_P.
$$

Given $f_i:A_i\to B$, the map $f=\sum_if_ip_i$ satisfies $f\iota_i=f_i$. If another map has those composites, multiplying the displayed identity by that map forces it to equal $f$. Thus $P$ is also a [coproduct in a category](../../../../../coproduct.md). The empty case is the [zero object](../../../../../zero-object.md). Reversing arrows proves that a finite [coproduct in a category](../../../../../coproduct.md) is likewise a [product in a category](../../../../../product-category-theory.md). Hence **finite [products in a category](../../../../../product-category-theory.md) and [coproducts in a category](../../../../../coproduct.md) are canonically [biproducts](../../../../../biproduct.md)** in an [additive category](../../../../../additive-category.md).

For the [category of abelian groups](../../../../../category-of-abelian-groups.md), let $(A_i,D_{ij})$ be a directed diagram, with no injectivity assumption on its transition maps. Its set [colimit](../../../../../colimit.md) consists of classes $[i,a]$, with

$$
[i,a]=[j,b]\quad\Longleftrightarrow\quad D_{ik}a=D_{jk}b\text{ for some }k\geq i,j.
$$

Directedness proves transitivity of this relation. Define addition by moving representatives to a common upper index:

$$
[i,a]+[j,b]=[k,D_{ik}a+D_{jk}b].
$$

Moving all indices involved to one further upper bound proves independence of representatives and of $k$. Define $-[i,a]=[i,-a]$ and use the common class of the zeros as zero. The abelian-group laws hold at a common index, so descend to the quotient. Every canonical map $A_i\to C$ is a homomorphism, and a compatible cocone induces the homomorphism $[i,a]\mapsto f_i(a)$. This is the unique extension. Moreover the formula for addition is forced by those canonical homomorphisms, proving that the underlying-set [functor](../../../../../functor.md) creates directed [colimits](../../../../../colimit.md). This establishes [directed colimits created by the abelian-group forgetful functor](../../../../../directed-colimits-created-by-the-abelian-group-forgetful-functor.md) explicitly.

If a cocone $\nu_i:A_i\to B$ has injective legs, the induced map $C\to B$ is injective. Indeed, equal images of $[i,a]$ and $[j,b]$ give, at a common index $k$,

$$
\nu_k(D_{ik}a)=\nu_i(a)=\nu_j(b)=\nu_k(D_{jk}b).
$$

Injectivity of $\nu_k$ gives equal representatives at $k$. Since [monomorphisms](../../../../../monomorphism.md) of [abelian groups](../../../../../abelian-group.md) are exactly injective homomorphisms, we have proved that **the [category of abelian groups](../../../../../category-of-abelian-groups.md) is a finitary [abelian category](../../../../../abelian-category.md)** in the directed-union sense of the question.

Now let $\mathcal A$ be complete, cocomplete and finitary. Index by finite subsets $J\subseteq I$ and put $S_J=\bigoplus_{j\in J}A_j$. For $J\subseteq K$, insert the additional zero coordinates. A compatible cocone on these finite [biproducts](../../../../../biproduct.md) is exactly a family of maps from every $A_i$, so their directed [colimit](../../../../../colimit.md) is $S=\coprod_{i\in I}A_i$.

Each finite [biproduct](../../../../../biproduct.md) has a map $k_J:S_J\to P=\prod_{i\in I}A_i$ using its coordinates in $J$ and zeros outside $J$. Projection to the finite set of coordinates in $J$ is a retraction, so $k_J$ is a [split monomorphism](../../../../../split-monomorphism.md). These maps form a cocone of [monomorphisms](../../../../../monomorphism.md). The finitary property makes its induced map a [monic arrow](../../../../../monomorphism.md), and that induced map is exactly the canonical infinite identity matrix:

$$
\boxed{j:\coprod_{i\in I}A_i\longrightarrow\prod_{i\in I}A_i\text{ is monic}.}
$$

This proves the [coproduct-to-product comparison in a finitary abelian category](../../../../../coproduct-to-product-comparison-in-a-finitary-abelian-category.md). The PDF's use of finite [products in a category](../../../../../product-category-theory.md) in the hint is valid because these are the same finite [biproducts](../../../../../biproduct.md).

If $\mathcal A$ is also a [cofinitary abelian category](../../../../../cofinitary-abelian-category.md), apply this argument in its opposite [category](../../../../../category-split.md). The same canonical comparison $j$ is then an [epic arrow](../../../../../epimorphism.md) in $\mathcal A$. In an [abelian category](../../../../../abelian-category.md) an arrow that is both a [monomorphism](../../../../../monomorphism.md) and an [epimorphism](../../../../../epimorphism.md) is invertible, so $j$ is an isomorphism.

For countably many copies of $A$, put $S=\coprod_{n\geq0}A$ and let $q=j^{-1}\Delta:A\to S$, where $\Delta$ is the [product in a category](../../../../../product-category-theory.md) diagonal. Let $\iota_n$ denote the [coproduct in a category](../../../../../coproduct.md) injections, let $s:S\to S$ shift them by $s\iota_n=\iota_{n+1}$, and let $\nabla:S\to A$ be the codiagonal. Comparing every [product in a category](../../../../../product-category-theory.md) coordinate gives

$$
jq=j\iota_0+jsq.
$$

Since $j$ is a [monic arrow](../../../../../monomorphism.md), $q=\iota_0+sq$. Also $\nabla\iota_0=1_A$ and $\nabla s=\nabla$. Therefore, for $z=\nabla q$,

$$
z=1_A+z.
$$

[Hom-sets](../../../../../hom-set.md) are [abelian groups](../../../../../abelian-group.md), so cancellation gives $1_A=0$. Any arrow to or from $A$ is consequently zero by composition with its identity. Thus every object is both initial and terminal, and

$$
\boxed{\mathcal A\text{ is degenerate: every object is a zero object}.}
$$

This is the countable shift-and-fold argument behind [countable biproducts in an additive category force triviality](../../../../../countable-biproducts-in-an-additive-category-force-triviality.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
