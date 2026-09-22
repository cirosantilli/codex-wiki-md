<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

Expand the state in the [energy eigenstates](../../../../../energy-eigenstate.md) of $H_0$ as

$$
|\psi(t)\rangle=\sum_kc_k(t)e^{-iE_kt/\hbar}|k\rangle.
$$

Substitution into the [Time-dependent Schrödinger equation](../../../../../time-dependent-schrodinger-equation.md) and projection onto $\langle k|$ gives the exact [interaction picture](../../../../../interaction-picture.md) equations

$$
i\hbar\dot c_k(t)=\sum_jc_j(t)e^{i(E_k-E_j)t/\hbar}\langle k|\Delta(t)|j\rangle.
$$

In first-order [time-dependent perturbation theory](../../../../../time-dependent-perturbation-theory.md), put $c_j(t)=\delta_{j0}$ on the right-hand side and integrate from $0$ to $t$:

$$
\boxed{c_k(t)=\frac1{i\hbar}\int_0^t
\langle k|\Delta(t')|0\rangle e^{i(E_k-E_0)t'/\hbar}\,dt'.}
$$

For a uniform [electric field](../../../../../electric-field.md), the [electric-dipole interaction](../../../../../electric-dipole-interaction.md) is $\Delta(t)=e\mathcal E_0ze^{-t/\tau}$ up to an irrelevant overall sign. The supplied [hydrogen atom](../../../../../hydrogen-atom.md) wavefunctions give

$$
\begin{aligned}
\langle210|z|100\rangle
&=\frac1{4\sqrt2\pi a_0^3}
\int_0^\infty\frac{r^4}{a_0}e^{-3r/(2a_0)}\,dr
\int\cos^2\theta\,d\Omega\\
&=\frac{2^8}{3^5\sqrt2}a_0.
\end{aligned}
$$

For $t\gg\tau$, the time integral is

$$
\int_0^\infty e^{-t/\tau+i\omega t}\,dt=\frac1{\tau^{-1}-i\omega}.
$$

The long-time transition fraction is consequently

$$
\boxed{|c_{210}(\infty)|^2
=\frac{2^{15}}{3^{10}}
\frac{e^2\mathcal E_0^2a_0^2}{\hbar^2(\omega^2+\tau^{-2})}.}
$$

Both $|100\rangle$ and $|200\rangle$ have even [parity](../../../../../parity.md), whereas $z$ is odd, so the [electric-dipole selection rule](../../../../../electric-dipole-selection-rule.md) gives $\langle200|z|100\rangle=0$. Thus the requested fraction in $|200\rangle$ is **zero**.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
