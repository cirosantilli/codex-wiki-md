<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To first order in the applied fields, the carrier acceleration gives $m\dot{\mathbf v}=q\mathbf E$. The [current density](../../../../../current-density.md) $\mathbf j=nq\mathbf v$ consequently obeys the first [London equation](../../../../../london-equations.md)

$$
\dot{\mathbf j}=\frac{nq^2}{m}\mathbf E=\epsilon_0\omega_p^2\mathbf E.
$$

Taking its curl and using [Faraday's law](../../../../../faraday-s-law-of-induction.md) yields

$$
\frac{\partial}{\partial t}\left(\nabla\times\mathbf j+\epsilon_0\omega_p^2\mathbf B\right)=0.
$$

For an initially field-free, current-free preparation, the integration constant is zero. Equivalently, impose the second [London equation](../../../../../london-equations.md) appropriate to the [Meissner state](../../../../../meissner-state.md), $\nabla\times\mathbf j=-\epsilon_0\omega_p^2\mathbf B$. In the final static state, [Ampère's law](../../../../../ampere-s-circuital-law.md) and $\nabla\cdot\mathbf B=0$ then give

$$
-\nabla^2\mathbf B=\mu_0\nabla\times\mathbf j
=-\frac{\omega_p^2}{c^2}\mathbf B,\qquad
\boxed{\lambda_L=\frac c{\omega_p}=\sqrt{\frac{m}{\mu_0nq^2}}}.
$$

For a planar half-space $z>0$ with a tangential surface field, the bounded solution is

$$
\boxed{\mathbf B(z)=\mathbf B(0)e^{-z/\lambda_L}}.
$$

The [plasma-frequency form of London penetration depth](../../../../../plasma-frequency-form-of-london-penetration-depth.md) therefore shows that an applied field is exponentially small several penetration depths inside the material.

The [magnetic-history constant in an undamped plasma](../../../../../magnetic-history-constant-in-an-undamped-plasma.md) explains the required qualification. Undamped carrier motion alone fixes a time-independent value of $\nabla\times\mathbf j+\epsilon_0\omega_p^2\mathbf B$; it does not force that value to vanish. A [perfect conductor](../../../../../perfect-conductor.md) can retain a pre-existing field. The additional [London equation](../../../../../london-equations.md) describes [London screening](../../../../../london-screening.md) independently of that arbitrary ideal-conductor history. The original London paper explicitly distinguishes its description from acceleration theory.[pp. 71–74: acceleration equation, its integration freedom and the additional superconducting relation](../../../../../the-electromagnetic-equations-of-the-supraconductor-by-fritz-london-and-heinz-london.md)

## ↑ Ancestors (14)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
