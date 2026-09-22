<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The four-parameter [panel-observed multi-state likelihood](../../../../../../../panel-observed-multi-state-likelihood.md) requires the following additional assumptions.

- **Irreversibility:** the [chronic disease](../../../../../../../chronic-disease.md) can progress but cannot improve, so $q_{21}=q_{32}=0$ and state 3 is absorbing. Merely permitting transitions between adjacent states does not impose this; allowing regression would require additional [transition intensities](../../../../../../../transition-intensity.md).
- **Piecewise-constant age:** the current age is held at 50 and 55 over the respective observation intervals. Actual age changes continuously, and a five-year interval can be too long for this approximation when the age effect is substantial.
- **Log-linear age effects and common rates:** the specified age functions apply to the patient, without unmodelled heterogeneity or other changing covariates.
- **Observation mechanism:** disease states are recorded without misclassification, and examination times or dropout carry no additional information about the underlying process once the modelled history is given. A new visit only one year after a five-year gap might have been prompted by worsening symptoms, making the observation schedule informative.

If age is instead updated continuously, the model is time-inhomogeneous and the displayed homogeneous transition formula is not exact. For example, set

$$
\Lambda(u,v)=\int_u^v q_{12}(A)\,dA,\qquad M(u,v)=\int_u^v q_{23}(A)\,dA.
$$

Then the exact irreversible [likelihood contribution](../../../../../../../likelihood-contribution.md) is

$$
L=e^{-\Lambda(50,55)}\left[1-e^{-\Lambda(55,56)}
-\int_{55}^{56}e^{-\Lambda(55,u)}q_{12}(u)e^{-M(u,56)}\,du\right].
$$

Thus **the simple closed form uses an explicit frozen-age approximation**; adjacency alone and continuously evolving age do not determine that form.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
