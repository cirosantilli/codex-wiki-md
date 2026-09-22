<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [diagram in a category](../../../../../diagram-category-theory.md) of shape $J$ is a [functor](../../../../../functor.md) $D:J\to\mathcal C$. A [categorical cone](../../../../../cone-over-a-diagram.md) with vertex $X$ is a family $\gamma_j:X\to Dj$ satisfying $D(a)\gamma_j=\gamma_k$ for every $a:j\to k$. A [morphism](../../../../../morphism.md) between [categorical cones](../../../../../cone-over-a-diagram.md) from $(X,\gamma)$ to $(Y,\delta)$ is a [morphism](../../../../../morphism.md) $u:X\to Y$ with $\delta_ju=\gamma_j$ for all $j$. A [categorical limit](../../../../../categorical-limit.md) is a [terminal object](../../../../../terminal-object.md) in this [category](../../../../../category-split.md) of cones: each cone has a unique such [morphism](../../../../../morphism.md) to the limiting cone.

For a finite $J$, form the [products in a category](../../../../../product-category-theory.md)

$$
P=\prod_{j\in\operatorname{ob}J}Dj,\qquad Q=\prod_{a:j\to k}Dk.
$$

Define $s,t:P\rightrightarrows Q$ with $a$-coordinates $D(a)\pi_j$ and $\pi_k$. The [equalizer](../../../../../equaliser.md) $e:L\to P$ imposes exactly the cone equations. Therefore $\pi_je$ gives a [categorical limit](../../../../../categorical-limit.md) of $D$, since maps into $P$ encode families of legs and factoring through $e$ encodes their compatibility. The empty [product in a category](../../../../../product-category-theory.md) is the [terminal object](../../../../../terminal-object.md), covering the empty diagram. This is the [construction of small limits from products and equalizers](../../../../../construction-of-small-limits-from-products-and-equalizers.md), restricted to finite shapes.

Now take an [initial functor](../../../../../initial-functor.md) $F:I\to J$ and a [categorical cone](../../../../../cone-over-a-diagram.md) $\delta_i:X\to DFi$ over $DF$. For each $j$ and each object $(i,u:Fi\to j)$ of the [comma category](../../../../../comma-category.md) $(F\downarrow j)$, consider $D(u)\delta_i$. A [morphism](../../../../../morphism.md) $a:(i,u)\to(i',u')$ there satisfies $u'F(a)=u$, so

$$
D(u')\delta_{i'}=D(u')D(Fa)\delta_i=D(u)\delta_i.
$$

Since $(F\downarrow j)$ is a nonempty [connected category](../../../../../connected-category.md), this common value is independent of the object. Define it to be $\gamma_j$. This does not require choosing representatives: the value is uniquely determined.

For $b:j\to k$, replacing $(i,u)$ by $(i,bu)$ proves $D(b)\gamma_j=\gamma_k$. Taking $(i,1_{Fi})$ proves $\gamma_{Fi}=\delta_i$. Conversely, extending a restricted cone recovers its original legs, since $\gamma_j=D(u)\gamma_{Fi}$. A vertex [morphism](../../../../../morphism.md) commuting with every $\delta_i$ also commutes with each $\gamma_j=D(u)\delta_i$, and the converse follows by restriction. Thus extension and restriction are strictly inverse [functors](../../../../../functor.md), not merely an [equivalence of categories](../../../../../equivalence-of-categories.md). This proves [cone restriction along an initial functor](../../../../../cone-restriction-along-an-initial-functor.md).

If $\mathcal C$ has all [categorical limits](../../../../../categorical-limit.md) of shape $I$, transport a [terminal object](../../../../../terminal-object.md) in the cone category of $DF$ across this isomorphism to obtain a [categorical limit](../../../../../categorical-limit.md) of $D$. Uniqueness of the induced comparison, and its compatibility with [natural transformations](../../../../../natural-transformation.md) of diagrams, gives

$$
\boxed{\lim_J\cong\lim_I\circ F^*.}
$$

For the converse use the [representable test for initial functors](../../../../../representable-test-for-initial-functors.md). For $j\in J$, the [representable presheaf](../../../../../representable-functor.md) $J(-,j):J^{\mathrm{op}}\to\mathbf{Set}$ is equivalently a [diagram in a category](../../../../../diagram-category-theory.md) $D_j:J\to\mathbf{Set}^{\mathrm{op}}$. Its [categorical limit](../../../../../categorical-limit.md) in the [opposite category](../../../../../opposite-category.md) is the [colimit](../../../../../colimit.md) of $J(-,j)$ in [sets](../../../../../set-split.md). Elements of that [colimit](../../../../../colimit.md) are connected components of the [category of elements](../../../../../category-of-elements.md), equivalently of the [opposite category](../../../../../opposite-category.md) of the slice $J\downarrow j$. This slice has [terminal object](../../../../../terminal-object.md) $(j,1_j)$, so that [colimit](../../../../../colimit.md) is a singleton.

For the restricted presheaf $J(F(-),j)$, the same description identifies its [colimit](../../../../../colimit.md) with the connected-component [set](../../../../../set-split.md) of $(F\downarrow j)$. Indeed a relation identifying $u':Fi'\to j$ with $u'F(a):Fi\to j$ is exactly a generating edge of the zigzag relation in this [comma category](../../../../../comma-category.md). The assumed isomorphism of limit [functors](../../../../../functor.md) forces this [set](../../../../../set-split.md) to be a singleton. Therefore $(F\downarrow j)$ is nonempty and connected for every $j$, proving

$$
\boxed{F\text{ is initial}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
