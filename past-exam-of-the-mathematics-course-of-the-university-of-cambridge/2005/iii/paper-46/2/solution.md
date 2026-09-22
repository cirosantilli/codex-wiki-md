<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the sample, put $\bar x=n^{-1}\sum_ix_i$ and use the [sample covariance matrix](../../../../../sample-covariance-matrix.md)

$$
S=\frac1{n-1}\sum_{i=1}^{n}(x_i-\bar x)(x_i-\bar x)^T.
$$

Order its [eigenvalues](../../../../../eigenvalue.md) $\widehat\lambda_j$ decreasingly and choose unit orthogonal [eigenvectors](../../../../../eigenvector.md) $\widehat\ell_j$. The [sample principal components](../../../../../sample-principal-component.md) are the score columns

$$
\boxed{z_{ij}=\widehat\ell_j^T(x_i-\bar x).}
$$

Their [sample means](../../../../../sample-mean.md) are zero and their sample [covariance](../../../../../covariance.md) is diagonal, since $\widehat\ell_j^TS\widehat\ell_k=\widehat\lambda_j\mathbf1_{\{j=k\}}$. The $j$th [sample variance](../../../../../sample-variance.md) is $\widehat\lambda_j$, and its [explained variance of a principal component](../../../../../explained-variance-of-a-principal-component.md) is $\widehat\lambda_j/\operatorname{tr}(S)$. Using divisor $n$ instead changes the numerical [variances](../../../../../variance-split.md) by a common factor but leaves the component directions unchanged.

Standardizing means replacing a variable with positive [sample variance](../../../../../sample-variance.md) by $(x_{ij}-\bar x_j)/s_j$. This gives [principal component analysis on a correlation matrix](../../../../../principal-component-analysis-on-a-correlation-matrix.md), using $C=D^{-1/2}SD^{-1/2}$ with $D=\operatorname{diag}(S)$. It removes arbitrary differences of measurement units and prevents a large-variance coordinate from dominating solely through its scale. It also changes the question being optimized: small-variance and possibly noisy coordinates receive equal marginal weight. [Principal component analysis](../../../../../principal-component-analysis.md) based on the [covariance matrix](../../../../../covariance-matrix.md) can be more appropriate when the variables have common meaningful units and absolute variability matters. Standardization is therefore a substantive choice, not an automatic improvement. A zero-variance variable must first be removed. In the word-rating example the variables share the same numerical range, but their across-word dispersions can differ; standardization gives each attribute equal initial [variance](../../../../../variance-split.md).

For the standardized eight-variable analysis, total [variance](../../../../../variance-split.md) is $\operatorname{tr}(C)=8$. The first three fractions of [explained variance of a principal component](../../../../../explained-variance-of-a-principal-component.md) are approximately **59.6%, 19.1% and 10.1%**, respectively. The first two account for about **78.8%**, and the first three for **88.9%**. The first direction is dominant but one direction alone loses substantial variation. Retaining two [principal components](../../../../../principal-component.md) is a plausible descriptive summary: their [eigenvalues](../../../../../eigenvalue.md) exceed $1$, whereas the third is below $1$. That cutoff is a heuristic, and the third [principal component](../../../../../principal-component.md) may still have interpretable content.

The reported coefficient rows are not unit-length vectors. The printed rounded rows have squared lengths $4.7514$, $1.5222$ and $0.8063$, consistent with their [eigenvalues](../../../../../eigenvalue.md) to the precision of the coefficient table. They are consistent with the scaled [principal component loading](../../../../../principal-component-loading.md) convention $r_j=\sqrt{\lambda_j}\ell_j$. Such rows remain [eigenvectors](../../../../../eigenvector.md), but the score direction with unit length is $\ell_j=r_j/\sqrt{\lambda_j}$, or more accurately the row divided by its actual [Euclidean norm](../../../../../euclidean-norm.md) when using rounded entries. Under this convention $r_{ij}$ is the [correlation](../../../../../pearson-correlation-coefficient.md) of standardized attribute $i$ with the variance-one score for component $j$:

$$
\operatorname{Corr}(Z_i,\ell_j^TZ/\sqrt{\lambda_j})=\sqrt{\lambda_j}\ell_{ij}.
$$

This explains both their sizes and why they must not be treated as the [unit vectors](../../../../../unit-vector.md) from parts (i) and (ii).

The first [principal component](../../../../../principal-component.md) has positive coefficients on every attribute, strongest on friendliness, goodness, niceness, bravery and strength. With the favorable endpoints coded in the positive direction, it describes a broad favorable or impressive evaluation, with a potency contribution. The second contrasts movement and speed, with some size and strength, against the first three evaluative attributes; it is chiefly an activity dimension. The third is dominated by size, with smaller positive strength and negative movement/speed coefficients, distinguishing size or potency from activity. These are interpretations of directions of variation, not evidence of causal latent traits. Reversing a [principal component](../../../../../principal-component.md)'s overall sign changes neither its meaning as an axis nor its explained [variance](../../../../../variance-split.md); endpoint coding fixes only how its positive side is described.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
