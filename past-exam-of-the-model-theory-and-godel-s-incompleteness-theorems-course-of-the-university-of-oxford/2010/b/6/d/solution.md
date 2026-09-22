<h1 id="b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**For the pure orders, yes.** Both structures satisfy the theory of [dense linear orders without endpoints](../../../../../dense-linear-order-without-endpoints.md). By [quantifier elimination for dense linear orders without endpoints](../../../../../quantifier-elimination-for-dense-linear-orders-without-endpoints.md), each formula is equivalent to a quantifier-free order formula. Inclusion of the rationals into the reals preserves and reflects all such formulas, hence is elementary:

$$
\boxed{(\mathbb Q,<)\preccurlyeq(\mathbb R,<).}
$$

**With a common named unit, yes.** In general an [elementary substructure](../../../../../elementary-substructure.md) remains elementary when elements already in the [substructure](../../../../../substructure-of-a-first-order-structure.md) are named by new constants. A formula using the new constant is just an old-language formula with that common element as a parameter. Since $1\in\mathbb Q$, this applies directly.

**With the real constant interpreted by $\pi$, no choice inside the rationals works for inclusion.** A [substructure](../../../../../substructure-of-a-first-order-structure.md) embedding must preserve every constant. The inclusion would send a rational interpretation $q$ to that same real $q$, whereas the target constant is $\pi\notin\mathbb Q$. Thus the expanded rational structure is not even a [substructure](../../../../../substructure-of-a-first-order-structure.md) of the expanded real one.

This last failure concerns the specified inclusion. There is an abstract [elementary embedding](../../../../../elementary-embedding.md) carrying a chosen rational $q$ to $\pi$: the increasing map $r\mapsto r+\pi-q$ has that property, and its image is a dense order without endpoints inside the reals. [Quantifier elimination](../../../../../quantifier-elimination.md) makes the embedding elementary, but its image is a translated copy of the rationals rather than the original rational subset.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
