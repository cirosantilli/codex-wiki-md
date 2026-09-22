<h1 id="28j/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\mathcal F_n$ represent the information at decision time $n$ and $E_n$ [conditional expectation](../../../../../../conditional-expectation.md) given it. $V_n(w)$ is the largest conditional expected utility from the remaining [consumption](../../../../../../consumption.md) opportunities with current wealth $w$; it may depend on the information state as well as $w$. The controls $c$ and $\theta$ are chosen using current information. In the usual allocation interpretation $0\leq c\leq w$ and $0\leq\theta\leq1$, and next wealth is $(w-c)[r+\theta(X_{n+1}-r)]$. Other borrowing/short-selling rules require explicitly replacing this admissible set while preserving solvency.

The [Bellman equation](../../../../../../bellman-equation.md) follows by separating current utility from future utility: after any current decision the best continuation has conditional value $V_{n+1}$, and maximizing over the current admissible decisions gives the stated recursion. At the last opportunity all wealth is consumed, because utility is increasing, giving $V_N(w)=U(w)$.

There are two printed qualifications. Strict convexity is not needed for this recursion, but it conflicts with the concave power utility in part (ii) and does not support the interior maximizing first-order conditions in part (iii). Also the displayed recursion starting at $n=0$ includes [consumption](../../../../../../consumption.md) at times $0,\ldots,N$, whereas the preceding sum starts at one. The same recursion represents that sum when begun at time one; alternatively relabel the [consumption](../../../../../../consumption.md) dates. Below the policy is given for the recursion's remaining horizon, so this indexing discrepancy does not leave the optimization unspecified.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [28J](../../28j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
