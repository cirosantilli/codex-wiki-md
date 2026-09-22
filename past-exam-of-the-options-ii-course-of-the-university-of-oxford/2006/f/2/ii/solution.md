<h1 id="f/2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For small $\|\Delta\|$, the [matrix](../../../../../matrix.md) $A+\Delta=A(I+A^{-1}\Delta)$ remains invertible and its inverse is locally bounded, for example by the convergent [Neumann series](../../../../../neumann-series.md) when $\|A^{-1}\Delta\|<1$. Applying the [resolvent identity](../../../../../resolvent-identity.md) twice gives

$$
(A+\Delta)^{-1}
=A^{-1}-A^{-1}\Delta A^{-1}
+A^{-1}\Delta A^{-1}\Delta(A+\Delta)^{-1}.
$$

The last term is $O(\|\Delta\|^2)$ by that local bound. Hence the inverse map is differentiable, with

$$
\boxed{D\mathcal I_A(\Delta)=-A^{-1}\Delta A^{-1}.}
$$

This verifies the differentiability and its remainder, rather than only formally differentiating the identity $AA^{-1}=I$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [F](../../../f.md)
4. [2006](../../../../2006-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
