<h1 id="s9/3/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

At each time-2 node, replicate one positive put payoff using $\Delta$ shares and a current cash deposit $b$. Its two terminal values must satisfy $\Delta S_u+Rb=P_u$ and $\Delta S_d+Rb=P_d$, with $R=1.04$. Thus

$$
\Delta=\frac{P_u-P_d}{S_u-S_d},\qquad b=\frac{P_u-\Delta S_u}{1.04}.
$$

For the three nodes the hedge is

$$
\boxed{\begin{array}{c|c|c|c}
S_2&\Delta&b&P_2=\Delta S_2+b\\\hline
121&0&0&0\\
99&-21/22&103.95/1.04=99.95192&5.45192\\
81&-1&108/1.04=103.84615&22.84615
\end{array}}
$$

At $S_2=121$, both child puts expire worthless. At $99$, the child payoffs are $0$ and $18.9$; at $81$, they are $18.9$ and $35.1$. Substituting the hedge holdings into both child states verifies those payoffs exactly.

The writer is short the option and therefore **holds this positive replicating portfolio** to offset the liability. At the lower nodes that means shorting shares and depositing the proceeds together with the option value, rather than buying positive-delta stock. Rebalancing the replicating holdings along the tree is self-financing in the ideal model; the combined short option plus hedge has zero terminal liability in either child state.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [3](../../3.md)
3. [S9](../../../s9.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
