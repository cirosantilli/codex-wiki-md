<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Normalize the Gaussian trial first. The [Gaussian integral](../../../../../gaussian-integral.md) gives

$$
1=C^2\sqrt{\frac\pi\alpha},\qquad\boxed{C=\pm\left(\frac\alpha\pi\right)^{1/4}.}
$$

Its second and fourth moments are $\langle x^2\rangle=1/(2\alpha)$ and $\langle x^4\rangle=3/(4\alpha^2)$. Since $\psi'=-\alpha x\psi$, the kinetic term is $\int(\psi')^2=\alpha^2\langle x^2\rangle=\alpha/2$. At the specified coupling, the [energy](../../../../../energy-split.md) is therefore

$$
E(\alpha)=\frac\alpha2+\frac1{2\alpha}+\frac3{2\alpha^2}.
$$

The stationary condition is

$$
E'(\alpha)=\frac{\alpha^3-\alpha-6}{2\alpha^3}=0,\qquad\alpha^3-\alpha-6=(\alpha-2)(\alpha^2+2\alpha+3).
$$

The quadratic factor is positive for real $\alpha$, so the unique positive stationary width is $\alpha=2$. Also $E''=\alpha^{-3}+9\alpha^{-4}>0$ and $E$ diverges at both ends of $\alpha>0$, proving a global minimum within this trial family. Its value is

$$
\boxed{E_{\rm trial,min}=\frac{13}{8},\qquad\psi_*(x)=\pm(2/\pi)^{1/4}e^{-x^2}.}
$$

The associated [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md) is

$$
\boxed{-\psi''+(x^2+2x^4)\psi=E\psi,\qquad\psi\in L^2(\mathbb R),\quad\psi\to0\text{ at }\pm\infty.}
$$

Here $\rho=1$, $\sigma=x^2+2x^4$ and $w=1$. The [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) makes the exact lowest [eigenvalue](../../../../../eigenvalue.md) the minimum over all normalized admissible states. Restricting to Gaussians can only raise this minimum, hence $\boxed{E_0\leq13/8}$. The inequality is strict because $H\psi_*/\psi_*=2-3x^2+2x^4$ is not constant: the trial is not an exact [eigenfunction](../../../../../eigenfunction.md). This is the [Gaussian trial for a quadratic-plus-quartic oscillator](../../../../../gaussian-trial-for-a-quadratic-plus-quartic-oscillator.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
