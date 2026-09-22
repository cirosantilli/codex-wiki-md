# Offset-adjusted cumulative hazard estimator

↑ **Parent:** [Nelson–Aalen estimator](nelson-aalen-estimator.md)

Suppose individual event hazards have the additive form $h_i=h_{0i}+h_1$, where $h_{0i}$ is known and $h_1$ is common. The aggregate [counting-process intensity in survival analysis](counting-process-intensity-in-survival-analysis.md) is $\lambda=\sum_iY_ih_{0i}+Yh_1$, with $Y=\sum_iY_i$ the current [risk set](risk-set.md) size. Writing $dN=\lambda\,dt+dM$ and dividing by $Y$ gives

$$
\widehat H_1(t)=\int_0^t\frac{\mathbf1_{\{Y>0\}}}{Y}\,dN-\int_0^t\mathbf1_{\{Y>0\}}\frac{\sum_iY_ih_{0i}}{Y}\,du
=\int_0^t\mathbf1_{\{Y>0\}}h_1\,du+\int_0^t\frac{\mathbf1_{\{Y>0\}}}{Y}\,dM.
$$

The last term is a [counting-process martingale](counting-process-martingale.md) integral. This establishes the cumulative common-hazard target on the observed at-risk time range. The known offset must be averaged over the current [risk set](risk-set.md), not the initial sample. Between event jumps, its subtraction can make the unconstrained estimate decrease. If all known hazards equal $h_0$ and $Y>0$ up to $t$, the estimate reduces to the [Nelson–Aalen estimator](nelson-aalen-estimator.md) minus $H_0(t)$.

## ↑ Ancestors (6)

1. [Nelson–Aalen estimator](nelson-aalen-estimator.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-41/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-34/4/a/solution.md)
