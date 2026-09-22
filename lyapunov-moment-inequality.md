# Lyapunov moment inequality

↑ **Parent:** [Probability inequality](probability-inequality-split.md)

The Lyapunov moment inequality says that higher positive [absolute moments](absolute-moment.md) give no smaller [absolute moment](absolute-moment.md) sizes on a [probability space](probability-space-split.md). For a real [random variable](random-variable-split.md) $Z$ and $0<r<s$,

$$
\boxed{\left(\mathbb E|Z|^r\right)^{1/r}\leq\left(\mathbb E|Z|^s\right)^{1/s},}
$$

allowing an infinite value. For $r\geq1$ the left expression is an [Lp norm](lp-norm.md); below one it is a [quasi-norm](quasi-norm.md), so the usual [triangle inequality](triangle-inequality.md) terminology needs that distinction. The comparison uses a [probability measure](probability-measure.md) of total mass one; arbitrary unnormalized [measure spaces](measure-space.md) need a factor depending on their total mass.

For a nonnegative count, the first moment size is its [expected value](expected-value-split.md), while the second is the [square root](square-root.md) of its [second moment](second-moment.md). Both ten-trial counts in [second moment method](second-moment-method.md) have first moment size one. The [independent](independent-random-variables.md) count has second moment size $\sqrt{1.9}\approx1.37840$, whereas the shared-outcome count $N=10B$ has second moment size $\sqrt{10}\approx3.16228$. The second moment distinguishes models with the same average because its square increases the influence of rare large counts.

More generally, for $N=10B$ with a [Bernoulli random variable](bernoulli-distribution.md) $B$ of parameter $1/10$,

$$
\left(\mathbb E N^r\right)^{1/r}=10(1/10)^{1/r}.
$$

It rises from one at $r=1$ toward ten as $r\to\infty$. Replacing $1/10$ by a parameter $0<q\leq1$ gives $10q^{1/r}$, which decreases toward zero for a fixed positive [exponent](exponent.md) when $q\downarrow0$, making the rare-event and large-exponent limits different questions. For a scaled [Rademacher random variable](rademacher-distribution.md) taking values $-2$ and two with equal [probabilities](probability.md), every absolute moment size is exactly two: increasing the [exponent](exponent.md) does not distinguish signs when the [absolute value](absolute-value.md) is constant.

<a id="image-lyapunov-moment-inequality-reveals-how-higher-moments-emphasize-large-outcomes-and-when-equality-holds"></a>
![](lyapunov-moment-sizes-for-rare-counts.png)

**[Figure 1](#image-lyapunov-moment-inequality-reveals-how-higher-moments-emphasize-large-outcomes-and-when-equality-holds). Lyapunov moment inequality reveals how higher moments emphasize large outcomes and when equality holds**. Left: the two original ten-trial models from [second moment method](second-moment-method.md) have the same [mean](expected-value-split.md) one, but different [absolute moment](absolute-moment.md) sizes at [exponents](exponent.md) above one. The shared model has $N=10B$ with $p=1/10$. Right: equal masses at $-2$ and two keep $|Z|=2$ [almost surely](almost-sure-convergence.md), giving equality for every pair of positive [exponents](exponent.md). These are fully specified mathematical probability models.

For finite $\mathbb E|Z|^s$, apply the reversed [Jensen's inequality](jensen-s-inequality.md) to the [strictly concave function](strictly-concave-function.md) $t^{r/s}$ and the nonnegative [random variable](random-variable-split.md) $|Z|^s$:

$$
\mathbb E|Z|^r\leq\left(\mathbb E|Z|^s\right)^{r/s}.
$$

Taking the positive $r$th root proves the claim. Equality in this finite case holds exactly when $|Z|$ is constant [almost surely](almost-sure-convergence.md). If the higher [moment](moment.md) is infinite, the upper bound is infinite and remains valid. Exponent zero is excluded from the statement; logarithmic or geometric limiting summaries require separately stated conventions, especially when $Z$ can vanish.

## ↑ Ancestors (6)

1. [Probability inequality](probability-inequality-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Lyapunov moment inequality](lyapunov-moment-inequality.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204/2/d/solution.md)
