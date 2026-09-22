<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [morphism of schemes](../../../../morphism-of-schemes.md) $f:X\to Y$ defines a [natural transformation](../../../../natural-transformation.md) $g_f:g_X\to g_Y$ by $u\mapsto f\circ u$. We construct the inverse correspondence.

Let $\alpha:g_X\to g_Y$ be a [natural transformation](../../../../natural-transformation.md), and choose an [affine open cover](../../../../affine-open-cover.md) $(j_i:U_i\hookrightarrow X)$. Regard $j_i$ as an element of $g_X(U_i)$ and set

$$
f_i=\alpha_{U_i}(j_i):U_i\longrightarrow Y.
$$

Here and below the [equivalence of categories](../../../../equivalence-of-categories.md) in the question lets us write the restricted [functor of points](../../../../functor-represented-by-a-scheme.md) on [affine schemes](../../../../affine-scheme.md), contravariantly, rather than on [commutative rings](../../../../commutative-ring.md), covariantly. If $W\subseteq U_i\cap U_j$ is an [affine open subscheme](../../../../affine-open-subscheme.md), [naturality](../../../../naturality.md) for its two inclusions gives

$$
f_i|_W=\alpha_W(W\hookrightarrow X)=f_j|_W.
$$

Such $W$ cover the overlap even when that overlap is not an [affine scheme](../../../../affine-scheme.md). Consequently the $f_i$ agree and glue to a [morphism of schemes](../../../../morphism-of-schemes.md) $f:X\to Y$.

It remains to check all elements of the restricted [functor of points](../../../../functor-represented-by-a-scheme.md), not only the chosen inclusions. Given an [affine scheme](../../../../affine-scheme.md) $T$ and $u:T\to X$, cover each $u^{-1}(U_i)$ by [affine open subschemes](../../../../affine-open-subscheme.md) $V$. On such a $V$, factor $u|_V=j_i\circ v$. Applying [naturality](../../../../naturality.md) first to $v:V\to U_i$ and then to $V\hookrightarrow T$ gives

$$
\alpha_T(u)|_V=\alpha_V(u|_V)=\alpha_{U_i}(j_i)\circ v=f\circ u|_V.
$$

These local equalities prove $\alpha_T(u)=f\circ u$. The glued $f$ is unique, since its restrictions to all $U_i$ are prescribed. Hence

$$
\boxed{\operatorname{Hom}_{\mathsf{Sch}}(X,Y)\cong\operatorname{Nat}(g_X,g_Y),}
$$

so the assignment is [fully faithful](../../../../full-and-faithful-functor.md).

If $g_X\cong g_Y$, the [natural isomorphism](../../../../natural-isomorphism.md) and its inverse correspond to [morphisms of schemes](../../../../morphism-of-schemes.md) $f:X\to Y$ and $h:Y\to X$. Their compositions induce the identity [natural transformations](../../../../natural-transformation.md), and faithfulness implies $hf=\operatorname{id}_X$, $fh=\operatorname{id}_Y$. Conversely, an [isomorphism of schemes](../../../../isomorphism-of-schemes.md) induces a [natural isomorphism](../../../../natural-isomorphism.md). Thus

$$
\boxed{X\cong Y\iff g_X\cong g_Y.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
