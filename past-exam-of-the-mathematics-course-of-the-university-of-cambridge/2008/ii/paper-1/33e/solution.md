<h1 id="33e/solution">Solution</h1>

↑ **Parent:** [33E](../33e.md)

For a spherically symmetric potential, take the polar axis along the momentum transfer $q$. Its angular integral is

$$
\int e^{-iqr\cos\vartheta}\,d\Omega=2\pi\int_{-1}^1e^{-iqr v}\,dv=4\pi\frac{\sin(qr)}{qr}.
$$

The [first Born approximation](../../../../../born-approximation.md) consequently gives $f(\theta)=-2m(\hbar^2q)^{-1}\int_0^\infty rV(r)\sin(qr)\,dr$. The incident and scattered [wave vectors](../../../../../wavevector.md) both have magnitude $k$, so $q^2=2k^2(1-\cos\theta)$ and $\boxed{q=2k\sin(\theta/2)}$.

For the exponential potential, $\int_0^\infty re^{-(1-iq)r}\,dr=(1-iq)^{-2}$. Taking the imaginary part gives $2q/(1+q^2)^2$. Therefore

$$
\boxed{f(\theta)=-\frac{4mV_0}{\hbar^2[1+4k^2\sin^2(\theta/2)]^2}.}
$$

The [differential scattering cross-section](../../../../../differential-scattering-cross-section.md) is proportional to $[1+q^2]^{-4}$. At large $k$, substantial intensity requires $q=O(1)$, hence $\theta=O(k^{-1})$. For a precise convention, the half-intensity cone has half-angle $\theta_{1/2}\sim\sqrt{2^{1/4}-1}/k$. Its full angular width is twice that. The exponential's range has been set to one; restoring range $a$ gives width of order $1/(ka)$. As [energy](../../../../../energy.md) increases, the scattering therefore concentrates into the forward cone.

## ↑ Ancestors (10)

1. [33E](../33e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
