<h1 id="4/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Write $\epsilon=\mu^{1/3}$ and $\delta_j=(a_j-a_0)/a_0$. The leading [Keplerian shear](../../../../../../keplerian-shear.md) is

$$
\frac{n_j-n_0}{n_0}=-\frac32\delta_j+O(\delta_j^2,\mu).
$$

The distinction between total mass $m$ and the individual [planet](../../../../../../planet.md)'s two-body central mass is order $\mu$, below the retained order $\epsilon$.

At one common reference epoch, the local [Kepler orbit](../../../../../../kepler-orbit.md) expansion takes the form

$$
\frac{x'_j}{a_0}-1\simeq\delta_j-e_j\cos(n_0t-\varpi_j),\qquad
\frac{y'_j}{a_0}\simeq-\frac32\delta_j n_0t+2e_j\sin(n_0t-\varpi_j)+\lambda_{j,0},
$$

where $\lambda_{j,0}$ is the initial [mean longitude](../../../../../../mean-longitude.md) relative to the rotating reference ray. Comparing its sine and cosine coefficients with the [free solution of Hill equations](../../../../../../free-solution-of-hill-equations.md) gives

$$
D_{1j}=-\frac{e_j}{\epsilon}\cos\varpi_j,\qquad
D_{2j}=-\frac{e_j}{\epsilon}\sin\varpi_j,\qquad
D_{3j}=\frac{\delta_j}{\epsilon},\qquad
D_{4j}=\frac{\lambda_{j,0}}\epsilon.
$$

The required [orbital elements from Hill coordinates](../../../../../../orbital-elements-from-hill-coordinates.md) are therefore

$$
\boxed{a_j=a_0(1+\epsilon D_{3j}),\qquad
e_j=\epsilon\sqrt{D_{1j}^2+D_{2j}^2},\qquad
\varpi_j=\operatorname{atan2}(-D_{2j},-D_{1j})\pmod{2\pi}.}
$$

These equalities have the first-order accuracy of the local approximation. If $e_j=0$, the [longitude of periapsis](../../../../../../longitude-of-periapsis.md) is undefined. The combination $D_{4j}+2D_{2j}$ fixes the initial true longitude divided by $\epsilon$. The special initial alignment imposed in part v would require $D_{4j}=-2D_{2j}$, but the general two-planet solution need not impose it.

Substitution also verifies $\ddot\xi_j-2n_0\dot\eta_j-3n_0^2\xi_j=0$ and $\ddot\eta_j+2n_0\dot\xi_j=0$: these are the unforced [Hill equations](../../../../../../hill-equations.md). Close encounters add mutual-gravity forcing and can change the constants. Replacing $n_j$ by $n_0$ in the oscillation is consistent at leading order over local orbital times; accumulated phase differences must be retained when following much longer evolution.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [4](../../4.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
