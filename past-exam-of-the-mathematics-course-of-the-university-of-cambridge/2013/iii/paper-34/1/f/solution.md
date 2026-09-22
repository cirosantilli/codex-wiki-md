<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [Type II maximum likelihood estimator](../../../../../../maximum-marginal-likelihood-estimator.md) maximizes the [Bayesian model evidence](../../../../../../bayesian-model-evidence.md) after integrating out the breed parameters:

$$
\widehat\alpha=\arg\max_{\alpha>0}
p(\mathbf y_1,\ldots,\mathbf y_I\mid\alpha,\beta).
$$

For positive sample sizes define $S=\sum_i\log(m_i/\beta)\ge0$. Up to an additive constant, the [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\alpha)=I\log\alpha-\sum_i\log(\alpha+n_i)-\alpha S.
$$

Differentiation gives the interior score equation

$$
\boxed{\frac I{\widehat\alpha}
-\sum_i\frac1{\widehat\alpha+n_i}
=\sum_i\log\max(1,M_i/\beta).}
$$

Also $\ell''(\alpha)=-I/\alpha^2+\sum_i(\alpha+n_i)^{-2}<0$. If $S>0$, the derivative decreases from infinity to $-S$, so a unique finite maximum exists. When all sample sizes equal $n$, the equation becomes $In/[\alpha(\alpha+n)]=S$, giving

$$
\boxed{S\widehat\alpha^2+Sn\widehat\alpha-In=0,\qquad
\widehat\alpha=\frac{\sqrt{n^2+4In/S}-n}{2}\quad(S>0).}
$$

For $S=0$ no finite maximum exists. Plugging this [hyperparameter](../../../../../../hyperparameter.md) estimate into the breed [posterior distributions](../../../../../../bayesian-posterior.md) is an [Empirical Bayes method](../../../../../../empirical-bayes-method.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
