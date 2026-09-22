<h1 id="41e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the same Fourier mode, the [leapfrog finite-difference scheme for the diffusion equation](../../../../../../leapfrog-finite-difference-scheme-for-the-diffusion-equation.md) gives

$$
r^{n+1}=r^{n-1}-2qr^n,
\qquad
p(r)=r^2+2qr-1.
$$

The two amplification roots are

$$
r_\pm=-q\pm\sqrt{1+q^2}.
$$

For every nonzero mode $q>0$, one has

$$
|r_-|=q+\sqrt{1+q^2}>1.
$$

Thus every $\mu>0$ admits a growing Fourier mode, and

$$
\boxed{\text{the leapfrog scheme is unstable for every }\mu>0.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [41E](../../41e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
