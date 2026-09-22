# Scalar static-state Kalman update

↑ **Parent:** [Kalman filter](kalman-filter.md)

Suppose the predicted state has [normal distribution](normal-distribution.md) $x\mid\mathcal F\sim N(\widehat x,V)$ and the new observation is $y=x+\eta$, where the [measurement noise](measurement-noise.md) $\eta\sim N(0,R)$ is [independent](independent-random-variables.md) of the state and previous observations. [Gaussian conditional expectation](gaussian-conditional-expectation.md) gives

$$
\mathbb E[x\mid\mathcal F,y]
=\widehat x+\frac{V}{V+R}(y-\widehat x),
\qquad
\operatorname{Var}(x\mid\mathcal F,y)
=\frac{VR}{V+R}.
$$

The coefficient $V/(V+R)$ is the scalar [Kalman gain](kalman-gain.md). The [posterior mean](posterior-mean.md) is a [weighted mean](weighted-arithmetic-mean.md) of the predicted state and the new observation, with the more precise quantity receiving more weight. For $V,R>0$, the same equations can be expressed in [precision parameters](precision-parameter.md)

$$
\frac1{P_{\mathrm{post}}}=\frac1V+\frac1R,\qquad
m_{\mathrm{post}}=P_{\mathrm{post}}\left(\frac{\widehat x}{V}+\frac{y}{R}\right).
$$

The two [precision parameters](precision-parameter.md) add because the [measurement noise](measurement-noise.md) is [independent](independent-random-variables.md) of the state and past observations. [Completing the square](completing-the-square.md) in the product of the [prior density](prior-density.md) and the [likelihood function](likelihood-function.md) gives this form directly. This is a [Gaussian conditional expectation](gaussian-conditional-expectation.md) for a fixed unknown state; a moving state additionally requires a [Kalman prediction step](kalman-prediction-step.md).

## ↑ Ancestors (6)

1. [Kalman filter](kalman-filter.md)
2. [State estimation](state-estimation.md)
3. [Control theory](control-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/30k/a/solution.md)
