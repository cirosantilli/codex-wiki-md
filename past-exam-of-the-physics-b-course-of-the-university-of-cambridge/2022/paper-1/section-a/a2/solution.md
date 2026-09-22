<h1 id="section-a/a2/solution">Solution</h1>

↑ **Parent:** [A2](../a2.md)

To find the [two-mass three-spring normal modes](../../../../../two-mass-three-spring-normal-modes.md), choose both displacements positive to the right, measured from [mechanical equilibrium](../../../../../mechanical-equilibrium.md). The middle [spring](../../../../../spring.md)'s extension changes by $x_2-x_1$. [Hooke's law](../../../../../hooke-s-law.md) and [Newton's second law](../../../../../newton-s-second-law.md) therefore give

$$
m_1\ddot x_1=-kx_1+k(x_2-x_1)=-2kx_1+kx_2,\qquad
m_2\ddot x_2=-kx_2-k(x_2-x_1)=kx_1-2kx_2.
$$

In a [normal mode](../../../../../normal-mode.md) both displacements have the same [angular frequency](../../../../../angular-frequency.md): take $x_j=A_j\cos(\omega t+\phi)$. A nonzero amplitude [vector](../../../../../vector.md) exists when the [determinant](../../../../../determinant.md) vanishes:

$$
\begin{vmatrix}2k-m_1\omega^2&-k\\-k&2k-m_2\omega^2\end{vmatrix}=0,
\qquad m_1m_2\omega^4-2k(m_1+m_2)\omega^2+3k^2=0.
$$

Writing $D=\sqrt{m_1^2-m_1m_2+m_2^2}$, the two [angular frequencies](../../../../../angular-frequency.md) are

$$
\boxed{\omega_\pm=\sqrt{\frac{k}{m_1m_2}(m_1+m_2\pm D)}.}
$$

The corresponding [eigenvectors](../../../../../eigenvector.md) can be specified by

$$
\frac{A_2}{A_1}=\frac{2k-m_1\omega_\pm^2}{k}
=\frac{m_2-m_1\mp D}{m_2}.
$$

Since $D>|m_2-m_1|$ for positive masses, the lower [normal mode](../../../../../normal-mode.md) $\omega_-$ has $A_2/A_1>0$: both bodies move in the same direction at any instant. The higher [normal mode](../../../../../normal-mode.md) $\omega_+$ has $A_2/A_1<0$: they move in opposite directions. Their amplitudes are generally unequal. For the useful check $m_1=m_2=m$, these reduce to $\omega_-=\sqrt{k/m}$ with $A_2=A_1$, and $\omega_+=\sqrt{3k/m}$ with $A_2=-A_1$. Each [angular frequency](../../../../../angular-frequency.md) has units $\mathrm{rad\,s^{-1}}$.

## ↑ Ancestors (14)

1. [A2](../a2.md)
2. [Section A](../../section-a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
