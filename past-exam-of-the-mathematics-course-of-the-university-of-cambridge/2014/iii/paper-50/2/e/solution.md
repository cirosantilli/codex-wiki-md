<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The trace-free [mass quadrupole moment](../../../../../../mass-quadrupole-moment.md) is diagonal:

$$
Q_{ij}=I_{zz}\,\operatorname{diag}(-1/3,-1/3,2/3).
$$

The same constant factors multiply its third derivatives, giving $\dddot Q_{ij}\dddot Q_{ij}=(2/3)(\dddot I_{zz})^2$. The [quadrupole formula](../../../../../../quadrupole-formula.md) and the preceding infall result therefore give

$$
\boxed{P(z)=\frac{m^5}{15z^4}\left(\frac1z-\frac1{z_0}\right).}
$$

For infall from infinity, $P=m^5/(15z^5)$ and $|\dot z|=\sqrt{m/(2z)}$. To find the emitted energy, integrate power over time, using $dt=|dz|/|\dot z|$:

$$
\begin{aligned}
E_{\rm rad}
&=\int_{2m}^\infty\frac{m^5}{15z^5}\sqrt{\frac{2z}{m}}\,dz\\
&=\frac{2\sqrt2\,m^{9/2}}{105}(2m)^{-7/2}
=\boxed{\frac m{420}}.
\end{aligned}
$$

The total initial mass is $2m$, so **the radiated fraction is $1/840\simeq1.19\times10^{-3}$**. The [Sun](../../../../../../sun.md) would emit that fraction of its [rest energy](../../../../../../rest-energy.md) in

$$
\boxed{t_\odot=\frac{t_{\rm all}}{840}\simeq1.76\times10^{10}\,\mathrm{yr},}
$$

under the stipulated constant [luminosity](../../../../../../luminosity.md). This is the [head-on quadrupole radiation from equal masses](../../../../../../head-on-quadrupole-radiation-from-equal-masses.md) prediction with the prescribed stopping rule. At the endpoint $|\dot z|=1/2$ and $m/z=1/2$, so extending the slow-motion weak-field formula that far is an extrapolation, not a controlled strong-field prediction.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
