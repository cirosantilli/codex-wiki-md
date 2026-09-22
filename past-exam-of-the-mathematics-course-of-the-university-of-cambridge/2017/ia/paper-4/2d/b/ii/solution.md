<h1 id="2d/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the value condition, a [function](../../../../../../../function-split.md) agrees with itself outside the empty exceptional [set](../../../../../../../set-split.md), proving the [reflexive relation](../../../../../../../reflexive-relation.md) property. Interchanging the two [functions](../../../../../../../function-split.md) preserves equality, so the same exceptional [finite set](../../../../../../../finite-set.md) proves the [symmetric relation](../../../../../../../symmetric-relation.md) property.

Suppose $(A,f)$ is related to $(B,g)$ and $(B,g)$ to $(C,h)$, with exceptional [finite sets](../../../../../../../finite-set.md) $F_{AB}$ and $F_{BC}$. Points of $A\cap C$ might be absent from $B$, so merely taking $F_{AB}\cup F_{BC}$ would miss a real issue. Use instead

$$
F_{AC}=(A\cap C)\cap\bigl(F_{AB}\cup F_{BC}\cup(A\setminus B)\bigr).
$$

This is a [finite set](../../../../../../../finite-set.md) contained in $A\cap C$: the first two terms are finite by hypothesis and $A\setminus B\subseteq A\mathbin\triangle B$ is finite by the domain condition. If $x\in(A\cap C)\setminus F_{AC}$, then $x\in B$ and neither original exception occurs, so $f(x)=g(x)=h(x)$. The domain condition is also preserved, as proved in the preceding scope. Thus the full relation is a [transitive relation](../../../../../../../transitive-relation.md), and

$$
\boxed{\mathcal R\text{ is an equivalence relation on }\Sigma.}
$$

Finite domains cause no problem: one may take the whole [intersection](../../../../../../../set-intersection.md) as the exceptional [set](../../../../../../../set-split.md). Both conditions are needed for [equivalence of partial functions modulo finite changes](../../../../../../../equivalence-of-partial-functions-modulo-finite-changes.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2D](../../../2d.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ia](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
