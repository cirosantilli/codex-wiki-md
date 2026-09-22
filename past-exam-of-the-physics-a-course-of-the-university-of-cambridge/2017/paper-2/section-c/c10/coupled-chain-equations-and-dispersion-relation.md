<h1 id="section-c/c10/coupled-chain-equations-and-dispersion-relation">Coupled-chain equations and dispersion relation</h1>

↑ **Parent:** [Solution](solution.md)

Put type-A atoms at $2ja$ and type-B atoms at $(2j+1)a$. Their displacements $u_j,v_j$ obey [Newton's second law](../../../../../newton-s-second-law.md),

$$
m_A\ddot u_j=\alpha(v_j+v_{j-1}-2u_j),\qquad
m_B\ddot v_j=\alpha(u_j+u_{j+1}-2v_j).
$$

Choose [normal modes](../../../../../normal-mode.md) $u_j=Ue^{i(2jaq-\omega t)}$ and $v_j=Ve^{i((2j+1)aq-\omega t)}$. Substitution gives

$$
\begin{pmatrix}2\alpha-m_A\omega^2&-2\alpha\cos qa\\-2\alpha\cos qa&2\alpha-m_B\omega^2\end{pmatrix}
\begin{pmatrix}U\\V\end{pmatrix}=0.
$$

A nonzero displacement vector requires zero [determinant](../../../../../determinant.md):

$$
m_Am_B\omega^4-2\alpha(m_A+m_B)\omega^2+4\alpha^2\sin^2qa=0.
$$

Solving this quadratic in $\omega^2$ gives the [diatomic-chain dispersion relation with equal springs](../../../../../diatomic-chain-dispersion-relation-with-equal-springs.md),

$$
\boxed{\omega_\pm^2=\frac\alpha{m_Am_B}\left[(m_A+m_B)\pm\sqrt{(m_A+m_B)^2-4m_Am_B\sin^2qa}\right]}.
$$

The [primitive unit cell](../../../../../primitive-unit-cell.md) has length $2a$, so the first [Brillouin zone](../../../../../brillouin-zone.md) is $|q|\leq\pi/(2a)$.

## ↑ Ancestors (15)

1. [Solution](solution.md)
2. [C10](../c10.md)
3. [Section C](../../section-c.md)
4. [Paper 2](../../../paper-2-split.md)
5. [2017](../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
