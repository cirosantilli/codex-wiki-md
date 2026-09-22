# Delta method for Bernoulli odds

↑ **Parent:** [Delta method](delta-method.md)

For independent [Bernoulli random variables](bernoulli-distribution.md) of fixed success [probability](probability.md) $0<p<1$, put $\widehat p=n^{-1}\sum_iX_i$ and $o=p/(1-p)$. The [central limit theorem](central-limit-theorem.md) gives $\sqrt n(\widehat p-p)\xrightarrow dN(0,p(1-p))$. Applying the [delta method](delta-method.md) to the [odds](odds.md) map $g(p)=p/(1-p)$, whose [derivative](derivative.md) is $(1-p)^{-2}$, gives

$$
\sqrt n\left(\frac{\widehat p}{1-\widehat p}-\frac p{1-p}\right)\xrightarrow dN\!\left(0,\frac p{(1-p)^3}\right).
$$

The ratio is undefined on the all-success [event](event.md), whose [probability](probability.md) is $p^n$. Any finite extension there has the same limiting [probability distribution](probability-distribution-split.md), since that [probability](probability.md) tends to zero. This is an asymptotic statement and does not assert an exact finite-sample [variance](variance-split.md) of the unextended ratio. It is useful for uncertainty in estimated [odds](odds.md) when the success [probability](probability.md) stays away from one.

## ↑ Ancestors (7)

1. [Delta method](delta-method.md)
2. [Asymptotic normality](asymptotic-normality.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2017/1/a/iii/solution.md)
