<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

Put $I_j=m_jr_j^2$ and $K=\omega^2r_1r_2$. The [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) are $I_1\ddot\phi_1=K\sin\psi$ and $I_2\ddot\phi_2=-K\sin\psi$, where $\psi=\phi_2-\phi_1$. Adding shows that **$I_1\dot\phi_1+I_2\dot\phi_2$ is conserved**. Subtracting gives the equation of a [simple pendulum](../../../../../simple-pendulum.md)

$$
\boxed{\ddot\psi=-k^2\sin\psi,\qquad
k^2=\omega^2r_1r_2\left(\frac1{m_1r_1^2}+\frac1{m_2r_2^2}\right).}
$$

The relative equilibria are $\psi=0$ and $\psi=\pi$ modulo $2\pi$. The relative energy $\dot\psi^2/2+k^2(1-\cos\psi)$ has a strict minimum at zero, proving stability there. Linearization gives $\ddot\eta=-k^2\eta$ near zero and $\ddot\eta=k^2\eta$ near $\pi$, so the latter is unstable. The small-oscillation period is **$2\pi/k$**. These are equilibria of the relative angle; a nonzero conserved total [angular momentum](../../../../../angular-momentum.md) permits common rotation of both particles.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
