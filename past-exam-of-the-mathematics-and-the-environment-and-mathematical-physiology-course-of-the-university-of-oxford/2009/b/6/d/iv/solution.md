<h1 id="b/6/d/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For the [first Hopf boundary of scalar delayed negative feedback](../../../../../../first-hopf-boundary-of-scalar-delayed-negative-feedback.md), first, if a root has nonnegative [real part](../../../../../../real-part.md) then $|\lambda+\beta|=\gamma e^{-\operatorname{Re}\lambda}\le\gamma$. For $\beta\ge\gamma$ this is impossible, apart from the potential equality case $\lambda=0$, already excluded. Thus $\beta<\gamma$ is necessary for instability, although not sufficient by itself.

At an imaginary root $\lambda=i\omega$ with $\omega>0$, separate real and imaginary parts:

$$
\beta+\gamma\cos\omega=0,\qquad\omega=\gamma\sin\omega.
$$

The first crossing uses $\omega_c\in(\pi/2,\pi)$ for $\beta>0$, and satisfies

$$
\boxed{\beta=-\omega_c\cot\omega_c,\qquad\gamma_c=\frac{\omega_c}{\sin\omega_c}=\sqrt{\beta^2+\omega_c^2},\qquad\mathcal T_c=\frac{2\pi}{\omega_c}.}
$$

The [period](../../../../../../period-of-a-function.md) is in scaled [time](../../../../../../time-in-physics.md); its physical value is $\tau\mathcal T_c$. Higher-frequency branches have larger critical gains. For fixed $\beta$, stability at zero delayed gain and absence of any earlier imaginary or zero-root crossing identify this lowest branch as the first stability boundary. Its crossing is transverse: implicit differentiation of $\lambda+\beta+\gamma e^{-\lambda}=0$ gives at the imaginary root

$$
\operatorname{Re}\frac{d\lambda}{d\gamma}=\frac{\beta(1+\beta)+\omega_c^2}{\gamma[(1+\beta)^2+\omega_c^2]}>0.
$$

For very small $\beta$, $\omega_c=\pi/2+2\beta/\pi+O(\beta^2)$, so $\mathcal T_c\to4$ and $\gamma_c=\pi/2+2\beta/\pi+O(\beta^2)$. Therefore **$\gamma_c=\pi/2$ is exact in the limit $\beta=0$ and is the leading approximation for small positive $\beta$**. At that limit $\lambda e^\lambda=-\gamma$ first has an imaginary pair at $\lambda=\pm i\pi/2$; subsequent pairs occur at $\pi/2+2n\pi$ and cannot be the first loss of stability. A nonlinear Hopf theorem, including its nondegeneracy conditions, is needed to turn the linear imaginary mode into a claim about a particular finite-amplitude periodic branch.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [D](../../d.md)
3. [6](../../../6.md)
4. [B](../../../../b.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../split.md)
7. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
