<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Factor $A+H=A(I+A^{-1}H)$. The [determinant](../../../../determinant.md) expansion near the identity is

$$
\det(I+K)=1+\operatorname{tr}K+O(\|K\|^2):
$$

the linear terms in the permutation formula come from choosing one diagonal increment and all remaining identity entries. Therefore

$$
\det(A+H)=\det A+\det A\operatorname{tr}(A^{-1}H)+O(\|H\|^2).
$$

The required [Fréchet derivative](../../../../frechet-derivative.md) is the [linear functional](../../../../linear-functional.md)

$$
\boxed{D(\det)_A(H)=\det(A)\operatorname{tr}(A^{-1}H).}
$$

The quadratic remainder proves full differentiability, rather than only the existence of each directional [derivative](../../../../derivative.md). This is the [derivative of the determinant](../../../../derivative-of-the-determinant.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
