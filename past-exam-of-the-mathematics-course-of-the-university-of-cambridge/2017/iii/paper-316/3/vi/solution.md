<h1 id="3/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

First adopt the uniform-angular-motion approximation implicit in the requested formula. Set the line of sight to longitude zero, the $b$ [exoplanet transit](../../../../../../exoplanet-transit.md) to $t=0$, and the next $c$ [exoplanet transit](../../../../../../exoplanet-transit.md) to $t=\tau$, with $0\leq\tau<P_c$. Write $n_b=2\pi/P_b$, $n_c=2\pi/P_c$, with $P_c>P_b$. The next [conjunction](../../../../../../conjunction-astronomy.md) satisfies

$$
(n_b-n_c)t+n_c\tau=2\pi.
$$

The common longitude is $n_bt$ modulo $2\pi$. Subtracting one $2\pi$ gives the [conjunction longitude from a transit time lag](../../../../../../conjunction-longitude-from-a-transit-time-lag.md)

$$
\Lambda_{bc}=\frac{n_c(2\pi-n_b\tau)}{n_b-n_c}
=2\pi\frac{1-\tau/P_b}{P_c/P_b-1}.
$$

Substitution of the period ratio yields

$$
\boxed{\Lambda_{bc}=2\pi\left(1-\frac{\tau}{P_b}\right)\frac pq
\left[1+\delta\frac{p+q}{q}\right]^{-1}\pmod{2\pi}}.
$$

It is exact in this uniform-angle model; no first-order expansion in $\delta$ is necessary here. For other choices of which [exoplanet transit](../../../../../../exoplanet-transit.md) is used, choose the appropriate whole-turn branch.

**For the finite-eccentricity [orbit](../../../../../../orbit-dynamical-system.md) specified earlier, this is an approximation**. Let $f_L$ and $M_L$ be the [true anomaly](../../../../../../true-anomaly.md) and [mean anomaly](../../../../../../mean-anomaly.md) at the line of sight. The eccentric [planet](../../../../../../planet.md) has $M_c(t)=M_L+n_c(t-\tau)$ and true angular advance $n_c(t-\tau)+\Delta_e(t)$, where

$$
\Delta_e(t)=f_c(t)-M_c(t)-(f_L-M_L).
$$

True [conjunction](../../../../../../conjunction-astronomy.md) therefore requires $(n_b-n_c)t+n_c\tau-\Delta_e(t)=2\pi$. The PDF omits this term, which is generally $O(e_c)$.

For a concrete counterexample take $p=q=1$, $\delta=0$, $e_c=1/5$, $\tau=P_b/4$, and a line of sight along $c$'s [periapsis](../../../../../../periapsis.md). The uniform model predicts $t=7P_b/4$ and longitude $3\pi/2$. At that time $M_c=3\pi/2$, but [Kepler's equation](../../../../../../kepler-s-equation.md) gives $f_c\ne3\pi/2$, so the [planets](../../../../../../planet.md) are not truly aligned. Accurate finite-eccentricity [conjunctions](../../../../../../conjunction-astronomy.md) must be found from the corrected equation.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [3](../../3.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
