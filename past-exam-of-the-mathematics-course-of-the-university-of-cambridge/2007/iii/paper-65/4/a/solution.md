<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\rho_0$ denote the midplane [mass density](../../../../../../density.md) and choose the symmetry plane at $z=0$. Isothermal [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) and the [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md) give

$$
c_s^2\frac{d\ln\rho}{dz}=-\frac{d\Phi_0}{dz},\qquad
\frac{d^2\Phi_0}{dz^2}=4\pi G\rho,
$$

so $c_s^2(d^2/dz^2)\ln\rho=-4\pi G\rho$. For $\rho=\rho_0\operatorname{sech}^2(z/H)$, direct differentiation yields

$$
\frac{d\ln\rho}{dz}=-\frac2H\tanh(z/H),\qquad
\frac{d^2\ln\rho}{dz^2}=-\frac2{H^2}\operatorname{sech}^2(z/H).
$$

Thus the profile is a [self-gravitating isothermal slab](../../../../../../self-gravitating-isothermal-slab.md) when $H^2=c_s^2/(2\pi G\rho_0)$. Integrating over both sides gives $\Sigma=2\rho_0H$, hence

$$
\boxed{H=\frac{c_s^2}{\pi G\Sigma},\qquad
\rho_0=\frac{\pi G\Sigma^2}{2c_s^2}}.
$$

The corresponding potential is $\Phi_0(z)-\Phi_0(0)=2c_s^2\ln\cosh(z/H)$, whose [gradient](../../../../../../gradient.md) vanishes at the midplane and tends to $\pm2\pi G\Sigma$ far from the slab. The profile parameter $H$ is not its asymptotic exponential [mass density](../../../../../../density.md) [scale height](../../../../../../scale-height.md): that is $H/2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
