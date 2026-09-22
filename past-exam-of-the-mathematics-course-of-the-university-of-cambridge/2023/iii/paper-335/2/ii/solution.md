<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

To first order in the weak fluctuation, $n^2-1=2\mu W+O(\mu^2)$, so

$$
E_x=\frac{i}{2k}E_{zz}+ik\mu WE.
$$

For

$$
F=E_1E_2^*E_3E_4^*,
\qquad E_j=E(x,z_j),
$$

introduce the signs $s=(1,-1,1,-1)$. The [product rule](../../../../../../product-rule.md) gives

$$
\partial_x\langle F\rangle
=\frac{i}{2k}
\left(\partial_{z_1}^2-\partial_{z_2}^2
+\partial_{z_3}^2-\partial_{z_4}^2\right)m_4
+ik\mu\sum_{j=1}^4s_j\langle W(x,z_j)F\rangle.
$$

Assume that $W$ is a zero-mean [stationary Gaussian random field](../../../../../../stationary-gaussian-random-field.md), that its longitudinal [correlation length](../../../../../../correlation-length.md) is short compared with the envelope's evolution scale, and that the propagation distance is long compared with that correlation length. The forward [Markov approximation](../../../../../../markov-approximation-for-a-random-medium.md) then neglects diffraction during one correlation length. Applying the [Furutsu–Novikov formula](../../../../../../novikov-s-theorem.md) closes the last average at second order in $\mu$. Define the integrated longitudinal [autocorrelation function of a random field](../../../../../../autocorrelation-function-of-a-random-field.md)

$$
C(\zeta)=\int_{-\infty}^{\infty}
\rho(\xi,\zeta)\,d\xi.
$$

Then

$$
\boxed{
\partial_xm_4
=\frac{i}{2k}
\left(\partial_{z_1}^2-\partial_{z_2}^2
+\partial_{z_3}^2-\partial_{z_4}^2\right)m_4
-Q_4m_4},
$$

where

$$
\boxed{
Q_4=\frac{k^2\mu^2}{2}
\sum_{i,j=1}^4s_is_jC(z_i-z_j)}.
$$

Writing $C_{ij}=C(z_i-z_j)$ and using the evenness of the covariance gives the equivalent expression

$$
Q_4=k^2\mu^2
\left(2C(0)-C_{12}+C_{13}-C_{14}
-C_{23}+C_{24}-C_{34}\right).
$$

The derivation also assumes [paraxial propagation](../../../../../../paraxial-approximation.md), weak scattering, sufficient regularity to interchange differentiation and [expectation](../../../../../../expected-value.md), and statistical homogeneity in both coordinates. Without the short-correlation approximation, the Gaussian identity produces a nonlocal longitudinal memory integral rather than this local closed equation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
