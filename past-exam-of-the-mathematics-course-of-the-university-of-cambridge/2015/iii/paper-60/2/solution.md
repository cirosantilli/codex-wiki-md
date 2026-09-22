<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [azimuthal derivative of a cylindrical vector Fourier mode](../../../../../azimuthal-derivative-of-a-cylindrical-vector-fourier-mode.md) must include basis rotation: the azimuthal dependence refers to the components in the rotating cylindrical basis. Since $\partial_\phi\widehat{\mathbf s}=\widehat{\boldsymbol\phi}$ and $\partial_\phi\widehat{\boldsymbol\phi}=-\widehat{\mathbf s}$, a vector amplitude $\mathbf v\propto e^{im\phi}$ obeys

$$
\partial_\phi\mathbf v=im\mathbf v+\widehat{\mathbf z}\times\mathbf v.
$$

Also $\mathbf B=(J/2)(-y,x,0)$ in [Cartesian coordinates](../../../../../cartesian-coordinate-system.md), so $(\mathbf v\cdot\nabla)\mathbf B=(J/2)\widehat{\mathbf z}\times\mathbf v$. Consequently

$$
\boxed{(\mathbf B\cdot\nabla)\mathbf b+(\mathbf b\cdot\nabla)\mathbf B
=J\widehat{\mathbf z}\times\mathbf b+\frac{imJ}{2}\mathbf b,}
$$

and the basis-rotation terms cancel in the [ideal magnetohydrodynamic induction equation](../../../../../ideal-magnetohydrodynamic-induction-equation.md):

$$
\boxed{(\mathbf B\cdot\nabla)\mathbf u-(\mathbf u\cdot\nabla)\mathbf B=\frac{imJ}{2}\mathbf u.}
$$

Here the printed $J$ is the coefficient in the specified [magnetic field](../../../../../magnetic-field.md): $\nabla\times\mathbf B=J\widehat{\mathbf z}$. If $J_{\rm phys}$ denotes SI [electric current density](../../../../../current-density.md), then $J=\mu_0J_{\rm phys}$. The field and all subsequent printed coefficients are mutually consistent with this normalization.

For a [normal mode](../../../../../normal-mode.md) with $\sigma\ne0$, induction gives $\mathbf b=imJ\mathbf u/(2\sigma)$. Substitution into the momentum equation, including the [Coriolis force](../../../../../coriolis-force.md), gives **the reduced velocity equation**

$$
\boxed{\left(\sigma+\frac{m^2J^2}{4\mu_0\rho\sigma}\right)\mathbf u
+\left(2\Omega-\frac{imJ^2}{2\mu_0\rho\sigma}\right)\widehat{\mathbf z}\times\mathbf u=-\nabla p.}
$$

Thus the coefficients are the printed $\lambda$ and $\nu$. Let $C=J^2/(\mu_0\rho)$. Inserting the allowed relation $\lambda=i\delta\nu$ and multiplying by $\sigma$ yields

$$
\sigma^2-2i\delta\Omega\sigma+\frac C4(m^2-2m\delta)=0.
$$

Hence **the [uniform-current rotating magnetohydrodynamic wave dispersion](../../../../../uniform-current-rotating-magnetohydrodynamic-wave-dispersion.md) is**

$$
\boxed{\sigma=i\delta\Omega\pm\sqrt{\frac C4(2m\delta-m^2)-\delta^2\Omega^2}.}
$$

The radicand is real. For $|m|\geq2$, $2m\delta-m^2<0$ because $|\delta|<1$, so both roots are purely imaginary. For $m=0$ the roots of the quadratic are also imaginary; any zero-frequency case must be checked in the original equations, since the elimination divided by $\sigma$. A positive real part requires

$$
2m\delta-m^2>0,\qquad
\boxed{\frac{J^2}{\mu_0\rho}>\frac{4\delta^2\Omega^2}{2m\delta-m^2}.}
$$

For integer $m$ this is possible only when $|m|=1$ and $m\delta>1/2$. Taking the conventional representative $m\geq0$ gives the printed exception $m=1$, with $\delta>1/2$ and sufficiently large $J$. Literally allowing negative integers also gives $m=-1$, $\delta<-1/2$; [complex conjugation](../../../../../complex-conjugation.md) maps $(m,\delta,\sigma)$ to $(-m,-\delta,\overline\sigma)$, so these describe the conjugate real disturbance. Purely imaginary roots describe neutral oscillatory modes; a repeated root at threshold does not itself prove boundedness of arbitrary initial perturbations.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
