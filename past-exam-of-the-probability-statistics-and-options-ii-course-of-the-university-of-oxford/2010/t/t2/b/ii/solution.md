<h1 id="t/t2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The expression $G^{-1}$ presupposes that $G$ is invertible; positivity of the stated optimal coordinates alone would not prove that, so use the nonsingularity implicit in this expression. Let $c_B$ be the first $m$ components of $c$ and set $y=G^{-T}c_B$. Then $G^Ty=c_B$.

For any nonbasic column $a_j$, introduce $x_j=\varepsilon>0$ while changing the basic vector from $u$ to $u-\varepsilon G^{-1}a_j$. This stays feasible for sufficiently small $\varepsilon$ because every $u_i>0$. Optimality at $u$ implies the objective slope $c_j-c_B^TG^{-1}a_j\le0$. Therefore $a_j^Ty\ge c_j$ for every such column, and the basic columns satisfy equality. Thus $y$ is dual feasible, independently of the right-hand side.

For $v=G^{-1}b^*\ge0$, the proposed $x^*$ is primal feasible and

$$
c^Tx^*=c_B^Tv=y^TGv=y^Tb^*.
$$

[Weak duality](../../../../../../weak-duality.md), valid with unrestricted equality multipliers, proves $\boxed{x^*\text{ is optimal}}$. This also explains the stability of an optimal [basis](../../../../../../basis.md) while its new basic coordinates remain nonnegative.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [T2](../../../t2.md)
4. [T](../../../../t.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
