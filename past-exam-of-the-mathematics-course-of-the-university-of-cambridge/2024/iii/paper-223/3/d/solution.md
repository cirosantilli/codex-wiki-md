<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $P_0=N(-\theta_0,1)$ and $P_1=N(\theta_0,1)$, the nominal log-likelihood ratio for one observation is $2\theta_0x$. Under sufficiently small [epsilon-contamination neighborhoods](../../../../../../epsilon-contamination-neighborhood.md), the least-favourable pair clips this likelihood ratio between two constants. Symmetry turns its log into a positive multiple of the winsorized score

$$
q_c(x)=\operatorname{clip}(x,-c,c).
$$

The robust form of the [Neyman-Pearson lemma](../../../../../../neyman-pearson-lemma.md) therefore rejects for large values of

$$
\sum_{i=1}^nq_c(X_i),
$$

with boundary randomization and threshold chosen so that the worst-case null rejection probability is $\alpha$. Extreme observations contribute only $\pm c$, preventing a few contaminants from dominating the test.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
