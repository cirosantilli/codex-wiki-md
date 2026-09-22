<h1 id="1/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Put $N=n_0+n_1+n_2$ and $s=2x=2\theta(1-\theta)$. The usual [recombination fraction](../../../../../../recombination-fraction.md) range $0\le\theta\le1/2$ gives $0\le s\le1/2$, and the preceding [likelihood function](../../../../../../likelihood-function.md) becomes

$$
\boxed{\mathcal L(s)\propto s^{\,2n_0+n_1}(1-s)^{\,2n_2+n_1}.}
$$

To see its relation to [nonparametric linkage analysis](../../../../../../nonparametric-linkage-analysis.md), use [Bayes' theorem](../../../../../../bayes-theorem.md) and the constant disease [probability](../../../../../../probability.md) $1/16$ to obtain the affected-pair marker-sharing [probabilities](../../../../../../probability.md)

$$
(z_0,z_1,z_2)=\left(\frac{L_0/4}{1/16},\frac{L_1/2}{1/16},\frac{L_2/4}{1/16}\right)=\bigl(s^2,\,2s(1-s),\,(1-s)^2\bigr).
$$

Their [multinomial likelihood](../../../../../../multinomial-likelihood.md) has exactly the same $s$-dependent kernel, since its extra factor $2^{n_1}$ is constant. Set $A=2n_0+n_1$ and $B=2n_2+n_1$. Then $A+B=2N$, and $B$ is the total number of shared ancestral copies. At fixed $N$, the [Fisher-Neyman factorization theorem](../../../../../../fisher-neyman-factorization-theorem.md) makes $B$ a [sufficient statistic](../../../../../../sufficient-statistic.md). The observed [mean](../../../../../../expected-value.md) shared proportion is $\widehat p=B/(2N)$, and the [binomial likelihood](../../../../../../binomial-likelihood.md) kernel gives

$$
\boxed{\widehat s=\min\!\left(\frac A{2N},\frac12\right),\qquad \widehat\theta=\frac{1-\sqrt{1-2\widehat s}}2.}
$$

The unlinked null is $s=1/2$, whereas linkage corresponds to $s<1/2$, or expected shared proportion $1-s>1/2$. If $\widehat p\le1/2$, the constrained [likelihood](../../../../../../likelihood-function.md) is maximized at the unlinked null. For $\widehat p>1/2$, its log [likelihood](../../../../../../likelihood-function.md) ratio is

$$
2N\left\{\widehat p\log(2\widehat p)+(1-\widehat p)\log\bigl(2(1-\widehat p)\bigr)\right\},
$$

whose derivative in $\widehat p$ is $2N\log[\widehat p/(1-\widehat p)]>0$. Hence it orders samples exactly by excess [IBD](../../../../../../identity-by-descent.md) sharing. **Under this fully penetrant recessive model, parametric linkage testing and a one-sided test of the overall IBD-sharing proportion use the same information.** This is [allele-sharing sufficiency for recessive linkage](../../../../../../allele-sharing-sufficiency-for-recessive-linkage.md), not a general equivalence for all disease models. Use limiting values for terms such as $0\log0$, and assume $N>0$ for the estimators.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [1](../../1.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
