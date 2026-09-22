<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The steady-state output is $q=\bar a\bar c+bc+\bar cd$. Its [Karnaugh map](../../../../../karnaugh-map.md), with rows $ab$ and columns $cd$ in [Gray code](../../../../../gray-code.md) order, is

$$
\begin{array}{c|cccc}
ab\backslash cd&00&01&11&10\\\hline
00&1&1&0&0\\01&1&1&1&1\\11&0&1&1&1\\10&0&1&0&0
\end{array}.
$$

The existing [prime implicants](../../../../../prime-implicant.md) cover adjacent ones except for some transitions in $c$. The [consensus theorem](../../../../../consensus-theorem.md) supplies the two missing bridging implicants **$\bar ab$ and $bd$**, giving

$$
\boxed{q_{\mathrm{safe}}=\bar a\bar c+bc+\bar cd+\bar ab+bd.}
$$

Both are needed in a hazard-free [sum of products](../../../../../disjunctive-normal-form.md) retaining the original terms. At $a=0,b=1,d=0$, the two values of $c$ require a common implicant, necessarily covered by $\bar ab$; at $a=1,b=1,d=1$, the corresponding transition requires $bd$. Neither bridge covers the other's critical edge. All other adjacent-one pairs already share a term. Thus two is the least number of additional [prime implicants](../../../../../prime-implicant.md). This addresses single-input static hazards; simultaneous input changes require separate analysis.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
