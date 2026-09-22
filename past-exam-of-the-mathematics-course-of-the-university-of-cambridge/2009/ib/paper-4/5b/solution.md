<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

At a regular constrained stationary point, $\nabla g\ne0$ and the directional derivative of $f$ vanishes along the tangent to $g=0$. Therefore $\nabla f=\lambda\nabla g$ for a [Lagrange multiplier](../../../../../lagrange-multiplier.md) $\lambda$. Solve this equation together with the constraint, then compare candidate values and any exceptional nonregular points. Proportionality of the two gradients gives

$$
\boxed{f_x(a,b)g_y(a,b)-f_y(a,b)g_x(a,b)=0.}
$$

If $\nabla g=0$ at an exceptional point, this determinant vanishes trivially, although the regular multiplier method need not identify every such point.

For the given ellipse, maximize $r^2=x^2+y^2$. The constraint is $r^2+xy=4$, and $xy\geq-r^2/2$, so $4\geq r^2/2$. Equality requires $x=-y$ and the constraint then gives $(x,y)=(2,-2)$ or $(-2,2)$. Thus

$$
\boxed{r_{\max}=2\sqrt2.}
$$

The constraint gradient vanishes only at the origin, which is not on this ellipse, so the regularity condition holds everywhere relevant.

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
