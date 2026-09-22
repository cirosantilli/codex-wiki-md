# Gaussian filtering with exact observations

↑ **Parent:** [Kalman filter](kalman-filter.md)

In a linear [Gaussian](normal-distribution.md) [state-space model](state-space-model-time-series.md) with [process noise](process-noise.md) [covariance](covariance.md) $Q$ and exact scalar observation $X_t=FS_t$, the predictive state [covariance](covariance.md) includes $Q$ even though there is no separate [measurement noise](measurement-noise.md). Here $R_t=GP_{t-1}G^\top+Q$ denotes predicted state [covariance](covariance.md); it differs from the measurement-noise notation in the general [Kalman filter](kalman-filter.md) equations. The observation [innovation](innovation-process.md) [variance](variance-split.md) is $V_t=FGP_{t-1}G^\top F^\top+FQF^\top$. Omitting the second term incorrectly removes the current [process noise](process-noise.md). If $V_t>0$, [Gaussian conditional expectation](gaussian-conditional-expectation.md) gives the [posterior covariance matrix](posterior-covariance-matrix.md) $P_t=R_t-R_tF^\top FR_t/V_t$. This can be a [singular matrix](singular-matrix.md) because the observed [linear combination](linear-combination.md) is then known exactly.

For a concrete example with two state components that are [dimensionless quantities](dimensionless-quantity.md), take predicted mean $(10,0)^\top$, predicted [covariance matrix](covariance-matrix.md)

$$
R=\begin{pmatrix}4&2\\2&9\end{pmatrix},
$$

and exact observation of the first component, $F=(1,0)$, $X=12$. The [innovation](innovation-process.md) is $2$, its [variance](variance-split.md) is $4$, and the [Kalman gain](kalman-gain.md) is $(1,1/2)^\top$. The [posterior mean](posterior-mean.md) and [posterior covariance matrix](posterior-covariance-matrix.md) are therefore

$$
m=\begin{pmatrix}12\\1\end{pmatrix},\qquad
P=R-\frac14\begin{pmatrix}4\\2\end{pmatrix}\begin{pmatrix}4&2\end{pmatrix}
=\begin{pmatrix}0&0\\0&8\end{pmatrix}.
$$

The observed component now has zero [variance](variance-split.md). The second component remains uncertain, but its [posterior mean](posterior-mean.md) changes and its [variance](variance-split.md) falls from $9$ to $8$ because its prediction error had nonzero [correlation](pearson-correlation-coefficient.md) with that of the first. This is the mechanism by which measurements of one component can inform another.

## ↑ Ancestors (6)

1. [Kalman filter](kalman-filter.md)
2. [State estimation](state-estimation.md)
3. [Control theory](control-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33/4/solution.md)
