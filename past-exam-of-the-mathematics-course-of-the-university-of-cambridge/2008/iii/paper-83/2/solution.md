<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Set $\zeta=\gamma/m>0$ and $\mathbf A=\mathbf A'/m$. Multiplying the [Langevin equation](../../../../../langevin-dynamics.md) by $e^{\zeta t}$ and integrating gives

$$
\boxed{\mathbf u(t)=\mathbf u_0e^{-\zeta t}+\mathbf U(t),\qquad \mathbf U(t)=\int_0^te^{-\zeta(t-s)}\mathbf A(s)\,ds.}
$$

The [expected value](../../../../../expected-value.md) of $\mathbf U$ is zero. For the printed dot-product force covariance, write $C_A(s-s')=\phi(|s-s'|)/m^2$, so $\int C_A(y)dy=\tau$. Without any white-noise approximation the trace [variance](../../../../../variance-split.md) is

$$
\langle|\mathbf U|^2\rangle=\int_0^t\!ds\int_0^t\!ds'\,e^{-\zeta(2t-s-s')}C_A(s-s').
$$

The intended short-correlation approximation replaces $C_A(y)$ by $\tau\delta(y)$, where $\delta$ is the [Dirac delta](../../../../../dirac-delta-function.md). It requires the force correlation time to be much shorter than $\zeta^{-1}$ and the observation time. Then

$$
\boxed{\langle|\mathbf U|^2\rangle=\frac{\tau}{2\zeta}(1-e^{-2\zeta t}).}
$$

At [thermal equilibrium](../../../../../thermal-equilibrium.md), the [equipartition theorem](../../../../../equipartition-theorem.md) gives $m\langle|\mathbf u|^2\rangle/2=3k_BT/2$. Taking the long-time limit determines the [vector noise normalization in inertial Langevin dynamics](../../../../../vector-noise-normalization-in-inertial-langevin-dynamics.md):

$$
\boxed{\tau=\frac{6\zeta k_BT}{m}=\frac{6\gamma k_BT}{m^2}.}
$$

This factor six corresponds to the dot-product covariance across three components. If $\phi$ were defined for one component instead, its integrated strength would be $2\gamma k_BT$ before dividing by $m^2$, and the acceleration strength would be $2\zeta k_BT/m$.

Finite rapid correlation is not literally a [Dirac delta](../../../../../dirac-delta-function.md). For a stationary force and local drag, its exact limiting velocity trace is

$$
\langle|\mathbf u|^2\rangle_\infty=\frac1{2\zeta}\int_{-\infty}^{\infty}C_A(y)e^{-\zeta|y|}\,dy.
$$

This follows by splitting the double convolution into $s\ge s'$ and $s'\ge s$. Thus equipartition fixes the weighted integral, not just $\tau$, unless the short-correlation approximation is made. For example, $C_A(y)=\tau e^{-|y|/t_c}/(2t_c)$ gives $\tau/[2\zeta(1+\zeta t_c)]$. The remaining explicit formulae use the intended [continuous-time Gaussian white noise](../../../../../continuous-time-gaussian-white-noise.md) limit.

Assume isotropic jointly [Gaussian noise](../../../../../gaussian-noise.md), as appropriate to an isotropic bath. The component covariance is

$$
\langle A_i(s)A_j(s')\rangle=\frac{\tau}{3}\delta_{ij}\delta(s-s')=\frac{2\zeta k_BT}{m}\delta_{ij}\delta(s-s').
$$

The scalar moment identities in the question must now be applied to a fixed Cartesian component $X=U_i$, not to the magnitude of the vector. Its [variance](../../../../../variance-split.md) is

$$
s_t^2=\langle U_i^2\rangle=\frac{k_BT}{m}(1-e^{-2\zeta t}).
$$

In the $2n$-fold integral for $\langle X^{2n}\rangle$, the [Isserlis theorem](../../../../../isserlis-s-theorem.md) replaces the force product by a sum of complete pairings. Each pairing yields $n$ identical two-time integrals, hence $(s_t^2)^n$. Pair the first labelled factor in $2n-1$ ways, then the first unpaired factor in $2n-3$ ways, and continue. The [Gaussian even-moment pairing count](../../../../../gaussian-even-moment-pairing-count.md) is

$$
(2n-1)(2n-3)\cdots1=(2n-1)!!=\frac{(2n)!}{2^nn!}.
$$

Odd force products vanish, so

$$
\boxed{\langle U_i^{2n+1}\rangle=0,\qquad \langle U_i^{2n}\rangle=(2n-1)!!(s_t^2)^n.}
$$

For completeness, summing the scalar [moment-generating function](../../../../../moment-generating-function.md) gives

$$
\langle e^{aU_i}\rangle=\sum_{n=0}^{\infty}\frac{a^{2n}}{(2n)!}(2n-1)!!(s_t^2)^n=e^{a^2s_t^2/2}.
$$

The same [Gaussian process](../../../../../gaussian-process.md) argument for every linear combination of components gives the vector [characteristic function](../../../../../characteristic-function.md) $\langle e^{i\mathbf k\cdot\mathbf U}\rangle=e^{-s_t^2|\mathbf k|^2/2}$. Inverting this [Fourier transform](../../../../../fourier-transform.md) yields the normalized [multivariate Gaussian distribution](../../../../../multivariate-gaussian-distribution.md)

$$
\boxed{W(\mathbf u,t;\mathbf u_0)=\left[\frac{m}{2\pi k_BT(1-e^{-2\zeta t})}\right]^{3/2}\exp\left[-\frac{m|\mathbf u-\mathbf u_0e^{-\zeta t}|^2}{2k_BT(1-e^{-2\zeta t})}\right].}
$$

The initial condition is a velocity [Dirac delta](../../../../../dirac-delta-function.md) as $t\downarrow0$, and the long-time limit is the thermal velocity density. The converted TeX's exponent is damaged; the PDF has the squared norm displayed here. The scalar pairing formula cannot be interpreted as a vector-norm formula: the [radial moments of an isotropic Gaussian vector](../../../../../radial-moments-of-an-isotropic-gaussian-vector.md) instead give $\langle|\mathbf U|^{2n}\rangle=(2n+1)!!(s_t^2)^n$ in three dimensions.

Integrate the velocity once more. Interchanging the time integrals gives the [integrated Ornstein-Uhlenbeck displacement](../../../../../integrated-ornstein-uhlenbeck-displacement.md)

$$
\boxed{\mathbf r(t)=\mathbf r_0+\frac{1-e^{-\zeta t}}{\zeta}\mathbf u_0+\frac1\zeta\int_0^t[1-e^{-\zeta(t-s)}]\mathbf A(s)\,ds.}
$$

For the stated fixed initial position and velocity,

$$
\boxed{\langle\mathbf r(t)\rangle=\mathbf r_0+\frac{1-e^{-\zeta t}}\zeta\mathbf u_0.}
$$

Let $\mathbf R=\mathbf r-\langle\mathbf r\rangle$ and $D=k_BT/\gamma$. Its component [covariance](../../../../../covariance.md) comes from integrating the squared noise kernel:

$$
\begin{aligned}
\langle R_iR_j\rangle&=\delta_{ij}\frac{2\zeta k_BT/m}{\zeta^2}\int_0^t(1-e^{-\zeta v})^2dv\\
&=2D\delta_{ij}\left[t-\frac{2(1-e^{-\zeta t})}{\zeta}+\frac{1-e^{-2\zeta t}}{2\zeta}\right].
\end{aligned}
$$

Therefore the total centered [variance](../../../../../variance-split.md) is

$$
\boxed{\langle|\mathbf R|^2\rangle=6D\left[t-\frac{2(1-e^{-\zeta t})}{\zeta}+\frac{1-e^{-2\zeta t}}{2\zeta}\right].}
$$

The mean-square displacement from $\mathbf r_0$ additionally contains $|\mathbf u_0|^2(1-e^{-\zeta t})^2/\zeta^2$. Confusing this deterministic drift contribution with centered [variance](../../../../../variance-split.md) changes the short-time conclusion.

For times longer than the force correlation time but $\zeta t\ll1$, the mean motion is $\mathbf r_0+\mathbf u_0t+O(t^2)$ and the centered trace is $2\zeta(k_BT/m)t^3+O(t^4)$. Thus a nonzero fixed initial velocity produces a leading ballistic mean-square displacement $|\mathbf u_0|^2t^2$; conditioned on $\mathbf u_0=0$, the white-noise displacement variance instead starts as $t^3$. If one averages over an independent equilibrium initial velocity, its covariance adds $3(k_BT/m)(1-e^{-\zeta t})^2/\zeta^2$, giving

$$
\langle|\mathbf r-\mathbf r_0|^2\rangle_{\rm eq}=6D\left[t-\frac{1-e^{-\zeta t}}\zeta\right]\sim\frac{3k_BT}{m}t^2.
$$

This is the usual thermal ballistic regime, before velocity memory has relaxed. At $\zeta t\gg1$, the conditional mean approaches $\mathbf r_0+\mathbf u_0/\zeta$, while the centered trace is $6Dt-9D/\zeta+O(e^{-\zeta t})$. Its leading behavior is **diffusion with $\langle|\mathbf R|^2\rangle\sim6Dt$ and $D=k_BT/\gamma$**, as successive displacement increments lose inertial memory. At times below a finite force correlation time the white-noise short-time expansion is not applicable; for a regular force covariance and fixed initial velocity the leading noise-induced displacement variance is of order $t^4$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 83](../../paper-83-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
