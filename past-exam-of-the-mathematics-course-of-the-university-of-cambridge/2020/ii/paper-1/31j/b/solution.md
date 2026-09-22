<h1 id="31j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $z=(x,y)$ define the [misclassification loss](../../../../../../misclassification-loss.md)

$$
f_h(z)=\mathbf1_{\{h(x)\ne y\}},
$$

and take the [loss class](../../../../../../loss-class.md)

$$
\boxed{\mathcal F=\{f_h:h\in\mathcal H\}.}
$$

Write $Pf=\mathbb Ef(Z)$ and $P_nf=n^{-1}\sum_{i=1}^nf(Z_i)$, so the [misclassification risk](../../../../../../misclassification-risk.md) and [empirical misclassification risk](../../../../../../empirical-misclassification-risk.md) are $R(h)=Pf_h$ and $\widehat R(h)=P_nf_h$.

Because $\widehat h$ is an [empirical risk minimizer](../../../../../../empirical-risk-minimization.md), $P_n(f_{\widehat h}-f_{h^*})\leq0$. Hence its [excess risk](../../../../../../excess-risk.md) obeys

$$
R(\widehat h)-R(h^*)
\leq G(Z_{1:n}),
\qquad
G(Z_{1:n})
=\sup_{h\in\mathcal H}(P-P_n)(f_h-f_{h^*}).
$$

Introduce an independent ghost sample and perform [Rademacher symmetrization](../../../../../../rademacher-symmetrization-inequality.md). The contribution involving the fixed function $f_{h^*}$ has zero expectation over the [Rademacher signs](../../../../../../rademacher-distribution.md), so each of the two independent sample terms has supremum expectation $\mathcal R_n(\mathcal F)$. Therefore

$$
\mathbb EG\leq2\mathcal R_n(\mathcal F).
$$

Every difference $f_h-f_{h^*}$ takes values in $[-1,1]$. Replacing one observation can consequently change $G$ by at most $2/n$. Applying the [Bounded differences inequality](../../../../../../mcdiarmid-s-inequality.md) with $c_i=2/n$ gives, except on an event of [probability](../../../../../../probability-theory-split.md) at most $\delta/2$,

$$
G\leq\mathbb EG+\sqrt{\frac{2\log(2/\delta)}n}.
$$

Combining these inequalities proves, with [probability](../../../../../../probability-theory-split.md) at least $1-\delta$,

$$
\boxed{
R(\widehat h)-R(h^*)
\leq2\mathcal R_n(\mathcal F)
+\sqrt{\frac{2\log(2/\delta)}n}.
}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [31J](../../31j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
