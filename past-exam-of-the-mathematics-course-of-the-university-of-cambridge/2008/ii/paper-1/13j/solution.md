<h1 id="13j/solution">Solution</h1>

↑ **Parent:** [13J](../13j.md)

The array has $K=10$ replicates, $I=2$ levels of factor $a$, and $J=3$ levels of factor $b$, giving $n=60$. R vectorizes an array with the first index changing fastest, then the second, then the third. Accordingly, `gl(I,K,length(y))` repeats each $a$ level for the ten replicates and cycles over its two levels, while `gl(J,K*I,length(y))` repeats each $b$ level for twenty observations. These factors align with the vectorized response.

The first fit is the additive [Analysis of variance](../../../../../analysis-of-variance.md) model $Y_{kij}=\mu+\alpha_i+\beta_j+\varepsilon_{kij}$, with independent normal errors of common [variance](../../../../../variance-split.md) $\sigma^2$. Under the default treatment constraints $\alpha_1=\beta_1=0$, the four fitted coefficients estimate the baseline cell mean, the $a=2$ minus $a=1$ effect, and the $b=2,3$ contrasts with $b=1$. Thus the baseline fitted mean is $3.7673$, the second $a$ level adds $3.4542$, and the second and third $b$ levels add $-6.3215$ and $-5.8268$.

The summary $t$ tests compare each indicated coefficient with zero, using its [standard error](../../../../../standard-error.md) and residual [variance](../../../../../variance-split.md) estimate $77.20/56$. They have 56 residual [degrees of freedom](../../../../../degree-of-freedom.md). The three non-intercept contrasts are strongly significant; the intercept test asks whether the baseline mean is zero, not whether either factor matters overall. The [Analysis of variance](../../../../../analysis-of-variance.md) tests are joint nested-model $F$ tests: no $a$ main effect, with one numerator degree of freedom, and no $b$ main effect, with two. Their sequential sums of squares are $178.98$ and $494.39$. In this balanced design the main-effect subspaces are orthogonal, so ordering $a,b$ does not change those sums of squares. The denominator is the same residual mean square $77.20/56$; both factor effects are highly significant.

The second fit expands `a*b` to `a+b+a:b`, adding two [interaction](../../../../../interaction-statistics.md) coefficients. It allows the $a$ effect to differ between $b$ levels and has six parameters, equivalently one mean per cell, with 54 residual [degrees of freedom](../../../../../degree-of-freedom.md). The [interaction](../../../../../interaction-statistics.md) adds only about $0.27$ to explained sum of squares; its $F$ statistic is $0.0963$ with [degrees of freedom](../../../../../degree-of-freedom.md) $(2,54)$ and $p=0.9084$. There is no evidence against additivity, so the simpler first model is preferable on these data. This does not prove the true [interaction](../../../../../interaction-statistics.md) is exactly zero.

For the final expression, $p=6$, $p_0=4$, and $n=60$. The fitted vectors are orthogonal projections onto nested model spaces, so $\|P Y-P_0Y\|^2$ is the additional sum of squares due to [interaction](../../../../../interaction-statistics.md). The final code computes

$$
\boxed{F=\frac{\|PY-P_0Y\|^2/2}{\|y-PY\|^2/54}=0.0963\ \text{approximately},}
$$

the same [interaction](../../../../../interaction-statistics.md) test as the [Analysis of variance](../../../../../analysis-of-variance.md) row. The exact value uses the original, unrounded observations and fits. Using only the displayed rounded sums $0.27$ and $76.93$ gives about $0.0948$ instead; that discrepancy is rounding, not a different test. The omitted observations prevent reconstructing more digits from the printed data alone.

## ↑ Ancestors (10)

1. [13J](../13j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
