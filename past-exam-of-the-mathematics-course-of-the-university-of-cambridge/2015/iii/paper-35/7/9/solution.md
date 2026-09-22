<h1 id="7/9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Applying [death-only rate correction under exponential censoring](../../../../../../death-only-rate-correction-under-exponential-censoring.md) to the death fraction and combined-rate estimate, **the corrected plug-in death rate is**

$$
\boxed{\widehat\lambda_{\text{plug-in}}
=\frac23\times0.3=0.2\ \text{year}^{-1}.}
$$

The corresponding censoring-rate estimate is $0.1\ \text{year}^{-1}$. This correction is consistent under the [independent](../../../../../../independent-random-variables.md) exponential competition model: the death-only conditional rate estimates $s$ and the observed fraction estimates $\lambda/s$.

There is an important distinction from the full-data [maximum-likelihood estimate](../../../../../../maximum-likelihood-estimator.md). If $T_D$ and $T_C$ are total observed follow-up for the 100 deaths and 50 censored subjects, the full likelihood for both rates is

$$
L(\lambda,\gamma)\propto\lambda^{100}\gamma^{50}
 e^{-(\lambda+\gamma)(T_D+T_C)},
\qquad
\boxed{\widehat\lambda_{\mathrm{full}}=\frac{100}{T_D+T_C}.}
$$

The reported death-only rate determines $T_D=100/0.3$, but supplies no $T_C$, so the exact full-data estimate cannot be reconstructed from the numerical summaries alone. The value $0.2$ is the requested corrected rate using those summaries; it need not equal the realised full-data maximum-likelihood estimate. The full analysis should use the actual censored follow-up whenever available.

## ↑ Ancestors (11)

1. [9](../9.md)
2. [7](../../7.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
