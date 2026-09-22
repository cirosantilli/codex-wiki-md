<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Order the [period lattice](../../../../../period-lattice.md) basis so the indicated contour is positively oriented; reversing its orientation only changes the signs of the resulting integers. Set

$$
A=\int_a^{a+\lambda_1}h(w)\,dw,\qquad B=\int_a^{a+\lambda_2}h(w)\,dw,\qquad h=f'/f.
$$

Pairing the translated sides while retaining the factor $w$ gives

$$
\oint_{\Gamma_a}w h(w)\,dw=\lambda_1 B-\lambda_2 A.
$$

For example, the right side is the translate by $\lambda_1$ of the left side with reversed orientation; their combined contribution is $\lambda_1B$. The bottom and top similarly give $-\lambda_2A$.

Along either path there is a continuously continued logarithm of the nonzero finite function $f$. Since its endpoint values agree by periodicity, each logarithmic increment is an integer multiple of $2\pi i$. Therefore $A=2\pi i r$, $B=2\pi i s$ for integers $r,s$. The [residue theorem](../../../../../residue-theorem.md) applied to $wh$ now yields

$$
\boxed{\sum_i n_ip_i=s\lambda_1-r\lambda_2\in\Lambda.}
$$

This is the [elliptic divisor-sum identity](../../../../../elliptic-divisor-sum-identity.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the geometry course of the University of Oxford](../../../../split.md)
6. [Geometry course of the University of Oxford](../../../../../geometry-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
