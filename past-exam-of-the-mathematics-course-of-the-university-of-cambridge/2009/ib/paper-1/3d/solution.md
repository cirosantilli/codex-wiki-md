<h1 id="3d/solution">Solution</h1>

↑ **Parent:** [3D](../3d.md)

For a [holomorphic function](../../../../../holomorphic-function.md), compute its complex [derivative](../../../../../derivative.md) along the real and imaginary directions. The real direction gives $f'=u_x+iv_x$, while division by an imaginary increment gives $f'=v_y-iu_y$. Equating real and imaginary parts proves the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md):

$$
\boxed{u_x=v_y,\qquad u_y=-v_x.}
$$

For the specified real part, $u_x=-e^{-x}\cos y$ and $u_y=-e^{-x}\sin y$. Integrating $v_y=u_x$ gives $v=-e^{-x}\sin y+C(x)$; the other relation in the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) then forces $C'(x)=0$. Thus the [harmonic conjugate](../../../../../harmonic-conjugate.md) and the [holomorphic function](../../../../../holomorphic-function.md) are

$$
\boxed{v(x,y)=-e^{-x}\sin y+C,\qquad f(z)=e^{-z}+iC,\quad C\in\mathbb R.}
$$

## ↑ Ancestors (10)

1. [3D](../3d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
