<h1 id="13c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With constant [masses](../../../../../../mass.md), differentiate the [moment of inertia](../../../../../../moment-of-inertia.md) twice:

$$
 \frac12I''=\sum_i m_i\dot r_i^2+\sum_i m_i r_i\cdot\ddot r_i=2K+\sum_i r_i\cdot F_i.
$$

For each pair, $F_{ij}=-Gm_im_j(r_i-r_j)/|r_i-r_j|^3$ and $F_{ji}=-F_{ij}$. Hence its contribution is $(r_i-r_j)\cdot F_{ij}=-Gm_im_j/|r_i-r_j|=V_{ij}$. Summing over unordered pairs gives $\sum r_i\cdot F_i=V$. Time-averaging over $[0,T]$ yields

$$
 2\overline K_T+\overline V_T=\frac{I'(T)-I'(0)}{2T}.
$$

For a bound system with $I'(T)=o(T)$, or a stationary equilibrium with zero average left-hand [derivative](../../../../../../derivative.md), the [limit](../../../../../../limit-of-a-function.md) is the [virial theorem](../../../../../../virial-theorem.md)

$$
\boxed{2\langle K\rangle+\langle V\rangle=0.}
$$

Bounded spatial extent together with bounded [velocities](../../../../../../velocity.md) suffices for the [derivative](../../../../../../derivative.md) condition; possible gravitational collisions must be excluded or otherwise regularized.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13C](../../13c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
