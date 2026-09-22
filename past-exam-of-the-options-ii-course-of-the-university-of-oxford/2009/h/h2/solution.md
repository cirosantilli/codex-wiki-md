<h1 id="h/h2/solution">Solution</h1>

↑ **Parent:** [H2](../h2.md)

The lower particle has position $(x+l\sin\theta,-l\cos\theta)$, so its squared speed is $\dot x^2+2l\cos\theta\,\dot x\dot\theta+l^2\dot\theta^2$. The bead contributes $m_1\dot x^2/2$ to the [kinetic energy](../../../../kinetic-energy.md). The two equal springs have combined [potential energy](../../../../potential-energy.md) $kx^2$ up to a constant: their lengths are $a+x$ and $a-x$, and equal natural lengths cancel the linear terms in the sum of their squared extensions. The gravitational potential is $-m_2gl\cos\theta$. Therefore

$$
L=\frac12(m_1+m_2)\dot x^2+m_2l\cos\theta\,\dot x\dot\theta+\frac12m_2l^2\dot\theta^2-kx^2+m_2gl\cos\theta.
$$

There is no explicit time dependence, so the total [energy](../../../../energy-split.md)

$$
E=\frac12(m_1+m_2)\dot x^2+m_2l\cos\theta\,\dot x\dot\theta+\frac12m_2l^2\dot\theta^2+kx^2-m_2gl\cos\theta
$$

is conserved. The [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) are

$$
(m_1+m_2)\ddot x+m_2l\cos\theta\,\ddot\theta-m_2l\sin\theta\,\dot\theta^2+2kx=0,
$$



$$
m_2l\cos\theta\,\ddot x+m_2l^2\ddot\theta+m_2gl\sin\theta=0.
$$

At rest these require $x=0$ and $\sin\theta=0$, giving the downward and upward positions $\theta=0,\pi$ modulo $2\pi$. The downward position has positive-definite quadratic potential and is stable, whereas the upward position has a negative angular potential curvature.

Keeping terms of second order about the stable position and dropping a constant gives

$$
L_2=\frac12(m_1+m_2)\dot x^2+m_2l\dot x\dot\theta+\frac12m_2l^2\dot\theta^2-kx^2-\frac12m_2gl\theta^2.
$$

For unit parameters the [mass matrix](../../../../mass-matrix.md) and [stiffness matrix](../../../../stiffness-matrix.md) are $M=\begin{pmatrix}2&1\\1&1\end{pmatrix}$ and $K=\begin{pmatrix}2&0\\0&1\end{pmatrix}$. A [normal mode](../../../../normal-mode.md) with squared frequency $s$ requires

$$
0=\det(K-sM)=(2-2s)(1-s)-s^2=s^2-4s+2.
$$

Thus the positive [angular frequencies](../../../../angular-frequency.md) are

$$
\boxed{\omega_-=\sqrt{2-\sqrt2},\qquad\omega_+=\sqrt{2+\sqrt2}}.
$$

## ↑ Ancestors (12)

1. [H2](../h2.md)
2. [H](../../h.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
