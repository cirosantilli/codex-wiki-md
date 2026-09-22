<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Pullback and [tensor product](../../../../../../tensor-product.md) preserve [holomorphic line bundles](../../../../../../holomorphic-line-bundle.md) and their isomorphisms. Interpret negative tensor powers of $L$ as powers of $L^*$. Thus the formula defines a group homomorphism on isomorphism classes.

To prove injectivity, suppose $p^*M\otimes L^{\otimes n}$ is trivial. Restrict it to any fibre. A line pulled back from its base point is trivial there, so its fibre restriction is $\mathcal O_{\mathbb P^1}(n)$. By the [Picard group](../../../../../../picard-group.md) classification, $n=0$. It remains to show that $p^*M$ trivial implies $M$ trivial.

Let $\sigma$ be a nowhere-zero holomorphic section of $p^*M$. On a sufficiently small open set where both $E$ and $M$ are trivial, write $\sigma=a_i(x,[v])p^*e_i$ for a frame $e_i$ of $M$. For each fixed $x$, $a_i(x,\cdot)$ is a [holomorphic function](../../../../../../holomorphic-function.md) on the compact [complex projective line](../../../../../../complex-projective-line.md), hence is constant. It is therefore $b_i(x)$; evaluating at a constant projective point in the local trivialization shows $b_i$ is holomorphic in $x$. The section is nowhere zero, so each $b_i$ is nowhere zero. Its overlap laws are exactly those of a section of $M$, and $b_ie_i$ glue to a global holomorphic frame. Thus $M$ is trivial.

The kernel consists only of $(\mathcal O_X,0)$, proving

$$
 \boxed{\operatorname{Pic}_{\rm hol}(X)\times\mathbb Z
 \hookrightarrow\operatorname{Pic}_{\rm hol}(\mathbb P(E)).}
$$

This is the [Picard injection for holomorphic projective bundles](../../../../../../picard-injection-for-holomorphic-projective-bundles.md). The argument uses local fibrewise constancy, so no global section of the [projective bundle](../../../../../../projective-bundle.md) is required.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
