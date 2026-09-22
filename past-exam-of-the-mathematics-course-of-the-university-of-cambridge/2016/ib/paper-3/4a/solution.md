<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

Use [Fourier inversion](../../../../../fourier-inversion-theorem.md) with the stated [Fourier transform](../../../../../fourier-transform.md) convention:

$$
f(x)=\frac1{2\pi}\int_{-\infty}^{\infty}\frac{-2ik}{p^2+k^2}e^{ikx}\,dk.
$$

For $x<0$, close the [contour integral](../../../../../contour-integral.md) in the lower half-plane, where $|e^{ikx}|=e^{-x\operatorname{Im}k}$ decays. [Jordan lemma](../../../../../jordan-s-lemma.md) eliminates the large semicircle. The contour is clockwise, so the [residue theorem](../../../../../residue-theorem.md) supplies $-2\pi i$ times the residue at $k=-ip$. That [simple pole](../../../../../simple-pole.md) has

$$
\operatorname{Res}_{k=-ip}\left(\frac{-2ik}{(k-ip)(k+ip)}e^{ikx}\right)
=-ie^{px}.
$$

Consequently

$$
\boxed{f(x)=-e^{px},\qquad x<0.}
$$

The minus sign uses both the clockwise orientation and the residue $-i e^{px}$; it is consistent with the full odd function $\operatorname{sgn}(x)e^{-p|x|}$ away from zero.

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
