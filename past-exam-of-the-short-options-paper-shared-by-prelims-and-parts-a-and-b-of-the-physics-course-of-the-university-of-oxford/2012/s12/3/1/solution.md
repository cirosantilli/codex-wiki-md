<h1 id="s12/3/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write the one-dimensional [random walk](../../../../../random-walk-split.md) endpoint as $x_m=\sum_{j=1}^m\xi_j$, starting at the origin. Assume unbiased, independent increments, each with $\langle\xi_j\rangle=0$ and $\langle\xi_j^2\rangle=\Delta$. Expanding the square gives

$$
\langle x_m^2\rangle=\sum_j\langle\xi_j^2\rangle+2\sum_{i<j}\langle\xi_i\xi_j\rangle.
$$

Independence makes each cross expectation $\langle\xi_i\rangle\langle\xi_j\rangle=0$. Consequently

$$
\boxed{\langle x_m\rangle=0,\qquad \langle x_m^2\rangle=m\Delta.}
$$

Uncorrelated increments with the same second moments would suffice. Unbiasedness alone does not remove correlations: persistent or anticorrelated steps need not satisfy this result. The symbol $\Delta$ is already the mean-square step size, with units of length squared.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [3](../../3.md)
3. [S12](../../../s12.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
