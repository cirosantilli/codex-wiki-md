<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Adopt the planar [Fourier transform](../../../../../../fourier-transform.md) convention

$$
\widetilde g(\mathbf k)=\int e^{-i\mathbf k\cdot\mathbf x}g(\mathbf x)\,d^2x,\qquad
g(\mathbf x)=\int\frac{d^2k}{(2\pi)^2}e^{i\mathbf k\cdot\mathbf x}\widetilde g(\mathbf k).
$$

Extend the disk potential to three dimensions. The [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md) becomes

$$
(\partial_z^2-k^2)\widetilde\phi(\mathbf k,z)=4\pi G\widetilde\Sigma(\mathbf k)\delta(z),\qquad k=|\mathbf k|.
$$

For $k>0$, decay away from an isolated disk and continuity across it give $\widetilde\phi=B(\mathbf k)e^{-k|z|}$. Integration through the plane yields $-2kB=4\pi G\widetilde\Sigma$, hence the [razor-thin disk Poisson kernel](../../../../../../razor-thin-disk-poisson-kernel.md)

$$
\widetilde\phi(\mathbf k,0)=-\frac{2\pi G}{k}\widetilde\Sigma(\mathbf k).
$$

The given transform of $K(\mathbf x)=1/|\mathbf x|$ is $\widetilde K=2\pi/k$. The [convolution theorem](../../../../../../convolution-theorem.md) therefore gives the forward potential relation

$$
\boxed{\phi(\mathbf x)=-G\int\frac{\Sigma(\mathbf x')}{|\mathbf x-\mathbf x'|}\,d^2x'.}
$$

For the reverse relation, $\widetilde{\Delta_2\phi}=-k^2\widetilde\phi$, so

$$
\widetilde{K*\Delta_2\phi}
=\frac{2\pi}{k}(-k^2\widetilde\phi)
=4\pi^2G\widetilde\Sigma.
$$

Invert the transform to obtain the [thin-disk potential-density inversion](../../../../../../thin-disk-potential-density-inversion.md)

$$
\boxed{\Sigma(\mathbf x)=\frac1{4\pi^2G}\int\frac{\partial_{x'}^2\phi(\mathbf x')+\partial_{y'}^2\phi(\mathbf x')}{|\mathbf x-\mathbf x'|}\,d^2x'.}
$$

An additive constant in $\phi$ is annihilated by $\Delta_2$. These formulas hold for suitable isolated finite disks, and in a distributional or regularized sense for less regular profiles. The uniform zero-wavenumber sheet needs a separate vertical solution; the infinite [Mestel disk](../../../../../../mestel-disk.md) requires potential differences or an infrared regularization, since its absolute forward integral diverges.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
