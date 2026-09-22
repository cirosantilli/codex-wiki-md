<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use fixed [masses](../../../../mass.md) in an isolated Newtonian $N$-body system, with origin at its [centre of mass](../../../../center-of-mass.md). Define the $xx$ moment $I_{xx}=\sum_i m_ix_i^2$ and $K_{xx}=\tfrac12\sum_i m_iv_{x,i}^2$. Twice differentiating gives

$$
\frac12\ddot I_{xx}=\sum_i m_iv_{x,i}^2+\sum_i m_ix_i\dot v_{x,i}=2K_{xx}+W_{xx}.
$$

Insert the gravitational [equation of motion](../../../../equation-of-motion.md) and pair each ordered term $(i,k)$ with $(k,i)$:

$$
\begin{aligned}
W_{xx}&=-G\sum_i\sum_{k\ne i}\frac{m_im_kx_i(x_i-x_k)}{r_{ik}^3}\\
&=-\frac G2\sum_i\sum_{k\ne i}\frac{m_im_k(x_i-x_k)^2}{r_{ik}^3}
=-G\sum_{i<k}\frac{m_im_k(x_i-x_k)^2}{r_{ik}^3}.
\end{aligned}
$$

Thus one component of the [tensor virial theorem](../../../../tensor-virial-theorem.md) is

$$
\boxed{\frac12\ddot I_{xx}=2K_{xx}-G\sum_{i<k}\frac{m_im_k(x_i-x_k)^2}{r_{ik}^3}.}
$$

A stationary or time-averaged bounded system has $\langle\ddot I_{xx}\rangle=0$, yielding $2\langle K_{xx}\rangle+\langle W_{xx}\rangle=0$. If ordered and random motions are separated, $2K_{xx}=2T_{xx}+\Pi_{xx}$, where $T_{xx}=\tfrac12\int\rho u_x^2dV$ and $\Pi_{xx}=\int\rho\sigma_{xx}^2dV$. Summing the three diagonal equations recovers the scalar [virial theorem](../../../../virial-theorem.md), with the pair [gravitational potential energy](../../../../gravitational-energy.md) counted once.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
