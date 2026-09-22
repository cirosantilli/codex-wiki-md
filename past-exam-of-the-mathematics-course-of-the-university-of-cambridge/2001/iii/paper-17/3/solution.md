<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\mathcal C$ be a [locally small category](../../../../../locally-small-category.md), let $h_A=\mathcal C(-,A)$ be a [representable presheaf](../../../../../representable-functor.md), and let $X:\mathcal C^{\mathrm{op}}\to\mathbf{Set}$. The [Yoneda lemma](../../../../../yoneda-lemma.md) gives a [bijection](../../../../../bijection.md), natural in $A$ and $X$,

$$
\boxed{\operatorname{Nat}(h_A,X)\cong X(A),\qquad
\alpha\longmapsto\alpha_A(1_A).}
$$

For $x\in X(A)$, define a [natural transformation](../../../../../natural-transformation.md) $\alpha^x:h_A\to X$ by

$$
\alpha^x_B(f)=X(f)(x)\qquad(f:B\to A).
$$

For $v:C\to B$, the [functor](../../../../../functor.md) composition law gives $X(v)\alpha^x_B(f)=X(fv)(x)=\alpha^x_C(fv)$, proving [naturality](../../../../../naturality.md). Conversely, naturality of any $\alpha:h_A\to X$ along $f:B\to A$ gives

$$
\alpha_B(f)=X(f)\alpha_A(1_A).
$$

Thus $\alpha$ is determined by its displayed element, and $\alpha^x_A(1_A)=x$ proves that the constructions are inverse.

A [natural transformation](../../../../../natural-transformation.md) $\theta:X\to Y$ sends the element to $\theta_A(x)$, which corresponds to $\theta\alpha^x$. A [morphism](../../../../../morphism.md) $u:A'\to A$ induces $h_u:h_{A'}\to h_A$; precomposition by $h_u$ sends the element to $X(u)(x)$. This proves naturality in both variables and completes the [Yoneda lemma](../../../../../yoneda-lemma.md) proof.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
