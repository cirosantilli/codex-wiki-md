<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Normalize each reporter by its mean intensity, after correcting background and unequal brightness, so equal expression lies on $y=x$. Write $x=1+e+i_C$, $y=1+e+i_Y$, where the common fluctuation $e$ is [extrinsic gene-expression noise](../../../../extrinsic-gene-expression-noise.md) and the independent reporter-specific fluctuations $i_C,i_Y$ are [intrinsic gene-expression noise](../../../../intrinsic-gene-expression-noise.md). The [extrinsic gene-expression noise](../../../../extrinsic-gene-expression-noise.md) includes shared variation in cell size, expression machinery and growth state; [intrinsic gene-expression noise](../../../../intrinsic-gene-expression-noise.md) includes independent molecular production and removal events at each reporter.

If [intrinsic gene-expression noise](../../../../intrinsic-gene-expression-noise.md) is much smaller, points form a narrow elongated cloud along $y=x$: a cell that is bright in cyan is usually bright in yellow. If the two contributions have comparable magnitude, the cloud is still positively correlated but has substantial width perpendicular to $y=x$, because the two reporters can differ within the same cell. With [variance](../../../../variance-split.md) $\sigma_e^2$ in $e$ and equal [variance](../../../../variance-split.md) $\sigma_i^2$ in each independent intrinsic term,

$$
\operatorname{Cov}(x,y)=\sigma_e^2,\qquad
\operatorname{Var}(y-x)=2\sigma_i^2,\qquad
\operatorname{Corr}(x,y)=\frac{\sigma_e^2}{\sigma_e^2+\sigma_i^2}.
$$

Equal intrinsic and extrinsic [variances](../../../../variance-split.md) therefore give [correlation coefficient](../../../../pearson-correlation-coefficient.md) $1/2$, rather than an uncorrelated circular cloud. For mean-normalized reporters, $\eta_{\rm int}^2=\langle(x-y)^2\rangle/2$ and $\eta_{\rm ext}^2=\langle xy\rangle-1$. Measurement noise must be separately estimated before assigning perpendicular scatter to expression itself. These are the geometric diagnostics of the original dual-reporter experiment.[Figure 1 and definition of intrinsic and extrinsic noise: within-cell reporter differences versus correlated cell-to-cell variation](../../../../stochastic-gene-expression-in-a-single-cell-by-michael-b-elowitz-and-others.md)

The lower panels of [c](../c.md) show these two cases. Repeated observations of one cell can move both along and across the diagonal; a static population cloud alone does not determine the time scales of the fluctuations.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
