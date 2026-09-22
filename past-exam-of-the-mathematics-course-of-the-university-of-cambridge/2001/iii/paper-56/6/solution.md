<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Orient the boundary cyclically as $B_0,B_1,\ldots,B_{m-1},B_m=B_0$, and orient every fan triangle consistently as $(P,B_i,B_{i+1})$. Its [vector area](../../../../../vector-area.md) is

$$
\mathbf A_i=\frac12(B_i-P)\times(B_{i+1}-P).
$$

Choose the sign convention in which a triangle with positive normal component along the unit vector $V$ has positive projected area. Then the total signed, or algebraic, projected [area](../../../../../surface-area.md) is

$$
\boxed{A(V)=\frac12\sum_{i=0}^{m-1}V\cdot[(B_i-P)\times(B_{i+1}-P)].}
$$

This is a signed sum, so overlaps and oppositely oriented pieces cancel. Expand the cross product:

$$
(B_i-P)\times(B_{i+1}-P)=B_i\times B_{i+1}+P\times(B_i-B_{i+1}).
$$

The sum of $B_i-B_{i+1}$ is zero around the closed polygon. Consequently

$$
\boxed{A(V)=V\cdot\mathbf A,\qquad \mathbf A=\frac12\sum_{i=0}^{m-1}B_i\times B_{i+1}.}
$$

This [vector area of a polygonal boundary](../../../../../vector-area-of-a-polygonal-boundary.md) depends only on the oriented boundary, not on $P$, and does not require that the polygon be planar. Translating the boundary adds telescoping terms too, so the formula is independent of the choice of spatial origin. It is the polygonal instance of the [vector area](../../../../../vector-area.md) boundary integral $\tfrac12\oint B\times dB$.

For $\mathbf A\ne0$, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $A(V)\le|\mathbf A|$ because $|V|=1$. Hence

$$
\boxed{A_{\max}=|\mathbf A|,\qquad V_{\max}=\frac{\mathbf A}{|\mathbf A|}.}
$$

The opposite direction gives the minimum $-|\mathbf A|$; either direction maximizes the absolute algebraic area. Zero algebraic area occurs exactly for unit directions satisfying $V\cdot\mathbf A=0$, a great circle of directions perpendicular to the area vector. If $\mathbf A=0$, every direction gives zero and every direction is a maximizer, even though the sum of unsigned triangle areas may be positive. Reversing the initial orientation reverses every signed result consistently.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
