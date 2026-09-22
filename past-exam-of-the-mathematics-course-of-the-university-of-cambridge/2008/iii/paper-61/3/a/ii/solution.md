<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For target [unitary operator](../../../../../../../unitary-operator.md) $U_T$ and actual propagator $U_f(T)$ on an $n$-dimensional space, minimize the [phase-insensitive unitary gate error](../../../../../../../phase-insensitive-unitary-gate-error.md)

$$
\boxed{J_{
m gate}[f]=1-\frac{|\operatorname{Tr}(U_T^\dagger U_f(T))|^2}{n^2}.}
$$

The [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) for the [Hilbert-Schmidt inner product](../../../../../../../hilbert-schmidt-inner-product.md) gives a value in $[0,1]$, because both [unitary matrices](../../../../../../../unitary-matrix.md) have squared [norm](../../../../../../../norm.md) $n$. The error is zero exactly when the matrices are proportional, namely $U_f(T)=e^{i\phi}U_T$. It therefore tests the full process, not just its action on one state, and ignores a physically irrelevant common phase. If the gate phase itself must be fixed, instead minimize $\|U_f(T)-U_T\|_{\rm HS}^2/(2n)=1-\operatorname{Re}\operatorname{Tr}(U_T^\dagger U_f(T))/n$, which vanishes only at exact equality.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 61](../../../../paper-61-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
