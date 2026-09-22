<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose the knot origin so the span most influenced by $P_i$ is $[i,i+1]$, and use its local parameter $t\in[0,1]$. The three active uniform quadratic [B-spline](../../../../../../b-spline.md) basis functions give

$$
C_i(t)=\tfrac12(1-t)^2P_{i-1}+(\tfrac12+t-t^2)P_i+\tfrac12t^2P_{i+1}.
$$

The central coefficient reaches its maximum at $t=1/2$, so this is indeed the span centered on the strongest influence of $P_i$. Express it in the quadratic [Bernstein basis](../../../../../../bernstein-basis.md):

$$
C_i(t)=(1-t)^2B_0+2t(1-t)B_1+t^2B_2.
$$

Matching constant, linear and quadratic coefficients gives the quadratic [Bézier curve](../../../../../../bezier-curve.md) controls

$$
\boxed{B_0=\frac{P_{i-1}+P_i}{2},\qquad B_1=P_i,\qquad B_2=\frac{P_i+P_{i+1}}2}.
$$

For example, $C_i'(0)=2(B_1-B_0)=P_i-P_{i-1}$ and $C_i'(1)=2(B_2-B_1)=P_{i+1}-P_i$, checking the endpoint derivatives and the $C^1$ joins of neighboring spans.

## ↑ Ancestors (11)

1. [A](../a.md)
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
