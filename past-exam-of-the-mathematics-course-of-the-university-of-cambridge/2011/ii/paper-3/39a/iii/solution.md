<h1 id="39a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [leapfrog finite-difference scheme for the diffusion equation](../../../../../../leapfrog-finite-difference-scheme-for-the-diffusion-equation.md) uses centered time and space differences:

$$
\frac{u_j^{n+1}-u_j^{n-1}}{2\Delta t}=\frac{u_{j-1}^n-2u_j^n+u_{j+1}^n}{(\Delta x)^2}.
$$

A [Fourier mode](../../../../../../fourier-mode.md) with amplification factor $z$ gives

$$
z^2+8\mu\sin^2(\theta/2)z-1=0.
$$

Writing $b=4\mu\sin^2(\theta/2)$, the roots are $z_\pm=-b\pm\sqrt{1+b^2}$. For any $\mu>0$ and any nonzero spatial frequency, $b>0$ and

$$
|z_-|=b+\sqrt{1+b^2}>1.
$$

Thus

$$
\boxed{\text{leapfrog is unstable for the heat equation for every }\mu>0.}
$$

Although the other root decays, the growing parasitic root is excited by generic starting data or perturbations, so it cannot be discarded in a stability test.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [39A](../../39a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
