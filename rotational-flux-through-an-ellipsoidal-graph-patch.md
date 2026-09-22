# Rotational flux through an ellipsoidal graph patch

↑ **Parent:** [Surface integral](surface-integral.md)

Take the upward-oriented graph $z=c\sqrt{1-x^2/a^2-y^2/b^2}$ over $0\leq x\leq L_x$, $0\leq y\leq L_y$, where $a,b,c,L_x,L_y>0$, $A=L_x^2/a^2$, $B=L_y^2/b^2$ and $A+B<1$. The [surface flux](flux-integral.md) of the [vector field](vector-field.md) $F=(-y,x,0)$ is the displayed formula. Indeed the [vector surface element](vector-area-element.md) is $(-z_x,-z_y,1)dxdy$, so

$$
\Phi=c\left(\frac1{b^2}-\frac1{a^2}\right)\int_0^{L_x}\int_0^{L_y}\frac{xy}{\sqrt{1-x^2/a^2-y^2/b^2}}\,dy\,dx.
$$

The [change of variables](change-of-variables-formula.md) $u=x^2/a^2$, $v=y^2/b^2$ changes $xy\,dxdy$ to $a^2b^2\,dudv/4$. Integrating $(1-u-v)^{-1/2}$ over $[0,A]\times[0,B]$ gives $\tfrac43[1-(1-A)^{3/2}-(1-B)^{3/2}+(1-A-B)^{3/2}]$, proving the result. When $a=b$, the value of the [vector field](vector-field.md) is a [tangent vector](tangent-vector-split.md) to the [ellipsoid](ellipsoid.md) at every point, and the [surface flux](flux-integral.md) vanishes pointwise.

## ↑ Ancestors (9)

1. [Surface integral](surface-integral.md)
2. [Vector calculus](vector-calculus.md)
3. [Multivariable calculus](multivariable-calculus-split.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2/7/solution.md)
