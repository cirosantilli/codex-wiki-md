<h1 id="p/3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For nodes $0,1$ and $f(x)=e^x$, the cubic [Hermite interpolating polynomial](../../../../../hermite-interpolating-polynomial.md) is

$$
h(x)=1+x+(2e-5)x^2+(3-e)x^3.
$$

Indeed its values at zero and one are $1,e$, and its [derivatives](../../../../../derivative.md) there are also $1,e$. The [Hermite interpolation error formula](../../../../../hermite-interpolation-error-formula.md) gives

$$
|e^x-h(x)|=\frac{e^\xi}{4!}x^2(1-x)^2
\le\frac e{24}\left(\frac14\right)^2=\boxed{\frac e{384}},
$$

since $0\le\xi\le1$ and $x(1-x)\le1/4$ on $[0,1]$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [3](../../3.md)
3. [P](../../../p.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
