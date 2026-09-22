<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here the Hom groups must be taken over $A$; the printed subscript $B$ in this part has no defined coefficient ring. For an arbitrary [module](../../../../../../module-mathematics.md) $P$, form the [free module](../../../../../../free-module.md)

$$
F=\bigoplus_{p\in P}Ae_p,
$$

and define a [module homomorphism](../../../../../../module-homomorphism.md) $\pi:F\to P$ by $e_p\mapsto p$. Each element of $F$ has finite support, so this prescription extends uniquely and is well-defined. It is [surjective](../../../../../../surjective-function.md) because every $p\in P$ is the image of $e_p$. Thus every module is a quotient of a [free module](../../../../../../free-module.md).

Let $K=\ker\pi$. The [short exact sequence](../../../../../../short-exact-sequence.md) $0\to K\to F\xrightarrow{\pi}P\to0$ and the defining exactness condition for a [projective module](../../../../../../projective-module.md) make

$$
\operatorname{Hom}_A(P,F)\longrightarrow\operatorname{Hom}_A(P,P),\qquad s\longmapsto\pi s
$$

[surjective](../../../../../../surjective-function.md). Lift $1_P$ to a map $s:P\to F$. Then $\pi s=1_P$, so $s$ is [injective](../../../../../../injective-function.md). Every $f\in F$ has the decomposition

$$
f=(f-s\pi(f))+s\pi(f),
$$

whose first term lies in $K$ and second lies in $s(P)$. If $s(p)\in K$, applying $\pi$ gives $p=0$, so the intersection is zero. Consequently

$$
\boxed{F=K\oplus s(P)\cong K\oplus P.}
$$

This is a [split short exact sequence](../../../../../../split-short-exact-sequence.md) and proves that [projective modules are direct summands of free modules](../../../../../../projective-modules-are-direct-summands-of-free-modules.md), including modules that are not finitely generated.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
