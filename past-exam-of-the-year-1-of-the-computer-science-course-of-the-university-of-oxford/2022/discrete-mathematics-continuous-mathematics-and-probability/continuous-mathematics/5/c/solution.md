<h1 id="continuous-mathematics/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the preceding [Taylor's theorem](../../../../../../taylor-s-theorem.md) at $t=h$ and $t=-h$, with $h>0$. The even-order terms cancel in the [central finite difference](../../../../../../central-finite-difference.md), giving

$$
d(x,h)-f'(x)=\frac{R_x(h)-R_x(-h)}{2h}.
$$

Both [Lagrange remainders](../../../../../../lagrange-remainder.md) have magnitude at most $h^3/6$, so the [triangle inequality](../../../../../../triangle-inequality.md) gives the [sharp central-secant derivative error](../../../../../../sharp-central-secant-derivative-error.md)

$$
\boxed{|d(x,h)-f'(x)|\le\frac{h^2}{6}.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [Continuous mathematics](../../../continuous-mathematics.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
