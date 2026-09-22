<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $m_{ij}=m_{ij}^{(\pm2)}$ and $h=h^{(\pm2)}$. Since $m_{ij}e^ie^j=\tfrac12(1-\mu^2)e^{\pm2i\varphi}$, the line-of-sight solution is

$$
\Theta=-\frac{e^{i\mathbf k\cdot\mathbf x}}{2\sqrt2}
m_{ij}e^ie^j
\int_0^\eta d\eta'\,\dot h(\eta')e^{-ik(\eta-\eta')\mu}.
$$

The angular pattern $m_{ij}e^ie^j$ is proportional to $Y_{2,\pm2}$. Projecting onto this [spherical harmonic](../../../../../../spherical-harmonic.md) multiplies its coefficient by

$$
\frac{\int_{-1}^{1}(1-\mu^2)^2e^{-ix\mu}\,d\mu}
{\int_{-1}^{1}(1-\mu^2)^2\,d\mu}
=15\frac{j_2(x)}{x^2},
$$

where $x=k(\eta-\eta')$ and $j_2$ is a [Spherical Bessel function](../../../../../../spherical-bessel-function.md). Thus the quadrupole is

$$
\boxed{\Theta\big|_{\ell=2}
=-\frac{15}{2\sqrt2}m_{ij}e^ie^j e^{i\mathbf k\cdot\mathbf x}
\int_0^\eta d\eta'\,\dot h(\eta')\frac{j_2(k(\eta-\eta'))}{[k(\eta-\eta')]^2}}.
$$

Use the [isotropic tensor integral](../../../../../../isotropic-tensor-integral.md)

$$
\int\frac{d\Omega_e}{4\pi}e^ie^je^ae^b
=\frac1{15}(\delta^{ij}\delta^{ab}+\delta^{ia}\delta^{jb}+\delta^{ib}\delta^{ja}).
$$

Because $m$ is symmetric and trace-free, contracting this with $m_{ab}$ gives $2m^{ij}/15$. Substitution into the paper's signed [neutrino tensor anisotropic stress](../../../../../../neutrino-tensor-anisotropic-stress.md) therefore gives

$$
\boxed{\Pi^{ij}=2\sqrt2\,\bar\rho_\nu\,e^{i\mathbf k\cdot\mathbf x}m^{ij}
\int_0^\eta d\eta'\,\dot h(\eta')K(k(\eta-\eta'))},
\qquad K(x)=\frac{j_2(x)}{x^2}.
$$

The [neutrino tensor free-streaming kernel](../../../../../../neutrino-tensor-free-streaming-kernel.md) is finite at the origin, with $K(0)=1/15$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
