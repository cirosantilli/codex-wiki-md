<h1 id="1/vii/solution">Solution</h1>

↑ **Parent:** [Vii](../vii.md)

A [K correction](../../../../../../k-correction.md) accounts for observing a redshifted spectrum through a fixed [photometric passband](../../../../../../photometric-passband.md), rather than the corresponding emitted band. In the same R-band [astronomical magnitude](../../../../../../astronomical-magnitude.md) convention,

$$
M_R=m_R-5\log_{10}(d_L/10\,\mathrm{pc})-K_R.
$$

The [luminosity distance](../../../../../../luminosity-distance.md) already incorporates bolometric dimming; the additional correction depends on spectral shape and band response. At $z=3$, observed R-band light at $660\,\mathrm{nm}$ was emitted at $165\,\mathrm{nm}$, in the far ultraviolet. It is not a direct measurement of rest-frame R-band luminosity.

To fix the sign, let $L_\nu$ be emitted spectral [luminosity](../../../../../../luminosity.md) and approximate R as narrow. Counting photon energy, arrival time and the transformed frequency interval gives $F_{\nu_o}=(1+z)L_{(1+z)\nu_o}/(4\pi d_L^2)$. Thus

$$
K_R=-2.5\log_{10}\!\left[(1+z)
\frac{L_\nu((1+z)\nu_R)}{L_\nu(\nu_R)}\right],
\qquad M_{R,\rm ignored}-M_R=K_R.
$$

For an ordinary old [elliptical galaxy](../../../../../../elliptical-galaxy.md), the far-ultraviolet spectrum is weak relative to the optical, so typically $L_\nu(165\,\mathrm{nm})/L_\nu(660\,\mathrm{nm})<1/4$. Then $K_R>0$: **neglecting it overestimates the numerical absolute magnitude and underestimates the R-band luminosity**. For a young, unobscured [star-forming galaxy](../../../../../../star-forming-galaxy.md), hot stars make the far-ultraviolet strong, with an approximately flat $L_\nu$ spectrum often serving as a useful model. It gives $K_R=-2.5\log_{10}4\simeq-1.51$: **neglecting it underestimates the numerical absolute magnitude and overestimates the R-band luminosity**. Strong dust extinction or an unusual spectrum can reverse this latter sign; a galaxy label alone does not prove an exact correction. The band-integrated convention is given in [Hogg and collaborators' definition of the K-correction](https://arxiv.org/abs/astro-ph/0210394).

## ↑ Ancestors (11)

1. [Vii](../vii.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
