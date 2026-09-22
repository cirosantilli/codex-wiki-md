<h1 id="1/b/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Remove the two reciprocal tails by setting

$$
r(x)=w(x)-c_+u(x)+c_-u(-x).
$$

The assumed $O(x^{-2})$ remainder at each end and [local integrability](../../../../../../../locally-integrable-function.md) on bounded intervals imply $r\in L^1(\mathbb R)$. Its [Fourier transform](../../../../../../../fourier-transform.md) $\widehat r$ is therefore [continuous](../../../../../../../continuous-function.md) at zero. Since $\widehat{u(-\mathord\cdot)}(\lambda)=\widehat u(-\lambda)$,

$$
\widehat w(\lambda)
=c_+\widehat u(\lambda)-c_-\widehat u(-\lambda)+\widehat r(\lambda).
$$

Parts (iv) and (v) show that both requested one-sided limits exist. If $L_+$ denotes the limit from positive frequencies and $L_-$ the limit from negative frequencies, then the common value $\widehat r(0)$ cancels and

$$
\begin{aligned}
L_+-L_-
&=(c_++c_-)
\lim_{\lambda\downarrow0}
\bigl[f_+(\lambda)-f_-(-\lambda)\bigr]\\
&=\boxed{-i\pi(c_++c_-)}.
\end{aligned}
$$

This is the [universal jump caused by reciprocal tails](../../../../../../../fourier-transform-of-a-function-with-reciprocal-tails.md).

## ↑ Ancestors (12)

1. [Vi](../vi.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 327](../../../../paper-327-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
