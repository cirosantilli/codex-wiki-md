<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $d_e=\operatorname{depth}(e)$ and $d_f=\operatorname{depth}(f)$ measure the extra operand [stack](../../../../../stack-data-structure.md) space required from the current base, with each evaluation leaving one result. Evaluating $e$ first uses $d_e$ slots. Its result occupies one slot while evaluating $f$, so that stage uses $1+d_f$ slots. The final `add` reduces two slots to one. Thus

$$
\boxed{d_{e\text{ first}}=\max(d_e,1+d_f),\qquad d_{f\text{ first}}=\max(d_f,1+d_e).}
$$

By [commutativity](../../../../../commutativity.md) of [addition](../../../../../addition.md), choose the smaller of these two bounds. Evaluate the child of larger depth first. The optimum recurrence on a [binary expression tree](../../../../../binary-expression-tree.md) is

$$
\boxed{\operatorname{depth}(e+f)=\begin{cases}\max(d_e,d_f),&d_e\ne d_f,\\d_e+1,&d_e=d_f.\end{cases}}
$$

Assign depth one to a literal or a simple already-addressable value, and compute the child depths recursively. If $d_e>d_f$, the depths are [integers](../../../../../integer-split.md), so $d_e\geq1+d_f$; evaluating $e$ first therefore attains $d_e$, while reversing the order needs $d_e+1$. If the depths are equal, whichever child goes second needs the extra retained-result slot. These lower bounds prove the recurrence is optimal for evaluating each child subtree without interleaving or spilling. Apply it at every node to minimize peak operand [stack](../../../../../stack-data-structure.md) occupancy for the given [binary expression tree](../../../../../binary-expression-tree.md); this is [optimal stack evaluation of a binary expression tree](../../../../../optimal-stack-evaluation-of-a-binary-expression-tree.md).

This changes child evaluation order, not the parenthesization. For example, a chain-shaped [binary expression tree](../../../../../binary-expression-tree.md) can have depth two, whereas a balanced tree of eight leaves has depth four under this model. The reordering assumes expressions have no order-sensitive [side effects](../../../../../side-effect-computer-science.md) or observable exceptions. Reassociating [floating-point addition](../../../../../floating-point-addition.md) would require additional care because it can change [floating-point rounding](../../../../../floating-point-rounding.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
