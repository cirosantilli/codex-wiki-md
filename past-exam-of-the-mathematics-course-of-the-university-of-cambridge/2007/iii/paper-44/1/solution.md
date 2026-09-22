<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A useful full statement is the [rank-sum form of Cochran's theorem](../../../../../rank-sum-form-of-cochran-s-theorem.md). Let $Z\sim N_n(0,I_n)$ and let $A_1,\ldots,A_k$ be real [symmetric matrices](../../../../../symmetric-matrix.md) satisfying $\sum_iA_i=I_n$. Put $r_i=\operatorname{rank}(A_i)$ and $Q_i=Z^TA_iZ$. Then $\sum_ir_i\geq n$, and the following conditions are equivalent: the ranks sum to $n$; the $A_i$ are [orthogonal projection matrices](../../../../../orthogonal-projection-matrix.md) with mutually orthogonal ranges; and the $Q_i$ are independent, with $Q_i\sim\chi^2_{r_i}$. A rank-zero form is identically zero. In particular, the usual projection version of [Cochran's theorem](../../../../../cochran-s-theorem.md) partitions the squared length of a standard normal vector into independent [chi-squared distributions](../../../../../chi-squared-distribution.md).

Here is a proof which also explains the rank condition. Let $L_i=\operatorname{im}A_i$. Since every vector satisfies $x=\sum_iA_ix$, the spaces $L_i$ span $\mathbb R^n$. Therefore their dimensions sum to at least $n$. If they sum to $n$, their sum is a [direct sum](../../../../../direct-sum.md), so every vector has a unique decomposition into vectors belonging to the $L_i$. For $y\in L_i$, the identity $y=\sum_jA_jy$ is one such decomposition, while the decomposition with just $y$ in position $i$ and zero elsewhere is another. Uniqueness gives $A_jy=\delta_{ij}y$. Thus

$$
A_i^2=A_i,\qquad A_iA_j=0\quad(i\ne j).
$$

A [symmetric matrix](../../../../../symmetric-matrix.md) with this idempotence is an [orthogonal projection matrix](../../../../../orthogonal-projection-matrix.md). Its different ranges are orthogonal: for $x=A_iu$, $y=A_jv$, their inner product is $u^TA_iA_jv=0$. Choose an [orthonormal basis](../../../../../orthonormal-basis.md) for each range and concatenate them. The resulting change-of-basis matrix is an [orthogonal matrix](../../../../../orthogonal-matrix.md). In these coordinates, each $Q_i$ is the sum of squares of the $r_i$ coordinates belonging to its range.

The transformed [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) still has density proportional to $\exp(-\|z\|^2/2)$, which factors into the standard normal densities of its coordinates. The coordinates are independent, so the disjoint groups of squared coordinates give independent [chi-squared distributions](../../../../../chi-squared-distribution.md) of the asserted degrees of freedom. This proves the forward implication. Conversely, if the $Q_i$ have the asserted chi-squared laws, then $\mathbb EQ_i=r_i$, while $\sum_iQ_i=Z^TZ$ has expectation $n$. Taking expectations yields $\sum_ir_i=n$. This completes the equivalence and the proof of [Cochran's theorem](../../../../../cochran-s-theorem.md).

For the application, specify a [normal linear model](../../../../../normal-linear-model.md)

$$
Y=X\beta+\varepsilon,\qquad\varepsilon\sim N_n(0,\sigma^2I_n),
$$

with fixed full-column-rank [design matrix](../../../../../design-matrix.md) $X$ of size $n\times p$, $p<n$, unrestricted $\beta\in\mathbb R^p$, and unknown $\sigma^2>0$. Test $H_0:R\beta=r$ against $H_1:R\beta\ne r$, where $R$ has $q$ independent rows, $1\leq q\leq p$, and $r$ is specified. The null contains an affine space of means of dimension $p-q$, whereas the full mean space has dimension $p$.

Let $\widehat\beta=(X^TX)^{-1}X^TY$ be the [ordinary least squares](../../../../../ordinary-least-squares.md) and [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) in the full model, and write $G=(X^TX)^{-1}$. The constrained estimate follows by minimizing the residual squared length under $R\beta=r$:

$$
\widetilde\beta=\widehat\beta-GR^T(RGR^T)^{-1}(R\widehat\beta-r).
$$

Indeed, $R\widetilde\beta=r$ and the correction is the required constrained projection in the $X^TX$ inner product. The [least-squares normal equations](../../../../../normal-equations-for-linear-least-squares.md) give the Pythagorean decomposition

$$
\|Y-X\beta\|^2=\|Y-X\widehat\beta\|^2+(\beta-\widehat\beta)^TX^TX(\beta-\widehat\beta).
$$

Consequently the explicit residual quantities in the [likelihood-ratio test statistic](../../../../../likelihood-ratio-test-statistic.md) are

$$
\boxed{B=\|Y-X\widehat\beta\|^2,\qquad A=(R\widehat\beta-r)^T\{R(X^TX)^{-1}R^T\}^{-1}(R\widehat\beta-r).}
$$

Here $B$ is the full-model [residual sum of squares](../../../../../residual-sum-of-squares.md), and $A=\|Y-X\widetilde\beta\|^2-B$ is the increase caused by imposing the null restrictions.

To see the geometry behind [Cochran's theorem](../../../../../cochran-s-theorem.md), choose any $\beta_0$ with $R\beta_0=r$, and let $P$ project onto $\operatorname{col}X$ and $P_0$ onto $X\ker R$. For $z=Y-X\beta_0$,

$$
A=z^T(P-P_0)z,\qquad B=z^T(I-P)z.
$$

The projectors $P-P_0$ and $I-P$ are orthogonal and have ranks $q$ and $n-p$. Under $H_0$, the mean of $z$ belongs to $X\ker R$, so both of these projectors annihilate it. Thus [Cochran's theorem](../../../../../cochran-s-theorem.md) gives

$$
\frac A{\sigma^2}\sim\chi_q^2,\qquad\frac B{\sigma^2}\sim\chi_{n-p}^2,\qquad A\text{ and }B\text{ independent}.
$$

The nuisance variance cancels in the [nested-model F-test](../../../../../nested-model-f-test.md) statistic

$$
F=\frac{A/q}{B/(n-p)}\sim F_{q,n-p}.
$$

Since the [likelihood-ratio test statistic](../../../../../likelihood-ratio-test-statistic.md) is

$$
w_{LR}=n\log\left(1+\frac AB\right)=n\log\left(1+\frac q{n-p}F\right),
$$

it is a strictly increasing function of $F$. Therefore **an exact level-$\alpha$ likelihood-ratio test rejects when $F>F_{q,n-p;1-\alpha}$**, where the right-hand side is the upper reference quantile of the [F-distribution](../../../../../f-distribution.md). This calibration is exact under the [normal linear model](../../../../../normal-linear-model.md), rather than an asymptotic chi-squared replacement.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
