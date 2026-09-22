<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The barred integral in the PDF denotes a [Cauchy principal value](../../../../../../../cauchy-principal-value.md). With $p(x)=\operatorname{PV}(1/x)$ its left side is the [convolution](../../../../../../../convolution.md) $p*f$, whose [Fourier transform](../../../../../../../fourier-transform.md) is $-i\pi\operatorname{sgn}(k)\widehat f(k)$. The right side is $-1$ on $(-1,1)$ and zero outside; either direct integration or the [Fourier transform](../../../../../../../fourier-transform.md) shift rule gives

$$
\widehat{H(x-1)-H(x+1)}=-\frac{2\sin k}{k}.
$$

Thus, away from the irrelevant single point $k=0$ in the $L^2$ formulation,

$$
\widehat f(k)=-\frac{2i}{\pi}\frac{\sin k}{|k|}.
$$

By the [Fourier transform of the absolute logarithm](../../../../../../../fourier-transform-of-the-absolute-logarithm.md), the difference $\log|x-1|-\log|x+1|$ has transform $2i\pi\sin k/|k|$; its two delta terms cancel. Therefore

$$
\boxed{f(x)=\frac1{\pi^2}\log\left|\frac{x+1}{x-1}\right|}.
$$

Its endpoint logarithms are locally square integrable, and $f(x)=2/(\pi^2x)+O(x^{-3})$ at infinity, so it belongs to [L2 space](../../../../../../../l2-space-is-a-hilbert-space.md). The [Hilbert transform](../../../../../../../hilbert-transform.md) multiplier is invertible almost everywhere on this space, proving uniqueness there. Without a decay or function-space condition, one may also add a constant under the symmetric principal-value convention. If the reversed step function were used to retain the printed sign in part (i), this answer would acquire the opposite sign.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 76](../../../../paper-76-split.md)
5. [Iii](../../../../split.md)
6. [2004](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
