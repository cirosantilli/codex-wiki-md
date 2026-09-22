<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The tableau is the three-stage [Lobatto IIIA method](../../../../../../lobatto-iiia-method.md). To check its [order of a Runge-Kutta method](../../../../../../order-of-a-runge-kutta-method.md) directly, write $e=(1,1,1)^T$, $c=Ae=(0,1/2,1)^T$, and $C=\operatorname{diag}(c)$. The eight [fourth-order conditions for a Runge-Kutta method](../../../../../../fourth-order-conditions-for-a-runge-kutta-method.md) evaluate to

$$
\begin{gathered}
b^Te=1,\qquad b^Tc=\frac12,\qquad b^Tc^2=\frac13,\qquad b^TAc=\frac16,\\
b^Tc^3=\frac14,\qquad b^TCAc=\frac18,\qquad
b^TAc^2=\frac1{12},\qquad b^TA^2c=\frac1{24}.
\end{gathered}
$$

Powers of $c$ here mean componentwise powers. For example, $Ac=(0,1/8,1/2)^T$, $Ac^2=(0,1/24,1/3)^T$, and $A^2c=(0,1/48,1/6)^T$, which make the last three checks immediate. These [Butcher order conditions](../../../../../../butcher-order-condition.md) establish order at least four for general nonlinear [ordinary differential equations](../../../../../../ordinary-differential-equation.md).

It is not order five: part (b)'s [stability function](../../../../../../stability-function.md) has expansion

$$
R(z)=1+z+\frac{z^2}2+\frac{z^3}6+\frac{z^4}{24}+\frac{z^5}{144}+O(z^6)
=e^z-\frac{z^5}{720}+O(z^6).
$$

The fifth coefficient already fails on the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md). **The order is exactly four.**

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Section A](../../section-a.md)
4. [Paper 68](../../../paper-68-split.md)
5. [Iii](../../../split.md)
6. [2015](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
