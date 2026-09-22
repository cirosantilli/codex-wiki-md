# Weak-fluctuation memory equation for the coherent field

↑ **Parent:** [Coherent wave field](coherent-wave-field.md)

For a [parabolic wave equation](parabolic-wave-equation.md) with $n=1+\mu W$, a zero-mean stationary real field $W$ of unit variance, and $L_0=i\partial_z^2/(2k)$, finite-correlation perturbation theory gives

$$
\begin{aligned}
 m_x&=L_0m+\frac{ik\mu^2}{2}m\\
 &\quad-k^2\mu^2\int_{x_0}^x\int_{\mathbb R}C(x-s,z-\zeta)G_{x-s}(z-\zeta)m(s,\zeta)\,d\zeta\,ds+O(\mu^3).
\end{aligned}
$$

Here $m$ is the [coherent field](coherent-wave-field.md), $C$ is the [autocorrelation function of a random field](autocorrelation-function-of-a-random-field.md) and $G$ is the one-coordinate [Fresnel propagator](fresnel-propagator.md). Expand the random solution once using the [Duhamel principle](duhamel-s-principle.md), multiply by $W$ and average to obtain the memory term. The local phase term comes from the $\mu^2W^2$ term in $n^2$. The expansion is for fixed propagation distances with suitable covariance regularity and moment bounds. A [Markov approximation](markov-approximation-for-a-random-medium.md) is an additional scale assumption that can turn this integral equation into a local attenuation equation.

**Table of contents**

- [Quadratic refractive-index shift in the coherent field](quadratic-refractive-index-shift-in-the-coherent-field.md)

## ↑ Ancestors (7)

1. [Coherent wave field](coherent-wave-field.md)
2. [Wave propagation in a random medium](wave-propagation-in-a-random-medium.md)
3. [Random medium](random-medium.md)
4. [Wave scattering](wave-scattering.md)
5. [Wave](wave.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-76/1/d/solution.md)
