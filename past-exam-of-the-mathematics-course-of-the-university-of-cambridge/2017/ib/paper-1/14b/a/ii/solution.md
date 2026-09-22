<h1 id="14b/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The original PDF has forcing $e^{-|x|}$; the supplied TeX loses the absolute-value bars. Set $q=|\omega|$. First assume $q>0$ and $q\ne1$. The [Fourier transform of a derivative](../../../../../../../fourier-transform-of-a-derivative.md), obtained by [integration by parts](../../../../../../../integration-by-parts.md) with the boundary terms zero, is $\widetilde{u''}=-k^2\widetilde u$. Applying it and the preceding transform gives

$$
\boxed{\widetilde u(k)=\frac2{(k^2+1)(k^2+q^2)}}=\frac2{q^2-1}\left(\frac1{k^2+1}-\frac1{k^2+q^2}\right).
$$

Using the inverse [Fourier transform](../../../../../../../fourier-transform.md) pairs from part (i),

$$
\boxed{u(x)=\frac{e^{-|x|}-q^{-1}e^{-q|x|}}{q^2-1},\qquad q=|\omega|>0,\ q\ne1}.
$$

Both decay conditions hold. The first derivatives of the two exponential terms cancel at zero, so $u$ is continuously differentiable there; the second derivatives have matching limits and the [differential equation](../../../../../../../differential-equation-split.md) holds at zero as well as on both half-lines. For uniqueness, a difference solves the homogeneous equation. Decay gives $Ae^{-qx}$ on the positive half-line and $Be^{qx}$ on the negative half-line. Continuity gives $A=B$ and derivative continuity gives $-qA=qB$, forcing both to be zero.

The PDF's condition $\omega\ne\pm1$ also allows $\omega=0$, but **no decaying solution exists when $\omega=0$**. Indeed on $x>0$, $-u''=e^{-x}$ and decay forces $u=-e^{-x}$; on $x<0$, decay forces $u=-e^x$. Their one-sided derivatives at zero are $1$ and $-1$, which cannot match. The missing condition $\omega\ne0$ is therefore a genuine source omission, not a transcription repair. The transform expression at $q=0$ has a nonintegrable $k^{-2}$ singularity, consistently with this obstruction.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [14B](../../../14b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ib](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
