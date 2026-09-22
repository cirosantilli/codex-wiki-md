<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\mathbb P^r=\mathbb P^r_k$ over its ground [field](../../../../field.md); the argument also works over any [Noetherian](../../../../noetherian-ring.md) affine base. Since $\iota$ is a [closed immersion](../../../../closed-immersion.md), $X$ is a [noetherian scheme](../../../../noetherian-scheme.md) and a [quasi-compact scheme](../../../../quasi-compact-scheme.md). Let

$$
L=\iota^*\mathcal O_{\mathbb P^r}(1),\qquad F(n)=F\otimes_{\mathcal O_X}L^{\otimes n}.
$$

Here the [pullback of a sheaf of modules](../../../../pullback-of-a-sheaf-of-modules.md) makes $L$ an [invertible sheaf](../../../../line-bundle.md), the restriction of the [twisting sheaf on projective space](../../../../twisting-sheaf-on-projective-space.md). It is an [ample line bundle](../../../../ample-line-bundle.md).

By [global generation by sufficiently positive twists](../../../../global-generation-by-sufficiently-positive-twists.md), choose $n\geq0$ such that $F(n)$ is a [globally generated sheaf](../../../../globally-generated-sheaf.md). Finitely many [global sections](../../../../global-section.md) suffice: at each point, finite generation of the [stalk](../../../../stalk-of-a-sheaf.md) of the [coherent sheaf](../../../../coherent-sheaf.md) $F(n)$ lets us select finitely many generating germs of [global sections](../../../../global-section.md). Those sections generate on a neighbourhood, because their [cokernel sheaf](../../../../cokernel-sheaf.md) is a [coherent sheaf](../../../../coherent-sheaf.md) with zero [stalk](../../../../stalk-of-a-sheaf.md) at that point. A finite subcover, using that $X$ is a [quasi-compact scheme](../../../../quasi-compact-scheme.md), supplies finitely many [global sections](../../../../global-section.md) generating everywhere. This is [finite global generation on a quasi-compact scheme](../../../../finite-global-generation-on-a-quasi-compact-scheme.md), and gives a surjective [sheaf morphism](../../../../morphism-of-sheaves.md)

$$
\mathcal O_X^{\oplus m}\twoheadrightarrow F(n).
$$

Tensor with $(L^\vee)^{\otimes n}$, where $L^\vee$ is the [dual of a sheaf](../../../../dual-of-a-sheaf.md). Here [tensoring with an invertible sheaf is exact](../../../../tensoring-with-an-invertible-sheaf-is-exact.md): locally the [tensor product of sheaves](../../../../tensor-product-of-sheaves.md) is tensoring with a free module of rank one. Using the permitted identity $L\otimes L^\vee\cong\mathcal O_X$, we obtain

$$
\boxed{G=\bigl((L^\vee)^{\otimes n}\bigr)^{\oplus m}=\mathcal O_X(-n)^{\oplus m},\qquad G\twoheadrightarrow F\longrightarrow0.}
$$

A finite [direct sum of sheaves](../../../../direct-sum-of-sheaves.md) of [invertible sheaves](../../../../line-bundle.md) is a [locally free sheaf](../../../../locally-free-sheaf.md) of finite rank, and it is a [coherent sheaf](../../../../coherent-sheaf.md) on the [noetherian scheme](../../../../noetherian-scheme.md) $X$. This constructs the required $G$. No regularity or smoothness assumption on $X$ is needed.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
