<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We derive the [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md) from the [Leibniz rule for divided differences](../../../../../../leibniz-rule-for-divided-differences.md). Fix $t$, let $u_j=t_{i+j}$, and set

$$
q(s)=(s-t)_+^{k-2},\qquad h(s)=(s-t)q(s).
$$

Away from the [spline knots](../../../../../../spline-knot.md), $h(s)=(s-t)_+^{k-1}$. Introduce

$$
D=[u_0,\ldots,u_k]q,\quad
L=[u_0,\ldots,u_{k-1}]q,\quad
R=[u_1,\ldots,u_k]q.
$$

The defining divided-difference recurrence says $(u_k-u_0)D=R-L$. Since $s-t=(s-u_0)+(u_0-t)$ and the first factor is linear, the [Leibniz rule for divided differences](../../../../../../leibniz-rule-for-divided-differences.md) gives

$$
[u_0,\ldots,u_k]h=R+(u_0-t)D.
$$

Multiplication by $u_k-u_0$ consequently yields

$$
(u_k-u_0)[u_0,\ldots,u_k]h
=(t-u_0)L+(u_k-t)R.
$$

Replace $L$ and $R$ by the corresponding lower-order [B-splines](../../../../../../b-spline.md) divided by their support widths. This proves

$$
\boxed{
N_{i,k}(t)=\frac{t-t_i}{t_{i+k-1}-t_i}N_{i,k-1}(t)
+\frac{t_{i+k}-t}{t_{i+k}-t_{i+1}}N_{i+1,k-1}(t)}.
$$

The denominators are positive for the distinct [spline knots](../../../../../../spline-knot.md) of this question. The recursion starts with $N_{i,1}$, the interval indicator on $[t_i,t_{i+1})$. For $k\ge2$, values at the [spline knots](../../../../../../spline-knot.md) follow by the continuous extension of the left side; the usual half-open convention for the order-one factors gives the same result. This proves the recurrence rather than assuming it as a definition.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
