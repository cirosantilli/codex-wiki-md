<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [degree elevation of Bernstein coefficients](../../../../../../degree-elevation-of-bernstein-coefficients.md). If $b_j$ are degree-$p$ [Bézier curve](../../../../../../bezier-curve.md) controls, the identical curve has degree-$(p+1)$ controls

$$
b_0^+=b_0,\qquad b_{p+1}^+=b_p,\qquad b_j^+=\frac{j}{p+1}b_{j-1}+\left(1-\frac{j}{p+1}\right)b_j\quad(1\leq j\leq p).
$$

This follows by multiplying each degree-$p$ [Bernstein basis](../../../../../../bernstein-basis.md) polynomial by $(1-t)+t$ and collecting the degree-$(p+1)$ terms, so the operation changes the representation, not the curve.

For the quadratic controls in part (a), the cubic controls are

$$
D_0=B_0,\quad D_1=\frac{B_0+2B_1}{3}=\frac{P_{i-1}+5P_i}{6},\quad D_2=\frac{2B_1+B_2}{3}=\frac{5P_i+P_{i+1}}6,\quad D_3=B_2.
$$

Raise these cubic [Bézier curve](../../../../../../bezier-curve.md) controls once more. Then

$$
E_0=B_0,\quad E_1=\tfrac14D_0+\tfrac34D_1=\tfrac12(B_0+B_1),\quad E_2=\tfrac12(D_1+D_2)=\tfrac16(B_0+4B_1+B_2),
$$



$$
E_3=\tfrac34D_2+\tfrac14D_3=\tfrac12(B_1+B_2),\qquad E_4=B_2.
$$

Thus the requested quartic [Bézier curve](../../../../../../bezier-curve.md) controls, expressed in the original polygon, are

$$
\boxed{\begin{aligned}
E_0&=(P_{i-1}+P_i)/2,\\
E_1&=(P_{i-1}+3P_i)/4,\\
E_2&=(P_{i-1}+10P_i+P_{i+1})/12,\\
E_3&=(3P_i+P_{i+1})/4,\\
E_4&=(P_i+P_{i+1})/2.
\end{aligned}}
$$

Each expression is an [affine combination](../../../../../../affine-combination.md) whose coefficients sum to one. Endpoint positions and derivatives are preserved at each degree-raising step, as is every point of the span.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
