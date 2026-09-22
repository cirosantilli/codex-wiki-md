<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [inexact information in the SCI hierarchy](../../../../../../inexact-information-in-the-sci-hierarchy.md), replace every exact evaluation $\lambda\in\Lambda$ by a family of admissible approximations $\lambda_m$ satisfying

$$
d(\lambda_m(A),\lambda(A))\leq2^{-m}.
$$

An algorithm must converge for every admissible choice of approximations, not merely for one favored encoding.

For continuous nonsingular maps $F:X\to X$, take the evaluations to be arbitrary point queries. At precision $m$, a query at $x\in X$ returns any $y$ satisfying

$$
\boxed{d_X(y,F(x))\leq2^{-m}.}
$$

Thus the information set contains all triples $(x,m,y)$ satisfying this inequality. This is a [perfect measurement device for a dynamical system](../../../../../../perfect-measurement-device-for-a-dynamical-system.md): it can sample any state, at any requested accuracy, with no fixed noise floor. The finite-information rule still requires each terminating computation to make only finitely many such measurements.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
