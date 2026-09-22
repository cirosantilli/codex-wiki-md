<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

If the change is purely a rescaling of the physics mark, write $X'=DX$, where $D=\operatorname{diag}(10/3,1,1,1)$. The [sample covariance matrix](../../../../../../../sample-covariance-matrix.md) transforms as

$$
\Sigma'=D\Sigma D.
$$

The physics [variance](../../../../../../../variance-split.md) is multiplied by $100/9$, becoming approximately $10044.44$. Each covariance between physics and another subject is multiplied by $10/3$, and all other entries stay unchanged. [Principal component analysis](../../../../../../../principal-component-analysis.md) on this new [sample covariance matrix](../../../../../../../sample-covariance-matrix.md) maximizes [variance](../../../../../../../variance-split.md) in the new numerical units, so its [eigenvectors](../../../../../../../eigenvector.md) and [explained variance of a principal component](../../../../../../../explained-variance-of-a-principal-component.md) generally change. Physics receives disproportionately greater influence simply because its unit has changed.

One solution is to convert the physics marks back to the original scale before doing [principal component analysis](../../../../../../../principal-component-analysis.md). Alternatively, use [principal component analysis on a correlation matrix](../../../../../../../principal-component-analysis-on-a-correlation-matrix.md): standardize every subject by

$$
Z_j=\frac{X_j-\bar X_j}{s_j},\qquad R_{jk}=\frac{\Sigma_{jk}}{s_js_k},\qquad s_j=\sqrt{\Sigma_{jj}}.
$$

A positive change of units multiplies both a centered variable and its standard deviation by the same factor. Thus it leaves $Z_j$ and the [sample correlation matrix](../../../../../../../sample-correlation-matrix.md) $R$ unchanged.

**Correlation-based principal component analysis is invariant under positive changes of units; covariance-based principal component analysis is not.** Standardizing gives each subject unit [variance](../../../../../../../variance-split.md), which is a different weighting choice and can emphasize relatively low-variance subjects. If the revised assessment changes the scores themselves rather than just their units, its [sample correlation matrix](../../../../../../../sample-correlation-matrix.md) may also change, and mere standardization cannot recover the original analysis.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 46](../../../../paper-46-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
