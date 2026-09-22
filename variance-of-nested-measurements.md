# Variance of nested measurements

↑ **Parent:** [Nested measurements](nested-measurements.md)

For $n$ pots per [treatment](treatment.md) and $m$ [leaves](leaf.md) per pot, the group [sample mean](sample-mean.md) decomposes into two averages:

$$
\overline Y_g=\frac1{nm}\sum_{i=1}^n\sum_{j=1}^mY_{gij}
=\mu+\alpha_g+\frac1n\sum_{i=1}^nU_{gi}
+\frac1{nm}\sum_{i=1}^n\sum_{j=1}^m\varepsilon_{gij}.
$$

The [variance of a sum](variance-of-a-sum.md) adds the [variances](variance-split.md) of the [independent](independent-random-variables.md) terms. Every pot [random effect](random-effect.md) has weight $1/n$, whereas each remaining error has weight $1/(nm)$, giving the short proof

$$
\operatorname{Var}(\overline Y_g)
=n\frac{\tau^2}{n^2}+nm\frac{\sigma^2}{n^2m^2}
=\frac{\tau^2}{n}+\frac{\sigma^2}{nm}.
$$

This is also the [variance](variance-split.md) of the [arithmetic mean](arithmetic-mean.md) of the $n$ pot [sample means](sample-mean.md), each with [variance](variance-split.md) $\tau^2+\sigma^2/m$. Equal numbers of [leaves](leaf.md) per pot make the two averaging procedures identical.

If all $nm$ [leaf](leaf.md) measurements were falsely treated as [independent](independent-random-variables.md), the predicted [variance](variance-split.md) would instead be $(\tau^2+\sigma^2)/(nm)$. The ratio of correct to false [variance](variance-split.md) is

$$
\frac{m\tau^2+\sigma^2}{\tau^2+\sigma^2}
=1+(m-1)\rho.
$$

Thus [pseudoreplication](pseudoreplication.md) can underestimate a [standard error](standard-error.md) by the square root of this ratio. Equality holds when $m=1$ or $\tau^2=0$; sharing a pot creates an error here precisely when the shared influence has positive [variance](variance-split.md).

Choose $\tau^2=4$, $\sigma^2=1$, $n=4$ and $m=3$ as constructed model parameters in squared [length](length.md) units. These are assumptions rather than fitted experimental values. For each group,

$$
\operatorname{Var}(\overline Y_g)=\frac44+\frac1{12}=\frac{13}{12},
\qquad
\operatorname{Var}_{\mathrm{false}}(\overline Y_g)=\frac5{12},
\qquad \rho=\frac45.
$$

The [treatment contrast](treatment-contrast.md) $\widehat\Delta=\overline Y_B-\overline Y_A$ has [expected value](expected-value-split.md) $\alpha_B-\alpha_A$. Since the group errors are [independent](independent-random-variables.md) conditional on the allocation, its [variance](variance-split.md) is twice the group [variance](variance-split.md), namely $13/6$, whereas the false calculation gives $5/6$. Its correct [standard error](standard-error.md) is $\sqrt{13/6}\approx1.472$ [length](length.md) units; the false value is $\sqrt{5/6}\approx0.913$. The [variance](variance-split.md) ratio is $13/5=2.6$.

<a id="image-constructed-variance-predictions-adding-pots-reduces-uncertainty-faster-than-adding-leaf-measurements-within-four-pots"></a>
![](experimental-replication-variance-budget.png)

**[Figure 2](#image-constructed-variance-predictions-adding-pots-reduces-uncertainty-faster-than-adding-leaf-measurements-within-four-pots). Constructed variance predictions: adding pots reduces uncertainty faster than adding leaf measurements within four pots**. Each curve uses $\tau^2=4$ and $\sigma^2=1$; the horizontal axis counts measurements per [treatment](treatment.md). The solid designs agree at four pots with three [leaves](leaf.md) each. The dashed curve assumes all measurements are [independent](independent-random-variables.md) and therefore illustrates [pseudoreplication](pseudoreplication.md); none of the curves are observed experimental data.

With four pots fixed, increasing $m$ drives the error contribution $\sigma^2/(4m)$ towards zero, but the [limit](limit-of-a-function.md) of the group [variance](variance-split.md) remains $\tau^2/4=1$. Measuring twelve [leaves](leaf.md) on each of four pots gives $49/48$. Using the same forty-eight measurements on sixteen pots, with three [leaves](leaf.md) per pot, gives $13/48$. More independent [experimental units](experimental-unit.md) reduce both contributions. Extra [nested measurements](nested-measurements.md) are useful for characterizing each [experimental unit](experimental-unit.md), but cannot average away its shared [random effect](random-effect.md). This is why sample collection effort and the number of independent [treatment](treatment.md) [replicates](replicate.md) answer different questions.[Pseudoreplication and the Design of Ecological Field Experiments, p. 201, “Multiple samples per experimental unit”](pseudoreplication-and-the-design-of-ecological-field-experiments-by-stuart-h-hurlbert.md)

## ↑ Ancestors (9)

1. [Nested measurements](nested-measurements.md)
2. [Replication in experimental design](replication-in-experimental-design.md)
3. [Design of experiments](design-of-experiments-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Pseudoreplication](pseudoreplication.md)
