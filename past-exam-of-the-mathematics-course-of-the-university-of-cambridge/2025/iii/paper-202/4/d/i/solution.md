<h1 id="4/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix $t$ and apply [Itô formula](../../../../../../../ito-s-lemma.md) to $M_s=U(t-s,X_s)$ for $0\leq s\leq t$. Its drift is

$$
-\partial_tU(t-s,X_s)+b(X_s)\partial_xU(t-s,X_s)
+\frac12\sigma(X_s)^2\partial_{xx}U(t-s,X_s)=0
$$

by the [Kolmogorov backward equation](../../../../../../../kolmogorov-backward-equation.md). Hence

$$
M_s=M_0+\int_0^s\sigma(X_u)\partial_xU(t-u,X_u)dW_u.
$$

Localization makes this a martingale, and boundedness of $U$ permits passage to the limit. Conditioning the identity $M_t=U(0,X_t)$ on $X_0$ gives

$$
U(t,X_0)=\mathbb E[U(0,X_t)\mid X_0].
$$

This is the required special case of the [Feynman-Kac formula](../../../../../../../feynman-kac-formula.md), proved directly.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [4](../../../4.md)
4. [Paper 202](../../../../paper-202-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
