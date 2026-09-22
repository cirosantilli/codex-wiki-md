<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There are two distinct identifiability issues. Without centering, constants can move between the [regression intercept](../../../../../../regression-intercept.md) and the additive components. After centering, the decomposition still fails to be unique if there are nonzero allowed centered perturbations $h_j$ satisfying

$$
\sum_jh_j(x_{ij})=0\quad\text{for every }i.
$$

Then replacing $f_j$ by $f_j+h_j$ leaves every fitted response unchanged. This nonlinear analogue of [multicollinearity](../../../../../../multicollinearity.md) is [concurvity](../../../../../../concurvity.md). For example, if two predictor columns are identical, a centered function $h$ can be added to the effect of the first and subtracted from the effect of the second. Conceptually, the data observe their combined effect but cannot tell which predictor deserves the credit. A unique fitted sum can therefore coexist with nonunique individual effects. Smoothness penalties can distinguish some such decompositions, so a representation ambiguity is not automatically an ambiguity of every penalized estimator.

For a precise criterion for the [backfitting algorithm](../../../../../../backfitting-algorithm.md) with [linear smoothers](../../../../../../linear-smoother.md), put $C=I-\mathbf1\mathbf1^T/n$, $y_c=Cy$, and $T_j=CS_jC$. On the centered component space its fixed-point equations are the [linear backfitting equations](../../../../../../linear-backfitting-equations.md)

$$
f_j+T_j\sum_{k\ne j}f_k=T_jy_c,\qquad j=1,\ldots,p.
$$

A consistent system has more than one solution exactly when there is a nonzero centered tuple satisfying $h_j+T_j\sum_{k\ne j}h_k=0$ for all $j$. In the two-component case, elimination gives

$$
(I-T_1T_2)f_1=T_1(I-T_2)y_c.
$$

Thus

$$
\boxed{\text{For a consistent two-component linear backfit, nonuniqueness occurs iff }1\text{ is an eigenvalue of }T_1T_2.}
$$

A common centered direction $h$ reproduced exactly by both smoothers, $T_1h=T_2h=h$, gives the homogeneous perturbation $(h,-h)$ and is a concrete instance. For example, two identical predictor columns with smoothers that reproduce the same centered linear trend have this property. Approximate [concurvity](../../../../../../concurvity.md) yields an eigenvalue near one, causing poor conditioning and slow or unstable component estimation, but it does not constitute exact nonuniqueness. Failure of an iteration to converge is also distinct from the existence of multiple fixed points.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
