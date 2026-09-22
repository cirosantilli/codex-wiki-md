<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use complex Fourier amplitudes and let primes denote $z$ derivatives. Put $C=B^2/\mu_0$, $T=\gamma p+C$ and $d=ik_x\xi_x+ik_y\xi_y+\xi_z'$. Static balance gives $(p+B^2/(2\mu_0))'=-\rho g$. The perturbations from part (a) then imply

$$
\delta\rho=-\rho'\xi_z-\rho d,\qquad
\delta B=ik_yB\xi-(B'\xi_z+Bd)e_y,\qquad
\delta\Pi=\rho g\xi_z-Td+Cik_y\xi_y.
$$

For the last identity, combine $\delta p$ with $B\delta B_y/\mu_0$ and use static balance; this is where the background magnetic-pressure gradient cancels.

Multiply the Fourier momentum equation by $-\xi^*$ and integrate from $a$ to $b$. Integrating the pressure-gradient term by parts gives $[\xi_z^*\delta\Pi]_a^b-\int d^*\delta\Pi\,dz$. The gravity term is $\int[-g\rho'|\xi_z|^2-\rho g\xi_z^*d]dz$. The magnetic terms reduce to

$$
\int_a^b[Ck_y^2|\xi|^2+Cik_y\xi_y^*d]dz.
$$

Indeed the term from $\delta B_zB'e_y$ cancels exactly the $B'$ term arising from $ik_yB\delta B$. This establishes, before [completing the square](../../../../../../completing-the-square.md),

$$
\omega^2\int_a^b\rho|\xi|^2dz=[\xi_z^*\delta\Pi]_a^b+
\int_a^b[-d^*\delta\Pi-A^*d+Ck_y^2|\xi|^2-g\rho'|\xi_z|^2]dz,
\quad A=\rho g\xi_z+Cik_y\xi_y.
$$

Now $\delta\Pi=A-Td$, so

$$
-d^*\delta\Pi-A^*d=T|d|^2-2\operatorname{Re}(d^*A)
=\frac{|\delta\Pi|^2-|A|^2}{T}.
$$

Thus the [magnetohydrodynamic energy principle](../../../../../../magnetohydrodynamic-energy-principle.md) has the requested [quadratic form](../../../../../../quadratic-form.md)

$$
\boxed{\omega^2\int_a^b\rho|\xi|^2dz=[\xi_z^*\delta\Pi]_a^b+
\int_a^b\left[\frac{|\delta\Pi|^2}{T}-\frac{|\rho g\xi_z+Cik_y\xi_y|^2}{T}
+Ck_y^2|\xi|^2-g\rho'|\xi_z|^2\right]dz.}
$$

All squares are squared complex moduli. With the prescribed vanishing surface term the [quadratic form](../../../../../../quadratic-form.md) is real, as required for the self-adjoint stability problem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
