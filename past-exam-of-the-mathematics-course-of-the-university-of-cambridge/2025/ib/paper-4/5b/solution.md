<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

In vacuum, curl [Faraday's law](../../../../../faraday-s-law-of-induction.md) and use $\nabla\cdot E=0$ and the [Ampère-Maxwell equation](../../../../../ampere-s-circuital-law.md) to obtain

$$
\nabla^2E-\frac1{c^2}\partial_t^2E=0,\qquad c=(\mu_0\varepsilon_0)^{-1/2}.
$$

The plane wave solves this when $\omega=c|k|$ and $k\cdot E_0=0$. [Faraday's law](../../../../../faraday-s-law-of-induction.md) gives

$$
B=\operatorname{Re}\left(\frac{k\times E_0}{\omega}e^{i(k\cdot x-\omega t)}\right).
$$

For the stated wave, propagation is along $+x$ and polarization is $(0,1,1)/\sqrt2$. Thus

$$
B=\frac{E_0}{c}(0,-1,1)\frac{\cos(kx-\omega t)}{\sqrt2},
$$



$$
S=\frac{E_0^2}{\mu_0c}\cos^2(kx-\omega t)e_x,\qquad
\langle S\rangle=\frac{E_0^2}{2\mu_0c}e_x.
$$

The [Poynting vector](../../../../../poynting-vector.md) is electromagnetic energy flux, and its average is the wave intensity.

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
