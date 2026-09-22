<h1 id="g/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

With fixed endpoint values, the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) is $F_y-\frac d{dx}F_{y'}=0$. If $F$ has no explicit $x$ dependence, differentiation gives

$$
\frac d{dx}(F-y'F_{y'})
=F_x+y'(F_y-\tfrac d{dx}F_{y'})=0.
$$

Thus the [Beltrami identity](../../../../beltrami-identity.md) is $F-y'F_{y'}=\text{constant}$.

For this integrand, $F_y=2y$ and $F_{y'}=1+2y'$, so $y''=y$. The extremals are

$$
\boxed{y(x)=Ae^x+Be^{-x},}
$$

where the two fixed endpoint values determine $A,B$. The Beltrami constant is $y^2-y'^2$, consistent with this solution.

For a nonzero smooth perturbation $\eta$ vanishing at the endpoints, expand the quadratic functional. The first variation vanishes at an extremal, while

$$
J[y+\epsilon\eta]-J[y]
=\epsilon^2\int_{x_1}^{x_2}(\eta^2+\eta'^2)\,dx>0.
$$

The linear term $\int y'$ depends only on the fixed endpoints. Consequently the extremal is a strict minimum and **cannot be a maximum**.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [G](../../g.md)
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
