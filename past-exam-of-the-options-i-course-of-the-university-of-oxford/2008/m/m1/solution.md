<h1 id="m/m1/solution">Solution</h1>

↑ **Parent:** [M1](../m1.md)

The inverse transformation is $x=2u+v$, $y=v$, with absolute [Jacobian determinant](../../../../jacobian-determinant.md) two. The original positivity constraints become $v>0$ and $2u+v>0$. Thus

$$
\boxed{A=\{(u,v):v>\max(0,-2u)\}},\qquad
f_{U,V}(u,v)=\tfrac12e^{-u-v}\mathbf1_A.
$$

Integrating out $v$ gives

$$
f_U(u)=\frac12e^{-u}\int_{\max(0,-2u)}^\infty e^{-v}\,dv
=\frac12e^{-u-\max(0,-2u)}
=\boxed{\frac12e^{-|u|}}.
$$

This is the centred [Laplace distribution](../../../../laplace-distribution.md) with scale one.

## ↑ Ancestors (12)

1. [M1](../m1.md)
2. [M](../../m.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
