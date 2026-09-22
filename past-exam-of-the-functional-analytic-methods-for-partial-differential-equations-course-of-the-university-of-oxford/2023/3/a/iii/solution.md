<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

By the definition in (i), $u$ itself is an admissible test in the [weak formulation](../../../../../weak-formulation.md). Hence

$$
\|\nabla u\|_{L^2(B)}^2=\int_Eu\,dx\leq\int_E|u|\,dx=\|u\|_{L^1(E)}.
$$

The absolute value makes a proof of positivity unnecessary. [Holder inequality](../../../../../holder-inequality.md) with exponents $6$ and $6/5$, followed by the zero-boundary [Sobolev inequality](../../../../../sobolev-inequality.md), gives

$$
\|u\|_{L^1(E)}\leq |E|^{5/6}\|u\|_{L^6(B)}
\leq C_S|E|^{5/6}\|\nabla u\|_{L^2(B)}.
$$

Taking square roots of both estimates proves exactly the requested chain:

$$
\boxed{\|\nabla u\|_2\leq\|u\|_{L^1(E)}^{1/2}
\leq C_S^{1/2}|E|^{5/12}\|\nabla u\|_2^{1/2}.}
$$

If $\|\nabla u\|_2=0$, the zero-boundary [Poincaré inequality](../../../../../poincare-inequality.md) gives $u=0$ and the conclusion follows. Otherwise divide the first-to-last estimate by $\|\nabla u\|_2^{1/2}$ and square, obtaining $\|\nabla u\|_2\leq C_S|E|^{5/6}$. Finally the same [Poincaré inequality](../../../../../poincare-inequality.md) gives

$$
\boxed{\|u\|_{H^1(B)}\leq C|E|^{5/6}.}
$$

All constants depend only on the fixed unit ball and the dimension, and are independent of $E$ and $u$. If $|E|=0$, testing the homogeneous equation with $u$ gives the same zero solution directly.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analytic methods for partial differential equations course of the University of Oxford](../../../../split.md)
6. [Functional analytic methods for partial differential equations course of the University of Oxford](../../../../../functional-analytic-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
