<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $0\le t\le\theta$, independence and the [uniform distribution](../../../../../../continuous-uniform-distribution.md) give $P(X_{(n)}\le t)=(t/\theta)^n$. Consequently, for fixed $x\ge0$ and $n>x$,

$$
P\!\left(\frac{n(\theta-X_{(n)})}{\theta}>x\right)=P\{X_{(n)}<\theta(1-x/n)\}=(1-x/n)^n\longrightarrow e^{-x}.
$$

For $x<0$ the survival probability is one. Thus **the scaled endpoint gap converges in distribution to a unit-rate exponential law**; it is not exactly exponential at finite $n$.

The [plug-in estimator](../../../../../../plug-in-estimator.md) principle replaces the unknown sampling distribution by its [empirical distribution](../../../../../../type-information-theory.md) and evaluates its population functional at that fitted distribution. Here the fitted support endpoint is $\widehat\theta=X_{(n)}$, also the [maximum-likelihood estimate](../../../../../../maximum-likelihood-estimator.md): the [likelihood](../../../../../../likelihood-function.md) is $\theta^{-n}\mathbf1_{\{\theta\ge X_{(n)}\}}$ and decreases over its allowed support. For an empirical [bootstrap sample](../../../../../../bootstrap-sample.md) $Y_1,\ldots,Y_n$, the corresponding gap is

$$
\boxed{G^*=\frac{n(X_{(n)}-Y_{(n)})}{X_{(n)}}.}
$$

Almost surely the original maximum is unique. The bootstrap gap equals zero precisely when this observation is selected at least once, so

$$
\boxed{P_*(G^*=0)=1-(1-1/n)^n\longrightarrow1-e^{-1}.}
$$

The true limiting [exponential distribution](../../../../../../exponential-distribution.md) has no atom at zero. This nonvanishing discrepancy proves [bootstrap failure for a uniform endpoint](../../../../../../bootstrap-failure-for-a-uniform-endpoint.md): the bootstrap distribution cannot converge to the correct limit, even though the endpoint estimate itself is consistent. It fails to recreate the unsampled population tail beyond the observed maximum. A [parametric bootstrap](../../../../../../parametric-bootstrap.md) drawing from $U[0,X_{(n)}]$, rather than from the discrete empirical sample, reproduces the scaled-gap law here.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
