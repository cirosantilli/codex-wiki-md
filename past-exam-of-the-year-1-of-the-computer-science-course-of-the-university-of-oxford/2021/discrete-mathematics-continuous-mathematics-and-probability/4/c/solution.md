<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At a root of size between $1$ and $2$, the spacing of [floating-point numbers](../../../../../floating-point-number.md) is $\epsilon=2^{-40}$. With ordinary stable [function](../../../../../function-split.md) evaluations, a sensible generic absolute position tolerance has scale **$2^{-40}\approx9.09\times10^{-13}$**; sub-spacing progress cannot generally be represented. This is a resolution estimate, not a lower bound excluding an accidentally exactly representable root.

Define one [bisection method](../../../../../bisection-method.md) step as replacing the current bracket by the half retaining the sign change. Starting from $[1,2]$, the width after $N$ such updates is $2^{-N}$. Therefore

$$
\boxed{N=40\quad\text{for bracket width at most }2^{-40}.}
$$

The midpoint of a bracket has an exact-arithmetic error bound of half its width. If tolerance is defined instead as that midpoint error bound, $39$ updates suffice to make it at most $2^{-40}$. Stating the convention avoids an off-by-one difference; once the endpoints are adjacent [floating-point numbers](../../../../../floating-point-number.md), their exact midpoint need not itself be representable.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
