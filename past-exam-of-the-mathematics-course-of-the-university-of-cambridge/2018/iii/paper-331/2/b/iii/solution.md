<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $q=\alpha h$, $d=\alpha(1-h)$, and use the four regional amplitudes above. Continuity of $\widehat w$ at the two jumps gives

$$
A\sinh d=B\cosh q+C\sinh q,\qquad
D\sinh d=B\cosh q-C\sinh q.
$$

Pressure continuity, using [vorticity-jump matching for an inviscid shear flow](../../../../../../../vorticity-jump-matching-for-an-inviscid-shear-flow.md), gives the other two equations:

$$
\begin{aligned}
-\alpha(1-c)(A\cosh d+B\sinh q+C\cosh q)
+\frac{B\cosh q+C\sinh q}{h}&=0,\\
-\alpha(1+c)(-B\sinh q+C\cosh q-D\cosh d)
-\frac{B\cosh q-C\sinh q}{h}&=0.
\end{aligned}
$$

These are the required homogeneous four equations. As a useful reduction, put $X=\tanh q$, $Y=\tanh d$, $H=q(1+XY)$ and $J=q(X+Y)$. Eliminating $A,D$ leaves

$$
\boxed{[(1-c)H-Y]B+[(1-c)J-XY]C=0,\qquad
[(1+c)H-Y]B-[(1+c)J-XY]C=0.}
$$

The vanishing [determinant](../../../../../../../determinant.md) gives $c^2=(H-Y)(J-XY)/(HJ)$, which expands to the printed [dispersion relation](../../../../../../../dispersion-relation.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
