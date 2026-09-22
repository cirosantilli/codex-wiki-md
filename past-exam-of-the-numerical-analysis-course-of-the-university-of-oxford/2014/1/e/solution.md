<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The initial bottom-right entry is zero, so the chosen [QR shift](../../../../qr-shift.md) is $\mu_0=0$. One valid [QR factorization](../../../../qr-decomposition.md) is $Q_0=A$, $R_0=I$, using explicitly that $A^TA=I$. The update is

$$
A_1=R_0Q_0=A.
$$

It repeats forever and never approaches a diagonal [matrix](../../../../matrix.md). With the standard positive-diagonal convention for $R$, this factorization is unique, so **the Rayleigh-shift iteration is stationary and fails to diagonalize $A$**.

The failure is independent of harmless sign conventions. The columns of $A$ are already orthonormal, so another [QR factorization](../../../../qr-decomposition.md) can only replace $Q_0$ by $AD$ and $R_0$ by $D$, where $D$ is diagonal with entries $\pm1$. Then $A_1=DAD$ still has zero diagonal and off-diagonal magnitudes one. Subsequent bottom-right shifts remain zero and the off-diagonal magnitude never decreases. The [eigenvalues](../../../../eigenvalue.md) are $+1,-1$, with equal absolute values, explaining the lack of separation in the [unshifted QR algorithm](../../../../unshifted-qr-algorithm.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
