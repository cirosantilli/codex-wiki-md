<h1 id="invertible-arma-factorization-of-an-ar-1-plus-noise-process">Invertible ARMA factorization of an AR(1)-plus-noise process</h1>

↑ **Parent:** [Autocovariance of an AR(1) process observed with white noise](autocovariance-of-an-ar-1-process-observed-with-white-noise.md)

Filtering the observations by $1-\phi B$ gives covariance $A=\sigma_z^2+(1+\phi^2)\sigma_w^2$ at zero, $C=-\phi\sigma_w^2$ at lag one and zero elsewhere. Set $\nu=(A+\sqrt{A^2-4C^2})/2$ and $\vartheta=C/\nu$. Then $\nu(1+\vartheta^2)=A$, $\nu\vartheta=C$ and $|\vartheta|<1$. Applying $(1+\vartheta B)^{-1}$ defines actual white-noise innovations with variance $\nu$, proving an at-most-(1,1) ARMA representation without assuming Gaussianity.

## ↑ Ancestors (9)

1. [Autocovariance of an AR(1) process observed with white noise](autocovariance-of-an-ar-1-process-observed-with-white-noise.md)
2. [Autoregressive process of order one](autoregressive-process-of-order-one.md)
3. [Autoregressive model](autoregressive-model.md)
4. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
5. [Time series](time-series-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-36/2/c/solution.md)
