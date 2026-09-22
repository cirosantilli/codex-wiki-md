<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Parametrize the [unit circle](../../../../../../complex-unit-circle.md) by $\omega(\theta)=(\cos\theta,\sin\theta)$, with $-\pi\le\theta<\pi$ and $d\sigma=d\theta/(2\pi)$. Extract the constant phase at $\omega(0)$:

$$
e^{i\xi_1}\widehat{\psi\,d\sigma}(\xi)
=\frac1{2\pi}\int\psi(\omega(\theta))
 e^{-i[\xi_1(\cos\theta-1)+\xi_2\sin\theta]}\,d\theta.
$$

On the support, $|\theta|\le2\delta/C$. The frequency rectangle and the elementary bounds $|1-\cos\theta|\le\theta^2/2$, $|\sin\theta|\le|\theta|$ imply

$$
|\xi_1(\cos\theta-1)+\xi_2\sin\theta|
\le\frac2{C^2}+\frac2C.
$$

Choose the fixed constant $C$ large enough that this is less than $\pi/3$. Every phase then has real part at least $1/2$. Nonnegativity of $\psi$ prevents cancellation after this phase rotation, while its central plateau gives $\int\psi\,d\sigma\ge\delta/(\pi C)$. Hence the [Fourier transform](../../../../../../fourier-transform.md) satisfies

$$
\boxed{|\widehat{\psi\,d\sigma}(\xi)|
\ge\operatorname{Re}\!\left(e^{i\xi_1}\widehat{\psi\,d\sigma}(\xi)\right)
\ge\frac12\int\psi\,d\sigma
\ge\frac{\delta}{2\pi C}.}
$$

This is the [circle cap Fourier lower bound](../../../../../../circle-cap-fourier-lower-bound.md). No upper bound on the values of $\psi$ is needed here; the support, plateau and nonnegativity suffice. The long radial scale $\delta^{-2}$ comes from the quadratic term $\cos\theta-1$, whereas the transverse scale $\delta^{-1}$ comes from the linear term $\sin\theta$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
