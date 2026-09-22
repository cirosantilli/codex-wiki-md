# Complex visibility

↑ **Parent:** [Radio interferometry](radio-interferometry.md)

A complex visibility is a calibrated complex correlation of the signals received at a particular [interferometric baseline](interferometric-baseline.md). In a narrow field, with scalar radiation, the [far-field approximation for an outgoing source](far-field-approximation-for-an-outgoing-source.md), a narrow frequency channel, negligible noncoplanar phase curvature and a steady sky of mutually incoherent emitters,

$$
V(u,v)=\iint A(l,m)I(l,m)e^{-2\pi i(ul+vm)}\,dl\,dm.
$$

Here $l,m$ are small dimensionless sky-direction offsets, $I$ is brightness in the chosen channel, and $A$ is the [primary beam](primary-beam.md). This is the [Fourier transform](fourier-transform-split.md) of beam-weighted brightness. The two-dimensional formula requires those approximations: a wide field generally needs the third baseline coordinate and curved sky geometry.

For an explicit one-dimensional derivation, set the [primary beam](primary-beam.md) to one over the small field, and place independent emitters at angular offsets $\theta_j$. Choose a [wave phase](phase-waves.md) convention in which, after removing the [phase centre](phase-centre.md)'s delay, their received [complex amplitudes](complex-amplitude.md) are

$$
E_1(t)=\sum_j a_j(t),\qquad
E_2(t)=\sum_j a_j(t)e^{2\pi i u\theta_j},\qquad
\langle a_j a_k^*\rangle=I_j\delta_{jk}.
$$

Here $\delta_{jk}$ is the [Kronecker delta](kronecker-delta.md) and angle brackets denote an [expected value](expected-value-split.md) estimated by time averaging a steady signal. The last equality states mutual incoherence: different emitters have zero averaged cross term, although each emitter's two received copies remain correlated. Multiplying and averaging gives

$$
V(u)=\langle E_1E_2^*\rangle
=\sum_{j,k}\langle a_j a_k^*\rangle e^{-2\pi i u\theta_k}
=\sum_j I_j e^{-2\pi i u\theta_j}.
$$

For continuous brightness this becomes $V(u)=\int I(\theta)e^{-2\pi i u\theta}\,d\theta$. Real brightness implies the [Hermitian symmetry](hermitian-symmetry.md) $V(-u)=V(u)^*$; it does not require brightness to be even. In particular, an asymmetric real source usually has a nonzero imaginary [complex visibility](complex-visibility.md). At zero baseline, $V(0)=\sum_j I_j$ is the total beam-weighted source strength. Ordinary separated-element correlations need not measure that zero-baseline value.

**Table of contents**

- [Visibility of a one-dimensional uniform source](visibility-of-a-one-dimensional-uniform-source.md)
- [Visibility of a uniform rectangular source](visibility-of-a-uniform-rectangular-source.md)
- [Fringe stopping](fringe-stopping.md)
  - [Field-dependent averaging losses in radio interferometry](field-dependent-averaging-losses-in-radio-interferometry.md)
    - [Bandwidth decorrelation of a point source](bandwidth-decorrelation-of-a-point-source.md)
- [Primary beam](primary-beam.md)

## ↑ Ancestors (8)

1. [Radio interferometry](radio-interferometry.md)
2. [Aperture synthesis](aperture-synthesis.md)
3. [Radio astronomy](radio-astronomy.md)
4. [Observational astronomy](observational-astronomy.md)
5. [Astrophysics](astrophysics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Aperture synthesis](aperture-synthesis.md)
- [Complex visibility](complex-visibility.md)
- [Correlator](correlator.md)
- [Dirty beam](dirty-beam.md)
- [Dirty image](dirty-image.md)
- [Fringe stopping](fringe-stopping.md)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2012/paper-1/1/solution.md)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2014/paper-1/3/b/solution.md)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2015/paper-1/2/solution.md)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2016/paper-1/1/solution.md)
- [Phase centre](phase-centre.md)
- [Primary beam](primary-beam.md)
- [Radio interferometer calibration](radio-interferometer-calibration.md)
- [Radio interferometry](radio-interferometry.md)
- [Radio telescope](radio-telescope.md)
- [Synthesized beam](synthesized-beam.md)
- [Two-point-source aperture synthesis](two-point-source-aperture-synthesis.md)
- [Visibility-domain matched filter](visibility-domain-matched-filter.md)
