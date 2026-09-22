<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $w=g_T^{-1}(U_T+z)$ and define

$$
f_s(z)=g_{T-s}(w)-U_T.
$$

Then $f_0(z)=z$. Differentiating with the [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md) gives

$$
\partial_sf_s(z)=-\frac2{g_{T-s}(w)-U_{T-s}}=-\frac2{f_s(z)-(U_{T-s}-U_T)}.
$$

Uniqueness for this [ordinary differential equation](../../../../../../ordinary-differential-equation.md) shows that $f_s=h_s$. At $s=T$,

$$
h_T(z)=w-U_T=g_T^{-1}(U_T+z)-U_T,
$$

which is the endpoint identity for the [Reverse Loewner flow](../../../../../../reverse-loewner-flow.md).

For $0<s<T$, the pathwise identity $h_s(z)=g_s^{-1}(U_s+z)-U_s$ is generally false. The left side is built from the reversed final driver segment $(U_{T-r}-U_T)_{0\leq r\leq s}$, whereas the right side is built from the initial segment $(U_r)_{0\leq r\leq s}$. By time reversal and symmetry of [Brownian motion](../../../../../../brownian-motion-split.md) they have the same [probability distribution](../../../../../../probability-distribution.md), but they are not equal for the given Brownian path.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
