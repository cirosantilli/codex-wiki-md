<h1 id="f/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The required condition is $D_2F(a,b)\neq0$. The [implicit function theorem](../../../../implicit-function-theorem.md) then gives a unique local differentiable branch $y=f(x)$ with $f(a)=b$ and

$$
\boxed{f'(x)=-\frac{D_1F(x,f(x))}{D_2F(x,f(x))}.}
$$

The denominator remains nonzero after shrinking the neighborhood by [continuity](../../../../continuous-function.md).

For the specified smooth function,

$$
F_x=y+\cos(x+y),\qquad F_y=x+\cos(x+y).
$$

At $(0,0)$ both equal one, so the condition holds and $f'(0)=-1$. Differentiate $F(x,f(x))=0$ twice:

$$
F_{xx}+2F_{xy}f'+F_{yy}(f')^2+F_yf''=0.
$$

At zero, $F_{xx}=F_{yy}=0$, $F_{xy}=1$, and $F_y=1$. Consequently

$$
\boxed{f'(0)=-1,\qquad f''(0)=2.}
$$

The additional derivatives exist because this particular $F$ is smooth; the general first-derivative theorem only requires the stated continuous first [partial derivatives](../../../../partial-derivative.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [F](../../f.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
