<h1 id="3a/solution">Solution</h1>

↑ **Parent:** [3A](../3a.md)

With the stated [Fourier transform](../../../../../fourier-transform.md) convention, [Fourier inversion](../../../../../fourier-inversion-theorem.md) gives

$$
f(x)=\frac1{2\pi}\int_{-\infty}^{\infty}
\frac{-2ik}{p^2+k^2}e^{ikx},dk.
$$

For $x>0$, close the contour in the upper half-plane. [Jordan lemma](../../../../../jordan-s-lemma.md) removes the semicircle contribution, and the only enclosed pole is $k=ip$. Its residue is

$$
\operatorname{Res}_{k=ip}
\frac{-2ik e^{ikx}}{(k-ip)(k+ip)}=-i e^{-px}.
$$

The [residue theorem](../../../../../residue-theorem.md) therefore yields

$$
\boxed{f(x)=e^{-px},\qquad x>0}.
$$

## ↑ Ancestors (10)

1. [3A](../3a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
