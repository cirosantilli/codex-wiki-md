<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First address the unnumbered preliminaries. The **[Yoneda lemma](../../../../../../yoneda-lemma.md)** gives a [natural transformation](../../../../../../natural-transformation.md) bijection

$$
\boxed{\operatorname{Nat}(\mathcal C(A,-),F)\cong F(A),\qquad\tau\longmapsto\tau_A(1_A).}
$$

The element $x\in F(A)$ corresponds to $\tau_B(f)=F(f)(x)$ for $f:A\to B$. These bijections are natural in $A$ and $F$; the contravariant form replaces $\mathcal C(A,-)$ by $\mathcal C(-,A)$.

Let $E=(1\downarrow F)$ be the [category of elements](../../../../../../category-of-elements.md). Its objects are $(A,x)$ with $x\in F(A)$; an arrow $u:(A,x)\to(B,y)$ is $u:A\to B$ with $F(u)(x)=y$. Since $\mathcal C$ is a [small category](../../../../../../small-category.md), $E$ is small. Define a [diagram in a category](../../../../../../diagram-category-theory.md) $D:E^{\mathrm{op}}\to[\mathcal C,\mathbf{Set}]$ by

$$
D(A,x)=\mathcal C(A,-).
$$

For the opposite of $u$, the map $\mathcal C(B,-)\to\mathcal C(A,-)$ is precomposition with $u$. The [Yoneda lemma](../../../../../../yoneda-lemma.md) gives a [cocone under a diagram](../../../../../../cocone-under-a-diagram.md) $D\to F$ whose $(A,x)$ component sends $f:A\to B$ to $F(f)(x)$.

For any $G$, a competing [cocone under a diagram](../../../../../../cocone-under-a-diagram.md) amounts, by the [Yoneda lemma](../../../../../../yoneda-lemma.md), to elements $z_{A,x}\in G(A)$ satisfying

$$
G(u)(z_{A,x})=z_{B,F(u)(x)}.
$$

This is exactly the [naturality](../../../../../../naturality.md) condition for $\alpha_A:F(A)\to G(A)$ defined by $\alpha_A(x)=z_{A,x}$. It gives a unique [natural transformation](../../../../../../natural-transformation.md) $\alpha:F\to G$ factoring the cocone. Thus the [universal property](../../../../../../universal-property.md) of a [colimit](../../../../../../colimit.md) proves the [canonical colimit presentation of a covariant set-valued functor](../../../../../../canonical-colimit-presentation-of-a-covariant-set-valued-functor.md):

$$
\boxed{F\cong\operatorname*{colim}_{(A,x)\in E^{\mathrm{op}}}\mathcal C(A,-).}
$$

The opposite on $E$ is essential for the variance of the [representable functors](../../../../../../representable-functor.md).

We now prove the four conditions equivalent by the cycle $(i)\Rightarrow(ii)\Rightarrow(iii)\Rightarrow(iv)\Rightarrow(i)$. Suppose $F$ is a [finite-limit-preserving set-valued functor](../../../../../../finite-limit-preserving-set-valued-functor.md). For a finite [diagram in a category](../../../../../../diagram-category-theory.md) in the [comma category](../../../../../../comma-category.md) $(S\downarrow F)$, write its objects as $(A_i,s_i:S\to F(A_i))$. Take $L=\lim_i A_i$ in $\mathcal C$. Since $F$ preserves this [finite limit](../../../../../../finite-limit.md), the compatible maps $s_i$ determine a unique $s:S\to F(L)$ whose composites with $F(L)\to F(A_i)$ are $s_i$. The pair $(L,s)$ has the required [categorical limit](../../../../../../categorical-limit.md) property in $(S\downarrow F)$, by the same universal properties. For the empty diagram, $F(1)$ is a singleton, so there is exactly one map $S\to F(1)$; this provides the [terminal object](../../../../../../terminal-object.md). Hence **$(i)\Rightarrow(ii)$ for every set $S$**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
