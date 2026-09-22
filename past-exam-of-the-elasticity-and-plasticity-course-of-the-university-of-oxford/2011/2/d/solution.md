<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the complex [amplitude](../../../../wave-amplitude.md) and take its [real part](../../../../real-part.md) at the end; the equations are linear with real coefficients. Let $M=\lambda+2\mu$, $\omega=kc$, and $v=(A,B)^T$. The differential operators on this [exponential function](../../../../exponential-function.md) are $\partial_X=ik$, $\partial_Y=-b$, and $\partial_t=-i\omega$. Substitution gives

$$
\begin{pmatrix}
\mu b^2-Mk^2+\rho k^2c^2&-i(\lambda+\mu)kb\\
-i(\lambda+\mu)kb&Mb^2-\mu k^2+\rho k^2c^2
\end{pmatrix}\binom AB=0.
$$

The [determinant](../../../../determinant.md) factors as

$$
\mu M\left[b^2-k^2+\frac{\rho k^2c^2}{M}\right]
\left[b^2-k^2+\frac{\rho k^2c^2}{\mu}\right].
$$

Consequently choose the positive decay roots

$$
\boxed{b_1=k\sqrt{1-c^2/c_L^2},\qquad b_2=k\sqrt{1-c^2/c_T^2}.}
$$

The [Rayleigh wave decay exponents](../../../../rayleigh-wave-decay-exponents.md) must both give strict decay into the half-space. A genuine nonzero [Rayleigh wave](../../../../rayleigh-wave.md) combines both, as the free-surface equations below also show. Thus $b_1,b_2>0$ requires $\boxed{0<c<\min(c_T,c_L)}$. In a stable ordinary isotropic solid $c_T<c_L$, so it is slower even than the [transverse wave](../../../../transverse-wave.md). The roots depend on the candidate speed as well as the material constants and [wavenumber](../../../../wavenumber.md); the speed is fixed by the [boundary condition](../../../../boundary-condition.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
