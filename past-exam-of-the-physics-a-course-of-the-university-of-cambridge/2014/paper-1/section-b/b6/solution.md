<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

Set $k=\sqrt{2mE}/\hbar$ and $\kappa=\sqrt{2m(U-E)}/\hbar$. For unit incident [amplitude](../../../../../wave-amplitude.md), use $\psi=e^{ikx}+r e^{-ikx}$ on the left and $\psi=t_s e^{-\kappa x}$ on the right; the growing exponential is excluded at infinity. Continuity at zero gives $1+r=t_s$ and $ik(1-r)=-\kappa t_s$. Thus

$$
r=\frac{k-i\kappa}{k+i\kappa}=e^{i\delta},\qquad |r|^2=1,
\qquad\boxed{\delta=-2\arctan(\kappa/k)=-2\arccos\sqrt{E/U}.}
$$

The phase is chosen in $(-\pi,0)$ for $0<E<U$. The [evanescent wave](../../../../../evanescent-wave.md) is $\psi(x)=2k\,e^{-\kappa x}/(k+i\kappa)$ for $x>0$. Its [probability density](../../../../../probability-density.md) is nonzero, but its [probability current](../../../../../probability-current.md) $j=(\hbar/m)\operatorname{Im}(\psi^*\psi')$ is zero. Penetration into a forbidden region therefore does not require transmitted flux through a semi-infinite step.

For a finite rectangular barrier, matching both interfaces gives

$$
\mathcal T=\left[1+\frac{U^2}{4E(U-E)}\sinh^2(\kappa a)\right]^{-1}
\simeq\frac{16E(U-E)}{U^2}e^{-2\kappa a}.
$$

The approximation requires **$\kappa a\gg1$**, or a width much greater than the evanescent penetration [length](../../../../../length.md). The tunnelling exponent is $-2a\sqrt{2m(U-E)}/\hbar$; its factor of two converts an [amplitude](../../../../../wave-amplitude.md) decay to a [probability](../../../../../probability.md) decay. For the [electron](../../../../../electron.md) parameters, $\kappa=1.984\times10^9\,\mathrm{m^{-1}}$ and $\kappa a=19.84$. Therefore

$$
\boxed{\mathcal T\simeq3e^{-39.68}=1.75\times10^{-17}.}
$$

Keeping only the exponential gives $5.83\times10^{-18}$; the matched-interface prefactor accounts for the factor of three.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
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
