<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The orchard residual [mean square in ANOVA](../../../../../../mean-square-in-anova.md) is on the original tree-response scale: it equals 30 times the corresponding residual [mean square in ANOVA](../../../../../../mean-square-in-anova.md) for orchard means. Thus the estimated [variance](../../../../../../variance-split.md) of one orchard's [sample mean](../../../../../../sample-mean.md) is $240/30=8$.

Each pruning marginal [sample mean](../../../../../../sample-mean.md) averages four independent orchard means, giving [variance](../../../../../../variance-split.md) $8/4=2$. Two different pruning marginals use disjoint orchards, so the [variance](../../../../../../variance-split.md) of their estimated [treatment contrast](../../../../../../treatment-contrast.md) is

$$
\boxed{\widehat{\operatorname{Var}}(\widehat\mu_{P_i}-\widehat\mu_{P_j})=2\frac{240}{30\cdot4}=4.}
$$

Each spray marginal [sample mean](../../../../../../sample-mean.md) uses six orchards. Similarly,

$$
\boxed{\widehat{\operatorname{Var}}(\widehat\mu_S-\widehat\mu_{\mathrm{no\ spray}})=2\frac{240}{30\cdot6}=\frac83.}
$$

The corresponding [standard errors](../../../../../../standard-error.md) are $2$ and $\sqrt{8/3}$ in the units of weight per tree. These compare per-tree marginal [sample means](../../../../../../sample-mean.md), averaging equally over the other factor, even when an [interaction term](../../../../../../interaction-term.md) is fitted. Comparing orchard totals instead would multiply these [variances](../../../../../../variance-split.md) by $30^2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
