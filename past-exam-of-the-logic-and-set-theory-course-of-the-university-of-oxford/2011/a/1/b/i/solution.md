<h1 id="a/1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The following is a [logical derivation](../../../../../../logical-derivation.md) using only A1, A2 and the [modus ponens rule](../../../../../../implication-elimination-rule.md). The first two lines are assumptions:

$$
\begin{array}{rll}
1.&\alpha\to\beta&\text{assumption},\\
2.&\beta\to\gamma&\text{assumption},\\
3.&(\beta\to\gamma)\to(\alpha\to(\beta\to\gamma))&\mathrm{A1},\\
4.&\alpha\to(\beta\to\gamma)&\mathrm{MP}\ (2,3),\\
5.&(\alpha\to(\beta\to\gamma))\to((\alpha\to\beta)\to(\alpha\to\gamma))&\mathrm{A2},\\
6.&(\alpha\to\beta)\to(\alpha\to\gamma)&\mathrm{MP}\ (4,5),\\
7.&\alpha\to\gamma&\mathrm{MP}\ (1,6).
\end{array}
$$

Thus $\boxed{\{\alpha\to\beta,\beta\to\gamma\}\vdash\alpha\to\gamma}$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
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
