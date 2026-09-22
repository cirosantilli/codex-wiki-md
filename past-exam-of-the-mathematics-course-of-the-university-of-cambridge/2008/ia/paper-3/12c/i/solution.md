<h1 id="12c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The inequalities $y\le x\le2y$ force $y\ge0$, and the reciprocal bounds exclude zero. Thus the whole region lies in the positive quadrant. Introduce [ratio-product coordinates](../../../../../../ratio-product-coordinates.md)

$$
u=\frac{x}{y},\qquad v=xy.
$$

The region becomes the rectangle $1\le u\le2$, $1\le v\le2$. The inverse map and its [Jacobian determinant](../../../../../../jacobian-determinant.md) are

$$
x=\sqrt{uv},\qquad y=\sqrt{v/u},\qquad
\frac{\partial(x,y)}{\partial(u,v)}=\begin{vmatrix}x/(2u)&x/(2v)\\-y/(2u)&y/(2v)\end{vmatrix}=\frac{xy}{2uv}=\frac1{2u}>0.
$$

The [change of variables formula](../../../../../../change-of-variables-formula.md) then gives

$$
\int_A\frac{x}{y}\,dx\,dy=\int_1^2\int_1^2u\frac1{2u}\,dv\,du=\boxed{\frac12}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12C](../../12c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
