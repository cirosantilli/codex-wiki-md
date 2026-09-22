<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the standard partition normalization of [B-splines](../../../../../../b-spline.md), with order $k$ meaning degree $k-1$. The [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md) on arbitrary increasing [spline knots](../../../../../../spline-knot.md) is

$$
N_{i,k}(x)=\frac{x-t_i}{t_{i+k-1}-t_i}N_{i,k-1}(x)+\frac{t_{i+k}-x}{t_{i+k}-t_{i+1}}N_{i+1,k-1}(x),
$$

starting with $N_{i,1}(x)=\mathbf1_{[t_i,t_{i+1})}(x)$. Terms with zero denominator are interpreted as zero in the usual repeated-knot convention. For the uniform knots here, $t_i=i$, this reduces to

$$
\boxed{N_{i,k}(x)=\frac{x-i}{k-1}N_{i,k-1}(x)+\frac{i+k-x}{k-1}N_{i+1,k-1}(x),\qquad k\ge2.}
$$

The index of the second lower-order [B-spline](../../../../../../b-spline.md) is $i+1$, not $i-1$. Both lower-order supports combine to give $[i,i+k]$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
