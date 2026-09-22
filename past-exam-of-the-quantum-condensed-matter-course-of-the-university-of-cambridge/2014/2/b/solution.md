<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Drude model](../../../../drude-model.md) treats mobile [electric charge](../../../../electric-charge-split.md) carriers as independent particles with density $n$, signed [electric charge](../../../../electric-charge-split.md) $q$, isotropic [mass](../../../../mass.md) $m$, and [momentum relaxation time](../../../../momentum-relaxation-time.md) $\tau$. In uniform steady fields,

$$
0=q(\mathbf E+\mathbf v\times\mathbf B)-\frac{m\mathbf v}{\tau},\qquad \mathbf J=nq\mathbf v.
$$

At zero [magnetic field](../../../../magnetic-field-split.md) the [drift velocity](../../../../drift-velocity.md) is $q\tau\mathbf E/m$, giving [electrical conductivity](../../../../electrical-conductivity.md) and [electrical resistivity](../../../../electrical-resistivity.md)

$$
\boxed{\sigma_0=\frac{nq^2\tau}{m},\qquad \rho_0=\frac{m}{nq^2\tau}.}
$$

The [electrical conductivity](../../../../electrical-conductivity.md) is positive for either carrier sign. Scattering dissipates directed drift [energy](../../../../energy-split.md) into the environment; a finite steady [electric current](../../../../electric-current.md) is compatible with a short-lived drift [momentum](../../../../momentum-split.md). The independent-carrier relaxation-time approximation omits detailed band anisotropy, quantum [interference](../../../../interference-wave-propagation.md) and microscopic collision correlations.

For [electric current](../../../../electric-current.md) along $x$ and [magnetic field](../../../../magnetic-field-split.md) $B\hat{\mathbf z}$, the magnetic [force](../../../../force-split.md) deflects carriers toward one side of the sample. [electric charge](../../../../electric-charge-split.md) accumulates until a transverse Hall field cancels that [force](../../../../force-split.md) in an open transverse circuit. With $J_y=0$, $E_y=v_xB$, so

$$
\boxed{R_H=\frac{E_y}{J_xB}=\frac1{nq},\qquad \rho_{yx}=\frac{B}{nq}.}
$$

[Electrons](../../../../electron.md) have negative $R_H$ in this convention, whereas positive carriers have positive $R_H$. For a strip of thickness $d$ along $z$, the magnitude of the Hall [electric potential difference](../../../../electric-potential-difference.md) across its width is $|V_H|=|IB/(nqd)|$. Thus Hall measurements determine carrier sign and, within this one-carrier model, density, while combining $R_H$ with $\sigma_0$ determines [charge carrier mobility](../../../../charge-carrier-mobility.md) $\mu=|q|\tau/m=\sigma_0|R_H|$.

Keeping both in-plane [electric current](../../../../electric-current.md) components, the [resistivity tensor](../../../../resistivity-tensor.md) is

$$
\boldsymbol\rho=\begin{pmatrix}\rho_0&-B/(nq)\\B/(nq)&\rho_0\end{pmatrix},\qquad \boldsymbol\sigma=\boldsymbol\rho^{-1}.
$$

This fixes the off-diagonal sign convention and shows that inversion is not componentwise reciprocation. Under the Hall boundary condition $J_y=0$, the ideal one-carrier isotropic model gives $E_x/J_x=\rho_0$, independent of [magnetic field](../../../../magnetic-field-split.md): there is no ordinary longitudinal [magnetoresistance](../../../../magnetoresistance.md) in this minimal model. Multiple carrier types or anisotropic bands can change both this conclusion and the simple $R_H=1/(nq)$ inference. Their [electrical conductivity](../../../../electrical-conductivity.md) must be added before inverting to obtain the total [electrical resistivity](../../../../electrical-resistivity.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
