<h1 id="g/g2/solution">Solution</h1>

↑ **Parent:** [G2](../g2.md)

At a regular constrained extremum, choose an admissible [variation](../../../../variation.md) $k$ with $\delta J[k]\ne0$. The [implicit function theorem](../../../../implicit-function-theorem.md) applied to $J[y+\varepsilon h+s k]$ permits a compensating $s(\varepsilon)$ keeping $J$ fixed. Differentiation at zero gives $\delta I[h]=\lambda\delta J[h]$ for every $h$, where $\lambda=\delta I[k]/\delta J[k]$. Integrating the [first variation](../../../../first-variation.md) of $I-\lambda J$ by parts and using arbitrary compactly supported $h$ gives

$$
\boxed{\frac d{dx}(F_{y'}-\lambda G_{y'})-(F_y-\lambda G_y)=0.}
$$

Smoothness alone does not exclude an abnormal constraint: if $\delta J$ vanishes identically, one needs the general multiplier form with two multipliers rather than automatically setting the coefficient of $I$ to one. The displayed normal form uses the usual regular-constraint hypothesis.

For the given quadratic functionals, the equation is $\boxed{(py')'+qy+\lambda ry=0}$. If the endpoint values of $y$ are free, the boundary [variation](../../../../variation.md) $[py'h]_a^b$ gives the natural conditions $\boxed{p(a)y'(a)=p(b)y'(b)=0}$, interpreted by limits at singular endpoints. Multiply the equation by $y$ and integrate. These boundary terms vanish, leaving

$$
\int_a^b(p(y')^2-qy^2)dx=\lambda\int_a^b ry^2dx,\qquad\boxed{I=\lambda J}.
$$

For two eigenfunctions, multiply their equations by the other function and subtract. Integration gives

$$
[p(y_ny_m'-y_my_n')]_a^b+(\lambda_m-\lambda_n)\int_a^b ry_my_n\,dx=0.
$$

The natural conditions remove the bracket, so distinct eigenvalues imply $\boxed{\int_a^b ry_my_n\,dx=0}$.

In the Legendre case, comparison of leading [polynomial](../../../../polynomial-split.md) coefficients gives $\lambda_n=n(n+1)$, so the degrees correspond to distinct eigenvalues. A [degree](../../../../degree-graph-theory.md)-zero [polynomial](../../../../polynomial-split.md) is $y_0=C_0$. Write $y_1=Ax+B$; [orthogonality](../../../../orthogonal-vectors.md) to $1$ on $[-1,1]$ gives $B=0$. Write $y_2=Ax^2+Bx+C$. [Orthogonality](../../../../orthogonal-vectors.md) to $x$ gives $B=0$, and [orthogonality](../../../../orthogonal-vectors.md) to $1$ gives $2A/3+2C=0$. Thus

$$
\boxed{y_0=C_0,\quad y_1=C_1x,\quad y_2=C_2(3x^2-1)/2.}
$$

These [polynomials](../../../../polynomial-split.md) satisfy the natural endpoint limits because $1-x^2$ vanishes at both endpoints.

## ↑ Ancestors (12)

1. [G2](../g2.md)
2. [G](../../g.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
