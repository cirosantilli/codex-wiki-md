<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Set $A_i=m_i\omega_i^2/2$, so $V_i=A_ir^2$, and $D=U_{11}U_{22}-U_{12}^2$. In the overlap region, the [Thomas–Fermi approximation for a condensate](../../../../../../thomas-fermi-approximation-for-a-condensate.md) neglects the [gradient](../../../../../../gradient.md) terms and requires

$$
\begin{pmatrix}U_{11}&U_{12}\\U_{12}&U_{22}\end{pmatrix}
\begin{pmatrix}n_1\\n_2\end{pmatrix}
=\begin{pmatrix}\mu_1-A_1r^2\\\mu_2-A_2r^2\end{pmatrix}.
$$

Inverting this [matrix](../../../../../../matrix.md) proves the unambiguous profiles

$$
\boxed{n_1=\frac{U_{22}\mu_1-U_{12}\mu_2-(U_{22}A_1-U_{12}A_2)r^2}{D},}
$$



$$
\boxed{n_2=\frac{U_{11}\mu_2-U_{12}\mu_1-(U_{11}A_2-U_{12}A_1)r^2}{D}.}
$$

Using $R_i^2=\mu_i/A_i$ and introducing

$$
\boxed{\lambda=\frac{A_2}{A_1}=\frac{m_2\omega_2^2}{m_1\omega_1^2},}
$$

these [Thomas–Fermi profiles for unequal condensate trap curvatures](../../../../../../thomas-fermi-profiles-for-unequal-condensate-trap-curvatures.md) become

$$
n_1=\frac{\mu_1/U_{11}}{1-U_{12}^2/(U_{11}U_{22})}
\left[1-\frac{U_{12}\mu_2}{U_{22}\mu_1}
-\frac{r^2}{R_1^2}\left(1-\lambda\frac{U_{12}}{U_{22}}\right)\right],
$$



$$
n_2=\frac{\mu_2/U_{22}}{1-U_{12}^2/(U_{11}U_{22})}
\left[1-\frac{U_{12}\mu_1}{U_{11}\mu_2}
-\frac{r^2}{R_2^2}\left(1-\frac1\lambda\frac{U_{12}}{U_{11}}\right)\right].
$$

There is a genuine printed error: the PDF puts $\lambda$ rather than $1/\lambda$ in the second bracket as well. In the first bracket its coefficient requires $\lambda=A_2/A_1$, while in the second it requires $\lambda=A_1/A_2$; for nonzero cross-coupling these cannot both hold unless the curvatures are equal. The TeX additionally drops both occurrences of $\lambda$. The matrix-inverse formulas above give the corrected general answer directly.

For example, $U_{11}=U_{22}=1$, $U_{12}=1/2$, $\mu_1=\mu_2=2$, $A_1=1$, $A_2=2$ give the physical overlap profiles $n_1=4/3$, $n_2=4/3-2r^2$. Using $\lambda=2$ in both printed brackets would instead give $n_2=4/3$, which fails the second equilibrium equation at every $r\ne0$ in the overlap region.

Only the region where both computed densities are positive belongs to this overlap solution. Beyond its edge, a remaining species has $n_i=(\mu_i-A_ir^2)/U_{ii}$ where positive, and both vanish outside the support; simply retaining negative values from the coupled inverse is unphysical. The actual [chemical potentials](../../../../../../chemical-potential.md) are determined by the two normalization integrals. If the reference uncoupled radii are defined at the coupled solution's chemical potentials, the identities $R_i^2=\mu_i/A_i$ are algebraic scales, not the actual interacting-cloud edges; holding particle numbers fixed and removing cross-coupling generally changes those chemical potentials. The approximation also fails in the healing regions at the edges.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
