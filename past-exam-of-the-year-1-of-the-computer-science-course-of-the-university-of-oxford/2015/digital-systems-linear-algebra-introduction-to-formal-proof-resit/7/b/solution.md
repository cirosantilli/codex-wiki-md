<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $H=(P\land Q)\lor(P\land R)$ and $K=P\land(Q\lor R)$. In the following [natural deduction](../../../../../natural-deduction.md) derivations, brackets name [temporary assumptions](../../../../../temporary-assumption.md), and cited ranges specify the [subproofs](../../../../../subproof.md) discharged. The abbreviations $\land E,\land I,\lor E,\lor I$ denote the corresponding [conjunction elimination rule](../../../../../conjunction-elimination-rule.md), [conjunction introduction rule](../../../../../conjunction-introduction-rule.md), [disjunction elimination rule](../../../../../disjunction-elimination-rule.md) and [disjunction introduction rule](../../../../../disjunction-introduction-rule.md).

First use the [disjunction elimination rule](../../../../../disjunction-elimination-rule.md) backwards: split the premise into two cases and build the whole conclusion in each case.

$$
\begin{array}{rll}
1&H&\text{premise}\\
2&[P\land Q]^a&\text{assumption}\\
3&\quad P&\land E\ 2\\
4&\quad Q&\land E\ 2\\
5&\quad Q\lor R&\lor I\ 4\\
6&\quad K&\land I\ 3,5\\
7&[P\land R]^b&\text{assumption}\\
8&\quad P&\land E\ 7\\
9&\quad R&\land E\ 7\\
10&\quad Q\lor R&\lor I\ 9\\
11&\quad K&\land I\ 8,10\\
12&K&\lor E\ 1,(2\text{--}6),(7\text{--}11).
\end{array}
$$

Alternatively, use the [conjunction introduction rule](../../../../../conjunction-introduction-rule.md) backwards on the conclusion. First obtain $P$ by cases, then obtain $Q\lor R$ by a second case analysis, and finally combine the results:

$$
\begin{array}{rll}
1&H&\text{premise}\\
2&[P\land Q]^a&\text{assumption}\\
3&\quad P&\land E\ 2\\
4&[P\land R]^b&\text{assumption}\\
5&\quad P&\land E\ 4\\
6&P&\lor E\ 1,(2\text{--}3),(4\text{--}5)\\
7&[P\land Q]^c&\text{assumption}\\
8&\quad Q&\land E\ 7\\
9&\quad Q\lor R&\lor I\ 8\\
10&[P\land R]^d&\text{assumption}\\
11&\quad R&\land E\ 10\\
12&\quad Q\lor R&\lor I\ 11\\
13&Q\lor R&\lor E\ 1,(7\text{--}9),(10\text{--}12)\\
14&K&\land I\ 6,13.
\end{array}
$$

The first [proof goal transformation](../../../../../proof-goal-transformation.md) starts with case analysis; the second starts by splitting a conjunction goal. Counting only actual applications of the printed [inference rules](../../../../../inference-rule.md), both use nine steps: the first has four $\land E$, two $\lor I$, two $\land I$ and one $\lor E$; the second has four $\land E$, two $\lor I$, one $\land I$ and two $\lor E$. The extra case analysis in the second exactly replaces one conjunction construction. If assumption lines are counted as well, the second display has two more lines because it opens four case [subproofs](../../../../../subproof.md) rather than two. Thus the apparent difference in display length need not be a difference in inference count.

$$
\boxed{H\vdash P\land(Q\lor R)\quad\text{by either proof; nine primitive inferences each}.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
