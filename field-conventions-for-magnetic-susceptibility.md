# Field conventions for magnetic susceptibility

↑ **Parent:** [Magnetic susceptibility](magnetic-susceptibility.md)

In vacuum, [magnetization](magnetization.md) is zero and [magnetic flux density](magnetic-field-split.md) obeys $\mathbf B=\mu_0\mathbf H$. The applied quantities $\mathbf H_{\rm app}$ and $\mathbf B_0=\mu_0\mathbf H_{\rm app}$ mean the field of the external sources at the sample position with the sample absent. The internal [magnetic field intensity](magnetic-field-intensity.md) includes the sample's [demagnetizing field](demagnetizing-field.md); its internal [magnetic flux density](magnetic-field-split.md) additionally includes $\mu_0\mathbf M$. A field quoted in the [tesla](tesla-unit.md) is a $B$ quantity, even when an instrument informally calls it “$H$”.

For a uniformly magnetized [ellipsoid](ellipsoid.md), along a principal axis with [demagnetizing factor](demagnetizing-factor.md) $N_d$ in the [International System of Units](international-system-of-units.md),

$$
H_{\rm int}=H_{\rm app}-N_dM,\qquad
\chi_{\rm app}\equiv\frac{M}{H_{\rm app}}
=\frac{\chi_v}{1+N_d\chi_v},\qquad
\chi_v=\frac{\chi_{\rm app}}{1-N_d\chi_{\rm app}}.
$$

For a [sphere](sphere.md), $N_d=1/3$. The axial value approaches zero in the long slender [ellipsoid](ellipsoid.md) limit and the normal value approaches one in the thin flat [ellipsoid](ellipsoid.md) limit. Thus a stipulated intrinsic [volume magnetic susceptibility](volume-magnetic-susceptibility.md) $\chi_v=3$ would yield apparent values $1.5$ in a [sphere](sphere.md) and approximately $3$ in a long axial sample. These are calculated geometry effects, not measured material values. For fixed $N_d$, [implicit differentiation](implicit-differentiation.md) gives the same conversion for local [differential magnetic susceptibility](differential-magnetic-susceptibility.md), $dM/dH_{\rm app}=\chi_{\rm diff}/(1+N_d\chi_{\rm diff})$.

## ↑ Ancestors (5)

1. [Magnetic susceptibility](magnetic-susceptibility.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Demagnetizing field](demagnetizing-field.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2019/section-b/6/solution.md)
