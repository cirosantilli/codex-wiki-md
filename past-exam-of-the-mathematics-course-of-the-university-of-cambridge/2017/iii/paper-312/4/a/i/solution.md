<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [comoving curvature perturbation](../../../../../../../comoving-curvature-perturbation.md) mode normalization. Take $H,\epsilon,c_s$ to be effectively constant at leading [slow-roll approximation](../../../../../../../slow-roll-approximation.md) order, with $H,\epsilon,c_s>0$, and use the [Bunch-Davies vacuum](../../../../../../../bunch-davies-vacuum.md) selected by the early-time $i\varepsilon$ contour. The regulator $\varepsilon$ is distinct from the [Hubble slow-roll parameter](../../../../../../../hubble-slow-roll-parameter.md) $\epsilon$.

Let $C=\epsilon+1-c_s^2$ and use the [Fourier transform](../../../../../../../fourier-transform.md) convention $\zeta(\mathbf x)=\int d^3k\,\zeta(\mathbf k)e^{i\mathbf k\cdot\mathbf x}/(2\pi)^3$. Conversion to [conformal time](../../../../../../../conformal-time.md) gives

$$
H_{\rm int}\,dt=-\frac{M_{\rm Pl}^2\epsilon C}{Hc_s^2}\int d^3x\,a\zeta'^3\,d\tau=\frac{M_{\rm Pl}^2\epsilon C}{H^2c_s^2\tau}\int d^3x\,\zeta'^3\,d\tau.
$$

The last sign follows from substituting $a=-1/(H\tau)$, which is positive for $\tau<0$; dropping the explicit minus sign in that substitution would reverse the final [primordial bispectrum](../../../../../../../primordial-bispectrum.md).

At the order needed by the [in-in formalism](../../../../../../../keldysh-formalism.md), the unequal-time [Wick contraction](../../../../../../../wick-contraction.md) is

$$
\langle\zeta(\mathbf k,0)\zeta'(\mathbf p,\tau)\rangle=(2\pi)^3\delta^{(3)}(\mathbf k+\mathbf p)u_k(0)u_k'^*(\tau).
$$

It uses the Gaussian quantum vacuum two-point function with the displayed operator ordering; an arbitrary classical unequal-time [covariance](../../../../../../../covariance.md) cannot replace it. For the connected three-point function, each external field contracts with one of the three fields at the vertex. There are $3!=6$ such [Wick contractions](../../../../../../../wick-contraction.md), all equal. The spatial integral conserves total momentum and leaves one factor $(2\pi)^3\delta^{(3)}(\mathbf k_1+\mathbf k_2+\mathbf k_3)$. The other nine pairings are disconnected tadpole terms supported on a zero external momentum; they are excluded from the connected [primordial bispectrum](../../../../../../../primordial-bispectrum.md), equivalently by subtracting the one-point function or normal ordering the vertex.

The free Gaussian odd correlator is zero. Applying the stated first-order [in-in formalism](../../../../../../../keldysh-formalism.md) therefore gives

$$
\boxed{B(k_1,k_2,k_3)=6\operatorname{Re}\!\left[-2i\int_{-\infty(1-i0)}^0\!d\tau\,\frac{M_{\rm Pl}^2\epsilon C}{H^2c_s^2\tau}\prod_{r=1}^3u_{k_r}(0)u_{k_r}'{}^*(\tau)\right].}
$$

By definition, the full connected correlator is $(2\pi)^3\delta^{(3)}(\sum_r\mathbf k_r)B$. The assumptions are a Gaussian [Bunch-Davies vacuum](../../../../../../../bunch-davies-vacuum.md), the given leading cubic vertex, tree order, the late-time limit $\tau\to0^-$, effectively constant background parameters, and connected nonzero external modes. No symmetry factor $1/3!$ is inserted into the given Hamiltonian.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 312](../../../../paper-312-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
