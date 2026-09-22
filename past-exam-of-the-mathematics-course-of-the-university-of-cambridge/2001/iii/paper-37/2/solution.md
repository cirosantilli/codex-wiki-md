<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The envelope is light and geometrically thin, so neglect its self-gravity and replace $m(r)$ and $r$ by the core's fixed $M,R$. The [stellar hydrostatic equation](../../../../../hydrostatic-pressure-support-equation.md) becomes $dP/dz=-\rho g$, where $g=GM/R^2$. Since $d\Sigma/dz=-\rho$, it gives $dP/d\Sigma=g$. Neglecting the surface pressure yields **$\boxed{P=g\Sigma}$**.

With $F=L_r/(4\pi R^2)$, the luminosity equation gives $dF/dz=\rho\epsilon$, and [radiative diffusion in a star](../../../../../radiative-diffusion-in-a-star.md) gives $dT/dz=-3\kappa\rho F/(4acT^3)$. Dividing each by $d\Sigma/dz$ gives

$$
\boxed{\frac{dF}{d\Sigma}=-\epsilon,\qquad\frac{dT}{d\Sigma}=\frac{3\kappa F}{4acT^3}.}
$$

The signs reflect that column mass increases inward: the temperature rises inward while outward flux decreases toward its source-free inner boundary.

Let $B=\mu g/\mathcal R$ for constant [mean molecular weight](../../../../../mean-molecular-weight.md). The gas [equation of state](../../../../../equation-of-state.md) and $P=g\Sigma$ give $\rho=B\Sigma/T$. With the supplied opacity and heating laws, put $y=T^7$ and $x=\Sigma^2/2$. Then

$$
\frac{dy}{d\Sigma}=\frac{21\kappa_0B}{4ac}\Sigma F,
\qquad \frac{dF}{d\Sigma}=-\epsilon_0B\Sigma T^{14}.
$$

Define $A=21\kappa_0B/(4ac)>0$. Since $dx/d\Sigma=\Sigma$, the equations become $dy/dx=AF$ and $dF/dx=-\epsilon_0By^2$. Thus the [inverse-square-opacity burning envelope](../../../../../inverse-square-opacity-burning-envelope.md) satisfies

$$
\boxed{\frac{d^2y}{dx^2}=-\omega^2y^2,\qquad\omega^2=A\epsilon_0B>0.}
$$

At the outer boundary $x=0$, the radiative-zero approximation neglects photospheric temperature relative to the burning layer, so $y=0$ and $y'=AF_s=AL/(4\pi R^2)$. This is an approximation, not an exactly zero physical photospheric temperature. At the base $x_b=\Sigma_0^2/2$, $y=y_b=T_0^7$. There is no luminosity entering from the helium core because all the luminosity is generated in the envelope, so $F(x_b)=0$ and $y'(x_b)=0$.

Multiply the second-order equation by $y'$ and integrate using the base conditions:

$$
\frac12(y')^2+\frac{\omega^2}{3}y^3=\frac{\omega^2}{3}y_b^3,
\qquad (AF_s)^2=\frac{2\omega^2}{3}y_b^3.
$$

Therefore **the base temperature obeys**

$$
\boxed{T_0=\left(\frac{3A^2}{2\omega^2}\right)^{1/21}F_s^{2/21}.}
$$

The physical branch has $y'\ge0$. A second integration gives

$$
x_b=\sqrt{\frac3{2\omega^2}}\,y_b^{-1/2}I,
\qquad I=\int_0^1\frac{dt}{\sqrt{1-t^3}}.
$$

The integral is finite because its endpoint singularity is proportional to $(1-t)^{-1/2}$. Hence $y_b\propto x_b^{-2}\propto\Sigma_0^{-4}$ and $F_s\propto y_b^{3/2}\propto\Sigma_0^{-6}$. More explicitly,

$$
\boxed{\frac{L}{4\pi R^2}=F_s=\frac{12I^3}{A\omega^2}\left(\frac{M_{\rm env}}{4\pi R^2}\right)^{-6}.}
$$

This envelope-mass comparison holds the core and the composition/opacity/heating normalizations fixed; the coefficient depends on $g$.

The steady solutions are susceptible to [thin-shell instability](../../../../../thin-shell-instability.md). At fixed overlying column, base pressure is constrained by $g\Sigma$, so $\rho\propto T^{-1}$. The nuclear heating per unit mass scales as $T^{14}$, whereas the radiative cooling through a fixed-column profile scales as $T^7$: the opacity decreases as $T^{-3}$ and diffusion adds the fourth-power temperature dependence. A positive temperature perturbation therefore increases heating faster than cooling; thin-layer expansion does not supply the strong pressure relief of a whole-star expansion. The inverse relation $F_s\propto\Sigma_0^{-6}$ also means consuming the envelope raises the corresponding steady luminosity rather than damping the burning. This idealized model predicts runaway or flashes, despite nondegenerate gas. It is not a claim that all accreting white dwarfs are unstable: sufficiently thick burning layers, altered reaction regimes or other transport/accretion conditions can stabilize burning outside these assumptions.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
