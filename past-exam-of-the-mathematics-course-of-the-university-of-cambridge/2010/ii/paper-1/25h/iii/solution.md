<h1 id="25h/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**All three assertions are false.** For the transversality assertion, use $f:\mathbb R\to\mathbb R$, $f(x)=x^3$, and $Z=\{0\}$. At the preimage point the derivative is zero, so $f$ is not transverse to $Z$, yet $f^{-1}(Z)=\{0\}$ is a codimension-one submanifold. Transversality is sufficient, not necessary.

For openness of [regular values](../../../../../../regular-value.md), the smooth function $f(x)=e^{-x}(2+3\sin x)$ gives a connected-domain counterexample. Every zero has $\sin x=-2/3$ and derivative $3e^{-x}\cos x\ne0$, so zero is a [regular value](../../../../../../regular-value.md). [Critical points](../../../../../../critical-point.md) solve $\cos x-\sin x=2/3$. Choose any such point $x_0$; its value is nonzero, since simultaneous vanishing would force $\sin x=-2/3$ and $\cos x=0$. The [critical points](../../../../../../critical-point.md) $x_0+2\pi n$ have nonzero critical values $e^{-2\pi n}f(x_0)\to0$. Thus no neighborhood of the [regular value](../../../../../../regular-value.md) zero consists entirely of [regular values](../../../../../../regular-value.md). Properness would supply the missing compactness needed for the usual open-regular-value conclusion.

For the measure assertion, a constant map $f:\mathbb R\to\mathbb R$ has every point critical. Its critical-point set has positive, indeed infinite, measure. [Sard theorem](../../../../../../sard-s-theorem.md) concerns the measure of the set of critical values in the target, not the measure of [critical points](../../../../../../critical-point.md) in the domain.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [25H](../../25h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
