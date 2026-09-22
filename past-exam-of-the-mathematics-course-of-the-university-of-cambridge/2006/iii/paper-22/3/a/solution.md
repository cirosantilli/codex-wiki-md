<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [flat connection](../../../../../../flat-connection.md) as $d+A_x\,dx+A_y\,dy$ in a global unitary frame. Solve the matrix ordinary differential equation

$$
\partial_x u(x,y)=-A_x(x,y)u(x,y),\qquad u(0,y)=I.
$$

Smooth dependence on parameters gives a smooth solution on the entire open square. Since $A_x$ is skew-Hermitian and trace free, differentiating $u^*u$ and $\det u$ shows that $u(x,y)\in SU(2)$. Under the [bundle gauge transformation](../../../../../../unitary-bundle-gauge-transformation.md) $u$, the transformed connection has

$$
A'_x=u^{-1}A_xu+u^{-1}\partial_xu=0.
$$

Its [vector-bundle curvature](../../../../../../curvature-form.md) is still zero. The remaining [vector-bundle curvature](../../../../../../curvature-form.md) equation is $\partial_xA'_y=0$, so $A'_y=B(y)$ is independent of $x$. Now solve $v'(y)=-B(y)v(y)$ with $v(0)=I$. Again $v\in SU(2)$; this second [bundle gauge transformation](../../../../../../unitary-bundle-gauge-transformation.md), independent of $x$, leaves $A'_x=0$ and makes $A''_y=0$. Thus **the original connection is gauge equivalent to the trivial connection**. Both transformations exist on the whole square, not just in a small coordinate neighborhood.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
