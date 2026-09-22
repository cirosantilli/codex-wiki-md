<h1 id="h/h2/solution">Solution</h1>

↑ **Parent:** [H2](../h2.md)

The lower [mass](../../../../mass.md) has coordinates $(x+l\sin\theta,-l\cos\theta)$. Its squared speed is $\dot x^2+2l\cos\theta\,\dot x\dot\theta+l^2\dot\theta^2$. Adding the bead's [kinetic energy](../../../../kinetic-energy.md) gives the kinetic part of the supplied [Lagrangian](../../../../lagrangian.md). Equal [spring](../../../../spring.md) prestresses give [spring](../../../../spring.md) energy $kx^2$ up to a constant: the two squared extensions are proportional to $(a+x-\ell_0)^2+(a-x-\ell_0)^2$. The gravitational potential is $-m_2gl\cos\theta$. Thus $L=T-V$ has exactly the stated form, with constant energy offsets discarded.

Since $L$ has no explicit time dependence, the conserved energy is

$$
\boxed{E=\tfrac12(m_1+m_2)\dot x^2+m_2l\cos\theta\,\dot x\dot\theta+\tfrac12m_2l^2\dot\theta^2+kx^2-m_2gl\cos\theta.}
$$

The two Euler–Lagrange equations are

$$
\begin{aligned}
(m_1+m_2)\ddot x+m_2l\cos\theta\,\ddot\theta-m_2l\sin\theta\,\dot\theta^2+2kx&=0,\\
m_2l\cos\theta\,\ddot x+m_2l^2\ddot\theta+m_2gl\sin\theta&=0.
\end{aligned}
$$

At equilibrium, $x=0$ and $\sin\theta=0$. There are two geometrically distinct positions, $\boxed{(x,\theta)=(0,0),(0,\pi)}$ modulo $2\pi$. The downward one has positive potential Hessian $\operatorname{diag}(2k,m_2gl)$ and is stable; the inverted one has a negative angular [curvature](../../../../second-derivative.md) and is unstable.

Keeping only quadratic terms about the downward equilibrium gives

$$
L_2=\tfrac12(m_1+m_2)\dot x^2+m_2l\dot x\dot\theta+\tfrac12m_2l^2\dot\theta^2-kx^2-\tfrac12m_2gl\theta^2.
$$

For unit parameters, the [mass](../../../../mass.md) and stiffness [matrices](../../../../matrix.md) are $M=\begin{pmatrix}2&1\\1&1\end{pmatrix}$ and $K=\begin{pmatrix}2&0\\0&1\end{pmatrix}$. The equation $\det(K-\omega^2M)=0$ is $\omega^4-4\omega^2+2=0$. Therefore the normal angular frequencies are

$$
\boxed{\omega_-=\sqrt{2-\sqrt2},\qquad\omega_+=\sqrt{2+\sqrt2}.}
$$

## ↑ Ancestors (12)

1. [H2](../h2.md)
2. [H](../../h.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
