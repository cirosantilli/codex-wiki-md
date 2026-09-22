<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $L_\tau=y^{-1/2}(\mathbb Z\tau+\mathbb Z)$, a covolume-one lattice, and define

$$
\Theta_{k,\tau}(t)=
\sum_{0\ne z\in L_\tau}\overline z^{,k}e^{-\pi t|z|^2}.
$$

Termwise Mellin transformation in the initial half-plane gives

$$
G_k(\tau,s)=
\frac{\pi^{s+k}y^{-k/2}}{\Gamma(s+k)}
\int_0^\infty\Theta_{k,\tau}(t)t^{s+k-1}\,dt.
$$

Split the integral at $t=1$. The integral over $[1,\infty)$ is entire in $s$ because the theta sum decays exponentially. Apply the [Poisson summation formula for a Euclidean lattice](../../../../../../poisson-summation-formula-for-a-euclidean-lattice.md) and the Fourier eigenfunction calculation from part b to the interval $(0,1]$, then substitute $t\mapsto1/t$. This rewrites the small-time integral as another exponentially convergent integral over $[1,\infty)$ plus explicit elementary Mellin terms. Those terms are meromorphic, but for positive even $k$ their apparent poles are canceled by the zeros of $1/\Gamma(s+k)$. The displayed formula therefore continues holomorphically to every $s\in\mathbb C$, proving the [analytic continuation of a weight-k real-analytic Eisenstein series](../../../../../../analytic-continuation-of-a-weight-k-real-analytic-eisenstein-series.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
