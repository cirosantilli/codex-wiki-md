<h1 id="a/3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**No such first-order axiom collection can force actual identity when the displayed symbol is treated as an ordinary relation.** The [duplication obstruction to axiomatizing identity](../../../../../../duplication-obstruction-to-axiomatizing-identity.md) proves this even for an infinite collection of extra axioms.

Start with any nonempty [first-order structure](../../../../../../first-order-structure.md) $\mathcal A$ in which the symbol is identity. Form $B=A\times\{0,1\}$ and the surjection $\pi:B\to A$. Interpret each relation by pulling it back along $\pi$; in particular,

$$
E^{\mathcal B}((a,i),(b,j))\iff a=b.
$$

Interpret every function on first coordinates as in $\mathcal A$ and choose second coordinate zero; likewise lift constants with second coordinate zero. Induction on [first-order terms](../../../../../../first-order-term.md) gives $\pi(t^{\mathcal B}(v))=t^{\mathcal A}(\pi v)$. Induction on [first-order formulas](../../../../../../first-order-formula.md) then gives

$$
\mathcal B\models\theta[v]\iff\mathcal A\models\theta[\pi v].
$$

The quantifier steps use surjectivity of $\pi$, so every witness in $A$ lifts to $B$.

Every proposed axiom valid with actual equality is therefore true in $\mathcal B$ under every assignment, along with A1–A7. But $E^{\mathcal B}((a,0),(a,1))$ holds for two different domain elements. Thus those axioms cannot enforce identity. The usual interpretation of [logical equality](../../../../../../logical-equality.md) as identity is a semantic requirement.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the logic and set theory course of the University of Oxford](../../../../../split.md)
7. [Logic and set theory course of the University of Oxford](../../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
