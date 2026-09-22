<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Extend $f$ by zero outside $[0,1]$. Since the [Fourier transform](../../../../../../fourier-transform.md) of $e^{-|x|}$ is $2/(1+\xi^2)>0$,

$$
\langle Kf,f\rangle
=\frac1{2\pi}\int_{\mathbb R}
\frac{2}{1+\xi^2}|\widehat f(\xi)|^2\,d\xi>0
$$

for $f\ne0$. Thus every eigenvalue is positive. From the relation in part (b),

$$
\boxed{\lambda=\frac2{1+\omega^2}>0}.
$$

The transcendental equation has its successive roots in intervals separated by the poles and zeros of $\tan\omega$, so $\omega_n$ grows linearly with $n$. Hence

$$
\boxed{\lambda_n=\frac2{1+\omega_n^2}=O(n^{-2})}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
