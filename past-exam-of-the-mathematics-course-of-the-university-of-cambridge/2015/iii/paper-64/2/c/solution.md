<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For nonzero real [wavenumber](../../../../../../wavenumber.md) $k$, seek a [Fourier mode](../../../../../../fourier-mode.md) of the [Newtonian gravitational potential](../../../../../../newtonian-gravitational-potential.md) in the form $\Phi'=f(z)e^{ikx}$. Away from the razor-thin sheet, the [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md) becomes $f''-k^2f=0$. Requiring the perturbation to decay on both sides and remain continuous gives $f=Ae^{-|k||z|}$.

Integrating the [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md) through $z=0$ fixes the derivative jump:

$$
f'(0^+)-f'(0^-)=4\pi G\Sigma_0,\qquad-2|k|A=4\pi G\Sigma_0.
$$

Thus **the perturbing gravitational potential** is

$$
\boxed{\Phi'(x,z)=-\frac{2\pi G\Sigma_0}{|k|}e^{ikx-|k||z|}.}
$$

At the midplane this reduces to the [razor-thin disk Poisson kernel](../../../../../../razor-thin-disk-poisson-kernel.md). The observable real disturbance is the real part. Writing the perturbation amplitude as $\Sigma_a$ instead of $\Sigma_0$ gives the same formula with $\Sigma_a$; linearity makes it independent of the background density. The $k=0$ disturbance is a uniformly changed sheet and has potential proportional to $|z|$, rather than a decaying nonzero-[wavenumber](../../../../../../wavenumber.md) solution.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
