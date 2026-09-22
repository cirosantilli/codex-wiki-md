# Product (category theory)

↑ **Parent:** [Finite limit](finite-limit.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Product_(category_theory))

A binary categorical product of [objects of a category](object-of-a-category.md) $A,B$ is an object $P$ with [categorical morphisms](morphism-in-a-category.md) $p_A:P\to A$ and $p_B:P\to B$. Its [universal property](universal-property.md) is that, for every object $X$ and pair of arrows $f:X\to A$, $g:X\to B$, there is exactly one arrow $h:X\to P$ satisfying

$$
p_A\circ h=f,\qquad p_B\circ h=g.
$$

The arrows $p_A,p_B$ are called the product projections. Existence lets us combine two maps; uniqueness means there is no extra unspecified information in the combined map.

In the [Category of sets](category-of-sets.md), take $A=\{0,1\}$ and $B=\{a,b,c\}$. Their [Cartesian product](cartesian-product.md) contains six [ordered pairs](ordered-pair.md), and the [projection maps](projection-map.md) select the first and second coordinates. Let $X=\{u,v,w\}$, $f(u)=0$, $f(v)=1$, $f(w)=1$, and $g(u)=a$, $g(v)=b$, $g(w)=a$. The unique required map is **$h(u)=(0,a)$, $h(v)=(1,b)$, $h(w)=(1,a)$**. Reading either coordinate recovers the corresponding input map.

<a id="image-two-maps-into-the-factors-determine-exactly-one-map-into-their-six-element-cartesian-product"></a>
![](categorical-product-factorization.png)

**[Figure 2](#image-two-maps-into-the-factors-determine-exactly-one-map-into-their-six-element-cartesian-product). Two maps into the factors determine exactly one map into their six-element Cartesian product**.

In a [partially ordered set](partially-ordered-set.md) viewed as a [category](category-split.md), the projection arrows mean $P\leq A$ and $P\leq B$. The [universal property](universal-property.md) says that every common [lower bound](lower-bound-in-a-partially-ordered-set.md) $X$ satisfies $X\leq P$, so $P$ is the [greatest lower bound](greatest-lower-bound-in-a-partially-ordered-set.md). For [subsets](subset.md) ordered by inclusion this is $A\cap B$, the [intersection](set-intersection.md); it is a different construction from the [Cartesian product](cartesian-product.md) in the [Category of sets](category-of-sets.md) because the allowed arrows have changed.

The [universal property](universal-property.md) also compares any two proposed products: each supplies a unique map to the other compatible with the projections. The two composites have the same projections as the corresponding [identity morphisms](identity-morphism.md), so uniqueness makes them identities. Thus a [categorical product](product-category-theory.md) is determined up to a unique projection-preserving [isomorphism](isomorphism.md), which explains why we can use whichever concrete construction is convenient.

**Table of contents**

- [Categorical diagonal](categorical-diagonal.md)

## ↑ Ancestors (10)

1. [Finite limit](finite-limit.md)
2. [Categorical limit](categorical-limit.md)
3. [Cone over a diagram](cone-over-a-diagram.md)
4. [Diagram (category theory)](diagram-category-theory.md)
5. [Category](category-split.md)
6. [Category theory](category-theory-split.md)
7. [Foundations of mathematics](foundations-of-mathematics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)
