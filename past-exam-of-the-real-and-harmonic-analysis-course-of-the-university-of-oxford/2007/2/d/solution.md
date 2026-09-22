<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $E\subseteq\mathbb R^n$, define the [Lebesgue outer measure](../../../../lebesgue-outer-measure.md) by

$$
\mathscr L^*(E)=\inf\left\{\sum_{j=1}^{\infty}\operatorname{vol}(Q_j):E\subseteq\bigcup_jQ_j,\quad Q_j=\prod_{r=1}^n[a_{jr},b_{jr})\right\},
$$

where the boxes are bounded and $\operatorname{vol}(Q_j)=\prod_r(b_{jr}-a_{jr})$. The empty covering handles the empty set. [Monotonicity](../../../../monotonic-function.md) follows by inclusion of admissible covers. Taking covers within $\varepsilon2^{-j}$ of the outer [measures](../../../../measure-split.md) of a sequence of sets proves [countable subadditivity](../../../../countable-subadditivity-of-a-measure.md); when the sum is infinite the inequality is automatic. [Lebesgue measure](../../../../lebesgue-measure.md) is the restriction of $\mathscr L^*$ to its Caratheodory-[measurable sets](../../../../measurable-set.md).

If $d(A,B)=\delta>0$, subdivide each box of any countable cover of $A\cup B$ into finitely many half-open boxes of diameter smaller than $\delta$, preserving its total volume. No small box can meet both $A$ and $B$. The boxes meeting $A$ cover $A$, and the disjoint family meeting $B$ covers $B$, so the original cover costs at least $\mathscr L^*(A)+\mathscr L^*(B)$. Taking the [infimum](../../../../infimum.md) and then using subadditivity gives

$$
\boxed{\mathscr L^*(A\cup B)=\mathscr L^*(A)+\mathscr L^*(B).}
$$

Thus the [outer measure](../../../../outer-measure.md) underlying [Lebesgue measure](../../../../lebesgue-measure.md) is a [metric outer measure](../../../../metric-outer-measure.md), and in particular every [Borel set](../../../../borel-set.md) is Lebesgue measurable.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../split.md)
5. [Real and harmonic analysis course of the University of Oxford](../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
