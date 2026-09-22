<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Assume small planar oscillations about the vertical equilibrium, with the connecting [spring](../../../spring.md) relaxed in that equilibrium. Let $x_j=l\theta_j$ be the first-order horizontal [displacements](../../../displacement.md) of the two [simple pendulums](../../../simple-pendulum-split.md). The gravitational restoring [force](../../../force-split.md) on bob $j$ is $-(mg/l)x_j$; the spring extension to first order is $x_2-x_1$. Thus the linearized [equations of motion](../../../equation-of-motion.md) are

$$
\begin{aligned}
m\ddot x_1&=-\frac{mg}{l}x_1+k(x_2-x_1),\\
m\ddot x_2&=-\frac{mg}{l}x_2+k(x_1-x_2).
\end{aligned}
$$

Adding and subtracting them diagonalizes the system. For $q_+=x_1+x_2$ and $q_-=x_1-x_2$,

$$
\ddot q_++\frac glq_+=0,\qquad
\ddot q_-+\left(\frac gl+\frac{2k}{m}\right)q_-=0.
$$

The [normal modes](../../../normal-mode.md) and [angular frequencies](../../../angular-frequency.md) are therefore

$$
\boxed{\begin{array}{c|c}
\text{mode shape}&\text{angular frequency}\\\hline
(1,1)^T&\omega_1=\sqrt{g/l}\\
(1,-1)^T&\omega_2=\sqrt{g/l+2k/m}
\end{array}}
$$

The in-phase mode does not stretch the spring, while the opposite-phase mode adds a restoring force of magnitude $2k$ times each bob's displacement. These are the small-oscillation frequencies, not exact amplitude-independent frequencies for arbitrary pendulum angles.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2019 resit](../../2019-resit-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
