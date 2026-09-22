<h1 id="three-coordinate-state-realization-of-an-arma-1-1-process">Three-coordinate state realization of an ARMA(1,1) process</h1>

↑ **Parent:** [State-space model (time series)](state-space-model-time-series.md)

For an [autoregressive moving-average model](autoregressive-moving-average-model.md) of order $(1,1)$, this state has observation row $F=(\phi,1,\theta)$ and transition [matrix](matrix.md)

$$
G=\begin{pmatrix}\phi&1&\theta\\0&0&0\\0&1&0\end{pmatrix}.
$$

The state noise is $(0,\varepsilon_t,0)^\top$. Its first transition row reconstructs $X_{t-1}$ and its third row shifts the previous [white noise](white-noise.md) value.

**Table of contents**

- [Stationary initialization of an ARMA(1,1) state](stationary-initialization-of-an-arma-1-1-state.md)

## ↑ Ancestors (6)

1. [State-space model (time series)](state-space-model-time-series.md)
2. [Time series](time-series-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33/4/solution.md)
