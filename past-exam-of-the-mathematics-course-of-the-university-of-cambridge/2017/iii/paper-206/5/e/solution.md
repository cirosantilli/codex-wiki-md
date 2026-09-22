<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $\mathcal F_t$ contain observations through time $t$. In the Gaussian [moving-average process of order one](../../../../../../moving-average-process-of-order-one.md), the innovations in

$$
Y_{t+7}=\mu+\varepsilon_{t+7}+\theta\varepsilon_{t+6}
$$

are independent of $\mathcal F_t$. Hence the [conditional expectation](../../../../../../conditional-expectation.md) is the constant mean. For known parameters, the forecast and its [mean squared prediction error](../../../../../../mean-squared-prediction-error.md) are

$$
\boxed{\widehat Y_{t+7\mid t}=\mu,\qquad \operatorname{MSPE}=\sigma_\varepsilon^2(1+\theta^2).}
$$

The mean prediction error itself is zero; the requested uncertainty is naturally interpreted as expected squared error. Plugging in the fit gives forecast $15.0133$, mean squared error $6.731002$, and root mean squared error about $2.5944$.

The usual [naive time-series forecast](../../../../../../naive-time-series-forecast.md) repeats $Y_t$. Its unconditional expected squared error is

$$
\mathbb E(Y_{t+7}-Y_t)^2=2\gamma(0)-2\gamma(7)=2\sigma_\varepsilon^2(1+\theta^2),
$$

since $\gamma(7)=0$. Thus

$$
\boxed{\operatorname{MSPE}_{\rm naive}\simeq13.462004,\qquad \operatorname{MSPE}_{\rm model}\simeq6.731002.}
$$

Conditional on $\mathcal F_t$, the naive error is $\gamma(0)+(Y_t-\mu)^2$, explaining directly why the conditional-mean forecast is better under [squared-error loss](../../../../../../squared-error-loss.md). These are fitted-model calculations that ignore parameter-estimation uncertainty. Estimating the unknown mean from the past adds its estimation mean squared error to the seven-step forecast risk; the printed summary does not provide a complete assessment of that extra uncertainty. This is distinct from claiming a signed mean error as a measure of forecasting accuracy.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
