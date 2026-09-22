<h1 id="j/j2/solution">Solution</h1>

↑ **Parent:** [J2](../j2.md)

In SI units, [Maxwell's equations](../../../../maxwell-equations-split.md) are

$$
\nabla\cdot\mathbf E=\rho_e/\epsilon_0,\quad\nabla\cdot\mathbf B=0,\quad
\nabla\times\mathbf E=-\partial_t\mathbf B,\quad
\nabla\times\mathbf B=\mu_0\mathbf J+\mu_0\epsilon_0\partial_t\mathbf E.
$$

Dotting the last equation with $\mathbf E/\mu_0$, and using the curl equation for $\mathbf E$, gives

$$
\partial_t\left(\frac{\epsilon_0}2|\mathbf E|^2+\frac1{2\mu_0}|\mathbf B|^2\right)
=-\mathbf E\cdot\mathbf J-\frac1{\mu_0}\nabla\cdot(\mathbf E\times\mathbf B).
$$

Integrate over the fixed region and apply the [divergence theorem](../../../../divergence-theorem.md). This proves [Poynting's theorem](../../../../poynting-theorem.md): the rate of increase of electromagnetic [energy](../../../../energy-split.md) stored inside, plus the outward [Poynting flux](../../../../poynting-flux.md), plus the rate of work on charges, is zero. The last term need not be positive for arbitrary externally driven currents; when positive it is power transferred from the [field](../../../../field.md) to matter.

For the travelling wave put $\varphi=kz-\omega t$. A purely oscillatory [magnetic field](../../../../magnetic-field-split.md) satisfying [Faraday's law](../../../../faraday-s-law-of-induction.md) is

$$
\mathbf B=(0,(k\alpha/\omega)\cos\varphi,0).
$$

Both divergences vanish. The [vacuum](../../../../vacuum.md) [Ampère-Maxwell law](../../../../ampere-s-circuital-law.md) then requires $k^2=\mu_0\epsilon_0\omega^2$, so with the positive constants in the question,

$$
\boxed{\omega=ck,\quad c=(\mu_0\epsilon_0)^{-1/2},\quad\mathbf B=(0,(\alpha/c)\cos\varphi,0)}.
$$

A superposed static background is not part of the pure plane-wave solution. The electric and magnetic [energy](../../../../energy-split.md) contributions are equal, giving

$$
\mathcal U=\epsilon_0\alpha^2\cos^2\varphi,\qquad
\mathbf P=\frac{\alpha^2}{\mu_0c}\cos^2\varphi\,\mathbf e_z
=c\mathcal U\,\mathbf e_z.
$$

Consequently $\boxed{|\mathbf P|=c\mathcal U}$ pointwise, including the nodes where both sides vanish.

## ↑ Ancestors (12)

1. [J2](../j2.md)
2. [J](../../j.md)
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
