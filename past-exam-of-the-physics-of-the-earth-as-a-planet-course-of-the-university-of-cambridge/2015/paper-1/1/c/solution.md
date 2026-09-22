<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [seismic source inversion](../../../../../seismic-source-inversion.md), collect calibrated, consistently filtered samples from all available stations and components into a data [vector](../../../../../vector.md) $\mathbf d$. For each trial source position and origin time, compute the corresponding [elastodynamic Green tensor](../../../../../elastodynamic-green-tensor.md) in an [Earth](../../../../../earth.md) model, including the instrument response used for the data. Write the symmetric [seismic moment tensor](../../../../../seismic-moment-tensor.md) in six independent symmetric basis [tensors](../../../../../tensor.md):

$$
\mathbf M=\sum_{j=1}^6m_j\mathbf B_j,
\qquad
\mathbf d=\mathbf G(\mathbf q)\mathbf m+\boldsymbol\epsilon,
\qquad \mathbf q=(x_s,y_s,z_s,t_s).
$$

Each column of $\mathbf G$ is the synthetic [seismogram](../../../../../seismogram.md) for one basis [tensor](../../../../../tensor.md). An off-diagonal basis [tensor](../../../../../tensor.md) contains both symmetric entries, so the double contraction and its factors of two remain consistent.

A suitable objective is

$$
\chi^2(\mathbf q,\mathbf m)
=[\mathbf d-\mathbf G(\mathbf q)\mathbf m]^T
\mathbf C_d^{-1}[\mathbf d-\mathbf G(\mathbf q)\mathbf m],
$$

with noise [covariance](../../../../../covariance.md) $\mathbf C_d$; a justified penalty can be added for [regularization](../../../../../regularization.md). At fixed $\mathbf q$, solve for the six entries of $\mathbf m$ by [weighted least squares](../../../../../weighted-least-squares.md), preferably using a [QR decomposition](../../../../../qr-decomposition.md) or [singular value decomposition](../../../../../singular-value-decomposition.md) rather than explicitly inverting the matrix of the normal equations. Then search over the four nonlinear parameters using a coarse location/time grid followed by local refinement. **This [variable projection](../../../../../variable-projection.md) reduces a ten-parameter search to a four-parameter nonlinear search with an inner six-parameter [linear](../../../../../linearity.md) fit.** Merely having more than ten data samples does not ensure identifiability: the [design matrix](../../../../../design-matrix.md) must have adequate rank and the network must resolve the source's radiation patterns.

Potential errors include inaccurate [velocity](../../../../../velocity.md), [density](../../../../../density.md), anisotropy and attenuation in the assumed [Earth](../../../../../earth.md) model; neglected finite rupture and source-time effects; timing, instrument calibration or component-orientation errors; correlated noise; uneven station coverage; and tradeoffs between depth, origin time and the moment [tensor](../../../../../tensor.md). Imposing a [double-couple seismic source](../../../../../double-couple-seismic-source.md) mechanism without evidence can hide genuine non-double-couple components. [Regularization](../../../../../regularization.md) also changes the recovered source and should be reported.

Inspect residuals, singular values, recovery of synthetic sources and uncertainty under resampling or noise perturbations. Linearized [covariance](../../../../../covariance.md) or a [posterior distribution](../../../../../bayesian-posterior.md) can quantify uncertainty within the assumed forward model, but does not automatically account for errors in that model. A good waveform fit alone is insufficient evidence that all ten parameters are uniquely recovered.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics of the Earth as a Planet course of the University of Cambridge](../../../../split.md)
6. [Physics of the Earth as a Planet course of the University of Cambridge](../../../../../physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
