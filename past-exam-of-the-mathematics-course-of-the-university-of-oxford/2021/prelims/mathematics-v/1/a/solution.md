<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [change of variables](../../../../../../change-of-variables-formula.md) $u=x^2-y^2$, $v=xy$. Its [Jacobian determinant](../../../../../../jacobian-determinant.md) in the first quadrant is $2(x^2+y^2)>0$, and the inverse is uniquely determined by

$$
x^2=\frac{\sqrt{u^2+4v^2}+u}{2},\qquad
y^2=\frac{\sqrt{u^2+4v^2}-u}{2}.
$$

Both are positive for $v>0$, so the transformation is one-to-one on the region. It becomes the [rectangle](../../../../../../rectangle.md) $-2\leq u\leq4$, $1\leq v\leq3$. The [integrand](../../../../../../integrand.md) is $uv$, and $x^2+y^2=\sqrt{u^2+4v^2}$. Thus

$$
\begin{aligned}
\iint_A(x^3y-xy^3)\,dx\,dy
&=\int_1^3\int_{-2}^4\frac{uv}{2\sqrt{u^2+4v^2}}\,du\,dv\\
&=\int_1^3v\left(\sqrt{v^2+4}-\sqrt{v^2+1}\right)\,dv\\
&=\boxed{\frac{13\sqrt{13}-10\sqrt{10}-5\sqrt5+2\sqrt2}{3}.}
\end{aligned}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
