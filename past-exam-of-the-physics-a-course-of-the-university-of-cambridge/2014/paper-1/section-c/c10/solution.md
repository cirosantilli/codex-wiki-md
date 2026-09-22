<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

Each electromagnetic [normal mode](../../../../../normal-mode.md) is a [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator-split.md) with $E_n=(n+1/2)h\nu$. For $x=h\nu/(k_BT)$ its [canonical partition function](../../../../../canonical-partition-function.md) and occupation [probabilities](../../../../../probability.md) are

$$
Z_\nu=\frac{e^{-x/2}}{1-e^{-x}},\qquad
P_n=(1-e^{-x})e^{-nx},\qquad
\langle n\rangle=\frac1{e^x-1}.
$$

The [geometric distribution](../../../../../geometric-distribution.md) is normalized and gives thermal mode [energy](../../../../../energy-split.md) $h\nu/(e^x-1)$. The zero-point term $h\nu/2$ is not part of the thermally emitted black-body [intensity](../../../../../intensity-physics.md). The equilibrium [photon](../../../../../photon.md) [chemical potential](../../../../../chemical-potential-split.md) is zero because [photon number](../../../../../photon-number.md) is not conserved.

Counting two transverse [polarizations](../../../../../polarization-waves.md) gives $8\pi\nu^2/c^3$ modes per volume per [frequency](../../../../../frequency.md) interval. Thus the spectral [energy density](../../../../../energy-density.md) is $u_\nu=8\pi h\nu^3/[c^3(e^x-1)]$. In an isotropic radiation field, [spectral radiance](../../../../../spectral-radiance.md) is $B_\nu=cu_\nu/(4\pi)$. Transforming the spectral measure, $B_\lambda=B_\nu|d\nu/d\lambda|$, gives

$$
\boxed{B_\lambda(T)=\frac{2hc^2}{\lambda^5}\frac1{e^{hc/(\lambda k_BT)}-1}.}
$$

Here [intensity](../../../../../intensity-physics.md) [means](../../../../../expected-value-split.md) [radiance](../../../../../radiance.md) per [wavelength](../../../../../wavelength.md) and solid angle; the hemispheric spectral exitance of a black surface is $M_\lambda=\pi B_\lambda$. The extra Jacobian is essential: the [wavelength](../../../../../wavelength.md) peak is not found by simply converting the [frequency](../../../../../frequency.md) peak using $\lambda=c/\nu$.

At short [wavelength](../../../../../wavelength.md) the exponential suppresses radiation. At long [wavelength](../../../../../wavelength.md) the Rayleigh-Jeans limit is $B_\lambda\simeq2ck_BT/\lambda^4$; using classical equipartition at every [frequency](../../../../../frequency.md) instead would produce the [ultraviolet catastrophe](../../../../../ultraviolet-catastrophe.md). The [wavelength](../../../../../wavelength.md) maximum solves $5(1-e^{-x})=x$, with nonzero root $x=4.9651$, yielding [Wien's displacement law](../../../../../wien-s-displacement-law.md). For the specified [temperature](../../../../../temperature-split.md),

$$
\boxed{\lambda_{\max}=\frac{2.898\times10^{-3}\,\mathrm{m\,K}}{2.7\,\mathrm K}
\simeq1.07\,\mathrm{mm}.}
$$

Integrating the hemispheric flux gives the Stefan-Boltzmann law, $M=\sigma T^4\simeq3.01\times10^{-6}\,\mathrm{W\,m^{-2}}$. The plot uses the specified ideal [temperature](../../../../../temperature-split.md), rather than substituting a later measured value. The physical black-body description of the [cosmic microwave background](../../../../../cosmic-microwave-background-split.md) is tested by comparing the sky spectrum with an absolute reference blackbody and separating instrumental and Galactic contributions.[abstract; FIRAS comparison with a precise blackbody and limits on spectral residuals](../../../../../the-cosmic-microwave-background-spectrum-from-the-full-cobe-firas-data-set-by-dale-j-fixsen-and-others.md)

<a id="section-c/c10/image-original-ideal-spectral-radiance-per-wavelength-at-2-7-k-with-the-wavelength-peak-near-1-07-mm"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2014/paper-1-planck.png)

**[Figure 2](#section-c/c10/image-original-ideal-spectral-radiance-per-wavelength-at-2-7-k-with-the-wavelength-peak-near-1-07-mm). Original ideal spectral radiance per wavelength at 2.7 K, with the wavelength peak near 1.07 mm**.

## ↑ Ancestors (14)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
