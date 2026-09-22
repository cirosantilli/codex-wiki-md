<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) of the quadratic [Lagrangian](../../../../../lagrangian.md) are

$$
\ddot{\boldsymbol\theta}+\mathsf K\boldsymbol\theta=0,\qquad
\mathsf K=\begin{pmatrix}1+k&-k\\-k&1+k\end{pmatrix}.
$$

The [mechanical mass matrix](../../../../../mechanical-mass-matrix.md) is the identity. A [normal mode](../../../../../normal-mode.md) $\boldsymbol\theta=\mathbf a\cos(\omega t+\phi)$ therefore satisfies the [eigenvalue problem](../../../../../eigenvalue-problem.md) $\mathsf K\mathbf a=\omega^2\mathbf a$. Direct multiplication gives

$$
\boxed{\begin{array}{c|c|c}
&\text{angular frequency}&\text{mode vector}\\\hline
\text{in phase}&\omega_+=1&(1,1)\\
\text{opposite phase}&\omega_-=\sqrt{1+2k}&(1,-1)
\end{array}}
$$

These are [normal modes of two spring-coupled equal pendulums](../../../../../normal-modes-of-two-spring-coupled-equal-pendulums.md). The corresponding [normal mode coordinates](../../../../../normal-coordinate.md) $u=\theta_1+\theta_2$ and $v=\theta_1-\theta_2$ obey $\ddot u+u=0$ and $\ddot v+(1+2k)v=0$.

For the in-phase [normal mode](../../../../../normal-mode.md), the bobs undergo identical [displacements](../../../../../displacement.md), leaving their separation exactly $r$. The [spring](../../../../../spring.md) stays at its natural length and exerts no [force](../../../../../force-split.md), so this [angular frequency](../../../../../angular-frequency.md) is independent of $k$. The value $1$ is the individual [simple pendulum](../../../../../simple-pendulum-split.md) [angular frequency](../../../../../angular-frequency.md) $\sqrt{g/l}$ in the chosen units.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the classical mechanics course of the University of Oxford](../../../../split.md)
6. [Classical mechanics course of the University of Oxford](../../../../../classical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
