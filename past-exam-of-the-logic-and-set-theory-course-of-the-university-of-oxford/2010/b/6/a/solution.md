<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Hartogs theorem](../../../../../hartogs-theorem.md) says that for every set $A$ there is a least [ordinal](../../../../../ordinal-split.md) $h(A)$ that does not inject into $A$. This theorem requires no [axiom of choice](../../../../../axiom-of-choice.md).

To prove it, collect all [well-orderings](../../../../../well-order.md) of subsets of $A$. They are set-sized data, coded by pairs from $\mathcal P(A)$ and $\mathcal P(A\times A)$. Each has a unique [ordinal](../../../../../ordinal-split.md) order type, so replacement gives a set $H$ of their order types. If $\eta\in H$ and $\xi<\eta$, restricting the corresponding [well-order](../../../../../well-order.md) to an initial segment shows $\xi\in H$. Hence $H$ is an [ordinal](../../../../../ordinal-split.md). If this [ordinal](../../../../../ordinal-split.md) itself injected into $A$, its transported [well-order](../../../../../well-order.md) would put $H$ among its own elements, impossible for an [ordinal](../../../../../ordinal-split.md). Every smaller [ordinal](../../../../../ordinal-split.md) does inject by definition. Thus $h(A)=H$ has the asserted property.

**The recursion printed in the source needs two boundary restrictions.** Its new-row successor clause allows $\beta=\alpha$, which would assign a value at $(\alpha,\alpha+1)$ outside the declared domain. Also, at $\alpha=0$, its row-start clause gives $g_1(0,0)=0$ while its column-start clause gives $g_1(0,0)=g_1(0,0)+1$. Taken literally, these clauses do not define a function.

The intended extension fills the new row first and the remaining new column second. Restrict the row successor clause to $\beta<\alpha$, and apply the column-start clause only when $\alpha>0$. With these two restrictions the domains are disjoint:

$$
\alpha\times\alpha,\qquad\{(\alpha,\beta):\beta\leq\alpha\},\qquad
\{(\beta,\alpha):\beta<\alpha\}.
$$

All successors here are [ordinal](../../../../../ordinal-split.md) successors. Simultaneous [transfinite induction](../../../../../transfinite-induction.md) proves a stronger result: $g_\alpha$ is a [bijection](../../../../../bijection.md) of $\alpha\times\alpha$ onto an [ordinal](../../../../../ordinal-split.md) $\gamma_\alpha$, and the functions extend one another.

At zero this is the [empty function](../../../../../empty-function.md). Assuming it at $\alpha$, the least missing [ordinal](../../../../../ordinal-split.md) is $\gamma_\alpha$. Recursion down the new row gives values $\gamma_\alpha+\beta$ for $\beta\leq\alpha$; recursion down the remaining column gives $\gamma_\alpha+(\alpha+1)+\beta$ for $\beta<\alpha$. These enumerate two disjoint consecutive [ordinal](../../../../../ordinal-split.md) intervals above the old range, so the extension is well defined and bijective, with

$$
\boxed{\gamma_{\alpha+1}=\gamma_\alpha+(\alpha+1)+\alpha.}
$$

At a limit $\lambda$, take the union of the earlier functions. Compatibility makes it a function, and every pair of coordinates below $\lambda$ is already present at some earlier stage. Its range is the [ordinal](../../../../../ordinal-split.md) $\bigcup_{\alpha<\lambda}\gamma_\alpha$, and injectivity is preserved by the compatible union. This completes the construction of the [row-and-column enumeration of an ordinal square](../../../../../row-and-column-enumeration-of-an-ordinal-square.md).

For finite stages $\gamma_n=n^2$. For example the table of $g_3$, with the first coordinate indexing rows, is

$$
\begin{pmatrix}0&3&7\\1&2&8\\4&5&6\end{pmatrix}.
$$

The remaining parts refer to this domain-consistent construction. The source's literal boundary claims are preserved in the archive, rather than silently asserted as valid.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
