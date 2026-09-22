<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[resistive-pulse sensing](../../../../resistive-pulse-sensing.md) detects the change in a conducting aperture's [electric current](../../../../electric-current.md) as a particle crosses it. For generic synthetic analytes it offers electrical detection of individual events without a fluorescent label, small sensing [volumes](../../../../volume.md), and simultaneous pulse-amplitude, shape and duration information. Event counts estimate flux, while calibrated amplitudes and durations can constrain excluded [volume](../../../../volume.md) and transport. These observables are not unique molecular identifiers: shape, [electric charge](../../../../electric-charge-split.md), orientation, pore geometry, salt conditions and detector [signal bandwidth](../../../../signal-bandwidth.md) can all change a pulse.

TODO: biomolecular identification and biological [nanopore](../../../../nanopore.md) applications are user-deferred. The calculations below concern an uncharged solid pore and generic synthetic charged [polymers](../../../../polymer-split.md).

The original cross-section has [radius](../../../../radius.md) $a$ at both ends and [radius](../../../../radius.md) $b$ midway through. In the intended one-dimensional series-resistance approximation, put $s=(b-a)/l$ and

$$
r(z)=\begin{cases}a+sz,&0\leq z\leq l,\\a+s(2l-z),&l\leq z\leq2l.\end{cases}
$$

For constant ionic [electrical resistivity](../../../../electrical-resistivity.md) $\rho$, a slice contributes $d\mathcal R=\rho\,dz/[\pi r(z)^2]$. The [ionic resistance of a conical pore](../../../../ionic-resistance-of-a-conical-pore.md) then gives

$$
\mathcal R=\frac{2\rho}{\pi}\int_0^l\frac{dz}{(a+sz)^2}
=\frac{2\rho}{\pi s}\left(\frac1a-\frac1b\right),\qquad
\boxed{\mathcal R=\frac{2\rho l}{\pi ab}.}
$$

This assumes locally Ohmic transport with negligible surface conduction and approximately uniform axial [current density](../../../../current-density.md) over each slice. An uncharged wall alone does not make it an exact three-dimensional solution of [Laplace's equation](../../../../laplace-equation.md) for a rapidly varying pore. [electrical resistance](../../../../electrical-resistance.md) outside the two end planes, including reservoir access [electrical resistance](../../../../electrical-resistance.md), is excluded.

Take $V=\Phi(0)-\Phi(2l)>0$ as the potential drop inside the pore, so positive [electric current](../../../../electric-current.md) flows along $+z$. [current conservation](../../../../conserved-current.md) and [Ohm's law](../../../../ohm-s-law.md) give

$$
I_0=\frac{V}{\mathcal R}=\frac{\pi abV}{2\rho l},\qquad
\boxed{E(z)=\frac{\rho I_0}{\pi r(z)^2}=\frac{Vab}{2l\,r(z)^2}.}
$$

This is the leading cross-section-averaged axial [electric field](../../../../electric-field-split.md), and the corresponding on-axis estimate in the same approximation. It is largest at the two narrow ends and smallest at the wide centre:

$$
E(0)=E(2l)=\frac{Vb}{2la},\qquad E(l)=\frac{Va}{2lb},\qquad
\frac{E(0)}{E(l)}=\left(\frac ba\right)^2.
$$

The graph is symmetric, falls on the first half and rises on the second, with a minimum at $l$. The [electric potential difference](../../../../electric-potential-difference.md) check is $\int_0^{2l}E(z)\,dz=V$. A narrow waist at the centre would give the opposite [electric field](../../../../electric-field-split.md) sketch and would misread this source figure.

Under a small insulating-volume perturbation, a short particle produces a [position-dependent resistive pulse](../../../../position-dependent-resistive-pulse.md) with a downward excursion. If its excluded [volume](../../../../volume.md) is $\Omega$ and small compared with the local sensing [volume](../../../../volume.md), a local volume-exclusion model gives $\Delta\mathcal R(z)\propto\rho\Omega/[\pi^2r(z)^4]$. Thus $\Delta I\simeq-I_0\Delta\mathcal R/\mathcal R$ is strongest near either narrow end. A sufficiently resolved event can show two deeper end features separated by a shallower middle depression, then return to baseline. Finite particle size and acquisition [signal bandwidth](../../../../signal-bandwidth.md) round entry and exit. The original illustration below shows this conditional small-particle mechanism, not a fitted amplitude. A charged analyte can also alter local ion density and [electrical conductance](../../../../electrical-conductance.md), so the exact sign and shape need not follow excluded [volume](../../../../volume.md) alone.

<a id="1/image-pore-field-and-pulse"></a>
![](../../../../past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge/2012/paper-1-pore-signals.png)

**[Figure 1](#1/image-pore-field-and-pulse). Pore field and pulse**.

For positive drift in this coordinate, require $\mu V>0$. The [electrophoretic transit time in a conical pore](../../../../electrophoretic-transit-time-in-a-conical-pore.md) is the integral of inverse local drift speed:

$$
\Delta t=\int_0^{2l}\frac{dz}{\mu E(z)}
=\frac{2l}{\mu Vab}\int_0^{2l}r(z)^2dz
=\frac{4l}{\mu Vab}\frac{b^3-a^3}{3s}.
$$

Therefore

$$
\boxed{\Delta t=\frac{4l^2}{3\mu Vab}\frac{b^3-a^3}{b-a}
=\frac{4l^2}{3\mu V}\left(\frac ba+1+\frac ab\right).}
$$

Reverse the polarity or use $|\mu V|$ when reporting a positive transit duration in the opposite direction. The limit $b\to a$ is regular: $\Delta t\to4l^2/(\mu V)$, equal to [length](../../../../length.md) divided by uniform drift speed. Also $b/a+a/b\geq2$, so nonuniform [electric field](../../../../electric-field-split.md) makes this point-particle transit no faster than the uniform-field value at the same [length](../../../../length.md) and [electric potential difference](../../../../electric-potential-difference.md). The wide, weak-field interior dominates residence time.

The final length-dependent observations do not uniquely identify a microscopic mechanism. The calculation assumed a point-like object, constant bulk [electrophoretic mobility](../../../../electrophoretic-mobility.md), the empty-pore [electric field](../../../../electric-field-split.md), no wall residence and a drift-defined transit interval. An extended chain can sample entrance and reservoir fields simultaneously, alter its conformation and tension, and change the effective driving-to-friction ratio. These effects can make a bulk-mobility, local-field prediction underestimate the driving. For a small object, wall interactions, reversible trapping, or repeated entry excursions can add residence time that the deterministic formula omits. A length-dependent effective [electrophoretic mobility](../../../../electrophoretic-mobility.md) can likewise produce opposite deviations for short and long synthetic chains. Extra drag alone would slow a long chain, so it cannot explain a faster event without another changed [force](../../../../force-split.md), [electrophoretic mobility](../../../../electrophoretic-mobility.md) or event definition.

Discriminate these possibilities by measuring the synthetic analyte's free-solution [electrophoretic mobility](../../../../electrophoretic-mobility.md), reversing [electric potential difference](../../../../electric-potential-difference.md), varying salt and surface passivation, and comparing pulse depth with dwell time. Resolved multiple occupancy or folds can alter amplitude as well as timing. Test detector thresholds and [signal bandwidth](../../../../signal-bandwidth.md): the interval between two detected [electric current](../../../../electric-current.md) features need not equal complete contour passage. A drift–[diffusion](../../../../diffusion.md) description additionally needs entrance/exit conditions; [diffusion](../../../../diffusion.md) by itself is not a universal reason for a longer mean transit time. No unique anomalous-duration prediction follows from the provided parameters alone.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the soft matter and biological physics course of the University of Cambridge](../../../split.md)
5. [Soft Matter and Biological Physics course of the University of Cambridge](../../../../soft-matter-and-biological-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
