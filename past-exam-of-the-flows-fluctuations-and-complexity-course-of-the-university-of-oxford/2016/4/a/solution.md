<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For constant positive [reaction rates](../../../../reaction-rate.md), the [integrating factor](../../../../integrating-factor.md) for the [RNA](../../../../ribonucleic-acid.md) equation gives

$$
\boxed{R(t)=R_*+[R(0)-R_*]e^{-\gamma_Rt},\qquad
R_*=\frac{k_R}{\gamma_R},\qquad P_*=\frac{k_PR_*}{\gamma_P}.}
$$

For completeness, the [protein](../../../../protein-split.md) transient when $\gamma_P\ne\gamma_R$ is

$$
P(t)=P_*+[P(0)-P_*]e^{-\gamma_Pt}
+k_P[R(0)-R_*]\frac{e^{-\gamma_Rt}-e^{-\gamma_Pt}}{\gamma_P-\gamma_R}.
$$

At equal degradation rates, the last term becomes $k_P[R(0)-R_*]t e^{-\gamma_Pt}$, its continuous limit.

One transcript per minute means $k_R=1\,\mathrm{min}^{-1}$ for a single active [gene](../../../../gene.md). A [mean](../../../../expected-value-split.md) [RNA](../../../../ribonucleic-acid.md) lifetime of ten minutes means $\gamma_R=0.1\,\mathrm{min}^{-1}$, not a ten-minute half-life. The steady [mean](../../../../expected-value-split.md) is therefore $\boxed{\langle R\rangle=10}$ [RNA](../../../../ribonucleic-acid.md) molecules per cell.

For the Fano factors below, $R,P$ denote molecule numbers in a fixed cell. If they instead denote dimensional concentrations, the same deterministic equations hold after rescaling, but the conversion to molecule-number [variance](../../../../variance-split.md) introduces the cell-volume factor; [variance](../../../../variance-split.md) divided by concentration is not intrinsically a dimensionless count [Fano factor](../../../../fano-factor.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the flows, fluctuations and complexity course of the University of Oxford](../../../split.md)
5. [Flows, fluctuations and complexity course of the University of Oxford](../../../../flows-fluctuations-and-complexity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
