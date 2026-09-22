<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Interpret the reported angles as total scattering angles $\psi=2\theta$. The photon [energy](../../../../energy-split.md) gives

$$
\lambda=\frac{hc}{E_\gamma}=1.23984\times10^{-10}\,\mathrm m.
$$

Combining $2d\sin\theta=\lambda$ with the two index assignments yields

$$
a_{111}=\frac{\sqrt3\lambda}{2\sin11.4^\circ}=0.54323\,\mathrm{nm},\qquad
 a_{220}=\frac{\sqrt8\lambda}{2\sin18.8^\circ}=0.54409\,\mathrm{nm}.
$$

The slight difference is consistent with the rounded angular data, giving

$$
\boxed{a\simeq0.544\,\mathrm{nm}.}
$$

The intensity estimate needs a stated convention. The geometric [structure factors](../../../../structure-factor.md) obey $|F_{111}|^2=32|f_{111}|^2$ and $|F_{220}|^2=64|f_{220}|^2$, so equal atomic factors give a **single-directed-reflection** ratio $1/2$. For a powder line, the [powder diffraction multiplicities](../../../../powder-diffraction-multiplicity.md) are eight for $\{111\}$ and twelve for $\{220\}$. Hence a multiplicity-and-structure-factor estimate is

$$
\boxed{\frac{I_{111}}{I_{220}}\simeq\frac{8\cdot32}{12\cdot64}=\frac13}
$$

if other angle-dependent factors are neglected.

A measured integrated powder intensity also contains the [Lorentz-polarization factor](../../../../lorentz-polarization-factor.md), atomic form factor, thermal-motion factor and instrument/sample corrections. For example, in the common unpolarized symmetric powder geometry,

$$
LP(\theta)\propto\frac{1+\cos^22\theta}{\sin^2\theta\cos\theta},\qquad
\frac{LP(11.4^\circ)}{LP(18.8^\circ)}=2.9174.
$$

Including this factor but still taking equal atomic factors gives $I_{111}/I_{220}\simeq0.9725$, rather than $1/3$. More generally,

$$
\frac{I_{111}}{I_{220}}\simeq0.9725
\left|\frac{f_{111}}{f_{220}}\right|^2e^{-2(W_{111}-W_{220})}
$$

within that geometry, before other corrections. The actual form factors and measurement geometry are not supplied, so no unique precision experimental peak-height ratio follows. The values $1/2$, $1/3$ and $0.9725$ refer to distinct explicitly stated levels of approximation; a powder family must not be silently treated as one directed reflection.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
