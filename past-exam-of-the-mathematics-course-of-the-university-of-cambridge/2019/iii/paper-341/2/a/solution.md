<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The tableau is the three-stage [Lobatto IIIA method](../../../../../../lobatto-iiia-method.md). For its stage [matrix](../../../../../../matrix.md) $A$, weights $b$, nodes $c$ and $C=\operatorname{diag}(c)$, the [Butcher order conditions](../../../../../../butcher-order-condition.md) through order four are

$$
\begin{gathered}
b^T\mathbf1=1,\quad b^Tc=\frac12,\quad b^Tc^{\circ2}=\frac13,\quad b^TAc=\frac16,\\
b^Tc^{\circ3}=\frac14,\quad b^TCAc=\frac18,\quad b^TAc^{\circ2}=\frac1{12},\quad b^TA^2c=\frac1{24},
\end{gathered}
$$

where $c^{\circ j}$ means coordinatewise powers. Direct substitution verifies all eight identities. Equivalently, this is a [collocation Runge-Kutta method](../../../../../../collocation-runge-kutta-method.md) at the three [Lobatto quadrature](../../../../../../lobatto-quadrature.md) nodes, whose weights integrate cubic [polynomials](../../../../../../polynomial-split.md) exactly.

Order five would require $b^Tc^{\circ4}=1/5$, but here $b^Tc^{\circ4}=5/24$. Therefore the method has **exactly order four**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
