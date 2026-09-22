<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [categorical presheaf](../../../../../../presheaf-category-theory.md) $X:\mathcal C^{\mathrm{op}}\to\mathbf{Set}$ and $A\in\mathcal C$, the [Yoneda lemma](../../../../../../yoneda-lemma.md) gives a [natural bijection](../../../../../../natural-bijection.md)

$$
\operatorname{Nat}(\mathcal C(-,A),X)\cong X(A),\qquad \theta\longmapsto\theta_A(1_A).
$$

To construct its inverse, take $x\in X(A)$ and [set](../../../../../../set-split.md) $\theta^x_U(h)=X(h)x$ for $h:U\to A$. For $k:V\to U$, the [functor](../../../../../../functor.md) law gives $X(k)\theta^x_U(h)=X(hk)x=\theta^x_V(hk)$, so $\theta^x$ is a [natural transformation](../../../../../../natural-transformation.md). Conversely, [naturality](../../../../../../naturality.md) of any $\theta$ at $h:U\to A$ gives $\theta_U(h)=X(h)\theta_A(1_A)$. Thus the two constructions are inverse, proving the [bijection](../../../../../../bijection.md).

The [bijection](../../../../../../bijection.md) is natural in $X$: a [natural transformation](../../../../../../natural-transformation.md) $t:X\to Y$ sends the distinguished element $x$ to $t_A(x)$ on either side. It is natural in $A$: for $f:A\to B$, precomposing a transformation $\mathcal C(-,B)\to X$ with postcomposition by $f$ sends its distinguished element $x\in X(B)$ to $X(f)x$. These equations prove the claimed [naturality](../../../../../../naturality.md), rather than just an objectwise correspondence. Reversing [morphisms](../../../../../../morphism.md) gives the covariant form $\operatorname{Nat}(\mathcal C(A,-),Z)\cong Z(A)$ for $Z:\mathcal C\to\mathbf{Set}$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
