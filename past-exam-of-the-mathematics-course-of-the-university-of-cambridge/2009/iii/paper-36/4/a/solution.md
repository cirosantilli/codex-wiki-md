<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Compute the [Bayesian model evidence](../../../../../../bayesian-model-evidence.md) for each model by integrating its sampling density against its parameter prior:

$$
m_i(y)=\int p_Y(y\mid\psi_i,M_i)p(\psi_i\mid M_i)\,d\psi_i.
$$

The [posterior odds](../../../../../../posterior-odds.md) are the [prior odds](../../../../../../prior-odds.md) multiplied by the [Bayes factor](../../../../../../bayes-factor.md):

$$
\boxed{\frac{\Pr(M_1\mid y)}{\Pr(M_2\mid y)}
=\frac{\Pr(M_1)}{\Pr(M_2)}\frac{m_1(y)}{m_2(y)}.}
$$

The parameter priors used for evidence must be normalized; arbitrary normalization constants in model-specific improper priors would make this comparison undefined.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
