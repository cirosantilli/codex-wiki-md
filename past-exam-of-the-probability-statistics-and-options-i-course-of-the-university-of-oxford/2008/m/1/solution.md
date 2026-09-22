<h1 id="m/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The inverse change of variables is $x=2u+v$, $y=v$, with absolute [Jacobian determinant](../../../../jacobian-determinant.md) two. Positivity of $x,y$ gives

$$
A=\{(u,v):v>0,\ 2u+v>0\}.
$$

The [change of variables for probability densities](../../../../change-of-variables-for-probability-densities.md) gives

$$
f_{U,V}(u,v)=\tfrac14e^{-(2u+2v)/2}\cdot2
=\tfrac12e^{-u-v}\quad((u,v)\in A).
$$

For fixed $u$, integrate over $v>\max(0,-2u)$:

$$
f_U(u)=\tfrac12e^{-u}\int_{\max(0,-2u)}^\infty e^{-v}\,dv
=\begin{cases}\tfrac12e^{-u},&u\geq0,\\
\tfrac12e^u,&u<0.\end{cases}
$$

Thus $\boxed{f_U(u)=\tfrac12e^{-|u|}}$, the standard [Laplace distribution](../../../../laplace-distribution.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [M](../../m.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
