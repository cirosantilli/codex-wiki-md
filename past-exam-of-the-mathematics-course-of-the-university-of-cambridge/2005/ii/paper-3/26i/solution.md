<h1 id="26i/solution">Solution</h1>

↑ **Parent:** [26I](../26i.md)

A [loss function](../../../../../loss-function.md) $L(\theta,a)$ measures the cost of taking action $a$ at parameter $\theta$. A [decision rule](../../../../../decision-rule.md) $\delta$ selects an action from the data; its [risk function](../../../../../risk-function.md) is $R(\theta,\delta)=E_\theta L(\theta,\delta(X))$. A [Bayes estimator](../../../../../bayes-estimator.md) minimizes the prior-averaged risk, or equivalently minimizes posterior expected loss at almost every observation. An admissible rule has no competing rule of no greater risk everywhere and strictly smaller risk somewhere. To construct a Bayes rule, form the posterior and minimize its expected loss over the allowed actions. Under squared error and finite posterior second moments the unique action is the posterior mean.

Put $S=|X|^2$. The given fourth moment and independence give $E_vS=nv$, $E_vS^2=n(n+2)v^2$. Thus

$$
R(v,\alpha S)=v^2[n(n+2)\alpha^2-2n\alpha+1]
=v^2\left[n(n+2)\left(\alpha-\frac1{n+2}\right)^2+\frac2{n+2}\right].
$$

Every $\alpha\ne1/(n+2)$ is strictly dominated at every $v>0$ by that coefficient. Hence **it cannot be a finite-risk Bayes rule for any proper prior**.

To make the second requested comparison, let $m_j=E_\pi v^j$ and assume finite quadratic [Bayes risk](../../../../../bayes-risk.md). For the affine rules the integrated risk is

$$
r(\alpha,\beta)=[n(n+2)\alpha^2-2n\alpha+1]m_2+2\beta(n\alpha-1)m_1+\beta^2.
$$

With $\alpha$ fixed, the minimum occurs at $\beta=(1-n\alpha)m_1$. Since $m_1>0$, this strictly improves the homogeneous rule unless $\alpha=1/n$, reducing risk by $(1-n\alpha)^2m_1^2$. Therefore **a homogeneous rule with $\alpha\ne1/n$ is not Bayes**, as requested. Combining the two restrictions excludes every homogeneous coefficient.

For a proper prior without global finite moments, the same nonvacuous conclusion follows from the posterior-mean condition. Let

$$
m(s)=\int_0^\infty v^{-n/2}e^{-s/(2v)}f_0(v)dv,\qquad
M_1(s)=\int_0^\infty v^{1-n/2}e^{-s/(2v)}f_0(v)dv.
$$

For $s>0$, $M_1'(s)=-m(s)/2$. If the posterior mean were $\alpha s$, positivity requires $\alpha>0$ and $M_1=\alpha s m$. Differentiation forces $m(s)=Cs^{-1-1/(2\alpha)}$. But the marginal density of $S$ would then be a constant times $s^{n/2-2-1/(2\alpha)}$, a pure power not integrable at both zero and infinity. This contradicts a proper prior's normalized predictive distribution. This is the [proper-prior obstruction to homogeneous variance Bayes rules](../../../../../proper-prior-obstruction-to-homogeneous-variance-bayes-rules.md).

The finite-loss qualification matters: allowing all posterior losses to equal infinity makes every action a vacuous minimizer. For example, with $n=1$ and proper density $f_0(v)=(1+v)^{-2}$, the posterior second moment diverges at positive observations, so a literal infinite-loss definition would defeat the printed assertion. Ordinary meaningful Bayes rules exclude that convention.

## ↑ Ancestors (10)

1. [26I](../26i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
