<h1 id="32d/solution">Solution</h1>

↑ **Parent:** [32D](../32d.md)

Insert the position and momentum resolutions of the identity to obtain the unitary [Fourier transform](../../../../../fourier-transform.md)

$$
\widetilde\psi(p)=\frac1{\sqrt{2\pi\hbar}}\int_{\mathbb R}e^{-ipx/\hbar}\psi(x)\,dx,\qquad
\psi(x)=\frac1{\sqrt{2\pi\hbar}}\int_{\mathbb R}e^{ipx/\hbar}\widetilde\psi(p)\,dp.
$$

The kinetic term is multiplication by $p^2/(2m)$, and the potential has momentum kernel $\langle p|V|p'\rangle=(2\pi\hbar)^{-1}\int V(x)e^{-i(p-p')x/\hbar}\,dx$. Thus the [Schrödinger equation](../../../../../schrodinger-equation.md) becomes

$$
\left(\frac{p^2}{2m}-E\right)\widetilde\psi(p)
=-\frac1{2\pi\hbar}\int_{\mathbb R^2}V(x)e^{-i(p-p')x/\hbar}\widetilde\psi(p')\,dx\,dp'.
$$

For the attractive [delta potential](../../../../../delta-potential.md), $V(x)=-(\hbar^2\lambda/m)\delta(x)$, the kernel is the constant $-\hbar\lambda/(2\pi m)$, giving the stated positive right-hand side. For $\widetilde\psi=N/(p^2+\alpha^2)$ with $\alpha>0$, constancy of the left side requires $E=-\alpha^2/(2m)$. Since $\int dp/(p^2+\alpha^2)=\pi/\alpha$, its coefficient equation gives

$$
\boxed{\alpha=\hbar\lambda,\qquad E=-\frac{\hbar^2\lambda^2}{2m}.}
$$

Finally, transforming $\sqrt\lambda e^{-\lambda|x|}$ gives $\widetilde\psi=2\lambda^{3/2}\hbar^2/[\sqrt{2\pi\hbar}(p^2+\hbar^2\lambda^2)]$, verifying the same momentum-space form and energy.

## ↑ Ancestors (10)

1. [32D](../32d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
