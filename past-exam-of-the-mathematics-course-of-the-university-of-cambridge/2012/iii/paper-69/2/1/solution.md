<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The coefficients are those of the three-stage [Lobatto IIIA method](../../../../../../lobatto-iiia-method.md). Set $e=(1,1,1)^T$, $c=Ae=(0,1/2,1)^T$ and $C=\operatorname{diag}(c)$. Direct calculation gives all eight [fourth-order conditions for a Runge-Kutta method](../../../../../../fourth-order-conditions-for-a-runge-kutta-method.md):

$$
\begin{gathered}
b^Te=1,\quad b^Tc=\tfrac12,\quad b^Tc^2=\tfrac13,\quad b^TAc=\tfrac16,\\
b^Tc^3=\tfrac14,\quad b^TCAc=\tfrac18,\quad
b^TAc^2=\tfrac1{12},\quad b^TA^2c=\tfrac1{24}.
\end{gathered}
$$

Powers of $c$ are componentwise. These [Butcher order conditions](../../../../../../butcher-order-condition.md) prove order at least four for a smooth general nonlinear vector field; matching a scalar test equation alone would not suffice. A necessary fifth-order condition fails:

$$
b^Tc^4=\frac5{24}\ne\frac15.
$$

Hence the method has **order exactly four**, with one-step [local truncation error](../../../../../../local-truncation-error.md) $O(h^5)$ and, under stability and smoothness hypotheses, [global error](../../../../../../global-discretization-error.md) $O(h^4)$.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [2](../../2.md)
3. [Section I](../../section-i.md)
4. [Paper 69](../../../paper-69-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
