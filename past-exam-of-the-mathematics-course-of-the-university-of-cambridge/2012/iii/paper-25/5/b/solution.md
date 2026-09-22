<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose $G$ is a [representable functor](../../../../../../representable-functor.md), with a [natural isomorphism](../../../../../../natural-isomorphism.md) $\theta:\mathcal C(R,-)\to G$. Put $r=\theta_R(1_R)$. For any $(A,a)$ in the [comma category](../../../../../../comma-category.md) $(1\downarrow G)$, the representing [bijection](../../../../../../bijection.md) gives a unique $f:R\to A$ with $\theta_A(f)=a$. By [naturality](../../../../../../naturality.md), $\theta_A(f)=G(f)(r)$, exactly the condition for $f:(R,r)\to(A,a)$. Hence $(R,r)$ is an [initial object](../../../../../../initial-object.md).

Conversely, if $(R,r)$ is an [initial object](../../../../../../initial-object.md), then

$$
\boxed{\theta_A:\mathcal C(R,A)\longrightarrow G(A),\qquad f\longmapsto G(f)(r)}
$$

is a [bijection](../../../../../../bijection.md) for each $A$: existence and uniqueness are precisely initiality applied to every $(A,a)$. For $h:A\to B$, $G(h)\theta_A(f)=G(hf)(r)=\theta_B(hf)$, proving [naturality](../../../../../../naturality.md). Thus $r$ is a [universal element](../../../../../../universal-element-of-a-set-valued-functor.md) and $\theta$ is a [representation of a functor](../../../../../../representation-of-a-functor.md). **Being [representable](../../../../../../representable-functor.md) is equivalent to the singleton [comma category](../../../../../../comma-category.md) having an [initial object](../../../../../../initial-object.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
