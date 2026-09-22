<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the horizontal velocity amplitudes as $(u,v)$ and magnetic amplitudes as $(b_x,b_y)$. The perturbation is horizontally uniform, divergence-free, and has no vertical velocity, so the unperturbed density and pressure are consistent at linear order. In the [Keplerian shearing sheet](../../../../../../keplerian-shearing-sheet.md), the horizontal components of the [linearized ideal magnetohydrodynamic equations](../../../../../../linearized-ideal-magnetohydrodynamic-equations.md) are

$$
su-2\Omega v=\frac{v_A^2}{h}\frac{F''}{ikF}b_x,\qquad
sv+\frac\Omega2u=\frac{v_A^2}{h}\frac{F''}{ikF}b_y.
$$

Use the undivided equations at a zero of $F$. If $F''=-k^2hF$, the magnetic-force coefficient becomes $ikv_A^2$; the stratification cancels. The [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) similarly reduces to

$$
sb_x=iku,\qquad sb_y=-\frac32\Omega b_x+ikv.
$$

The azimuthal induction term is field stretching by the background [differential rotation](../../../../../../differential-rotation.md). The four amplitudes obey the homogeneous system

$$
\begin{pmatrix}
s&-2\Omega&-ikv_A^2&0\\
\Omega/2&s&0&-ikv_A^2\\
-ik&0&s&0\\
0&-ik&3\Omega/2&s
\end{pmatrix}
\begin{pmatrix}u\\v\\b_x\\b_y\end{pmatrix}=0.
$$

Its [determinant](../../../../../../determinant.md) must vanish for a nonzero [normal mode](../../../../../../normal-mode.md). Put $A=v_A^2k^2$. For nonzero $s$, elimination first gives $(s^2+A)u-2\Omega sv=0$ and $s(s^2+A)v+\Omega(s^2-3A)u/2=0$, whose solvability condition is $(s^2+A)^2+\Omega^2(s^2-3A)=0$. The original determinant extends the same polynomial to marginal $s=0$. Thus

$$
\boxed{s^4+(\Omega^2+2v_A^2k^2)s^2+v_A^2k^2(v_A^2k^2-3\Omega^2)=0.}
$$

This is the [ideal magnetorotational dispersion relation](../../../../../../ideal-magnetorotational-dispersion-relation.md) with the midplane [Alfvén speed](../../../../../../alfven-speed.md) $v_A=B_0/\sqrt{4\pi\rho_0}$. The vertical structure enters through the admissible eigenvalues $k$, rather than through a different horizontal dispersion polynomial. No division by a vanishing growth rate is required in the determinant derivation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
