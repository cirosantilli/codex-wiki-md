<h1 id="a4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The nine-atom nonlinear ion has **$3N-6=21$ vibrational degrees of freedom**. To construct its displacement [group representation](../../../../../../group-representation.md), only atoms left in place by an operation contribute to the [character](../../../../../../character-of-a-representation.md). Each such atom contributes the trace of the operation on $(x,y,z)$:

$$
\chi_{3N}(R)=N_{\rm fixed}(R)\,\operatorname{tr}D_{xyz}(R).
$$

For example, reflection in the square's molecular plane fixes all nine atoms and has trace $1$, giving character $9$; inversion fixes nickel alone and has trace $-3$, giving $-3$. [Molecular character reduction](../../../../../../molecular-character-reduction.md) uses

$$
n_\lambda=\frac1{|G|}\sum_C |C|\,\chi_{3N}(C)\chi_\lambda(C)^*.
$$

For the [D4h molecular point group](../../../../../../d4h-molecular-point-group.md), with primed twofold axes along the Ni–C directions, the class order and displacement characters are

$$
\begin{array}{c|rrrrrrrrrr}
C&E&2C_4&C_2&2C_2'&2C_2''&i&2S_4&\sigma_h&2\sigma_v&2\sigma_d\\\hline
\chi_{3N}&27&1&-1&-5&-1&-3&-1&9&5&1
\end{array}
$$

Reducing and removing translations $A_{2u}+E_u$ and rotations $A_{2g}+E_g$ gives

$$
\boxed{\Gamma_{\rm vib}^{D_{4h}}
=2A_{1g}+A_{2g}+2B_{1g}+2B_{2g}+E_g
+2A_{2u}+2B_{2u}+4E_u.}
$$

The [vibrational infrared activity](../../../../../../vibrational-infrared-activity.md) belongs to $2A_{2u}+4E_u$, giving **six features**. The [Raman vibrational activity](../../../../../../raman-vibrational-activity.md) belongs to $2A_{1g}+2B_{1g}+2B_{2g}+E_g$, giving **seven features**. The remaining $A_{2g}+2B_{2u}$ modes are silent. There are **zero shared fundamentals**, by [infrared and Raman mutual exclusion](../../../../../../infrared-and-raman-mutual-exclusion.md). Counting dimensions gives $10$ IR-active, $8$ Raman-active and $3$ silent vibrational coordinates, totaling $21$.

For the [Td molecular point group](../../../../../../td-molecular-point-group.md), the corresponding calculation starts from

$$
\begin{array}{c|rrrrr}
C&E&8C_3&3C_2&6S_4&6\sigma_d\\\hline
\chi_{3N}&27&0&-1&-1&5
\end{array}
$$

and gives $\Gamma_{3N}=2A_1+2E+2T_1+5T_2$. Subtracting translations $T_2$ and rotations $T_1$ leaves

$$
\boxed{\Gamma_{\rm vib}^{T_d}=2A_1+2E+T_1+4T_2.}
$$

The $4T_2$ fundamentals give **four IR features**. The $2A_1+2E+4T_2$ fundamentals give **eight Raman features**, of which **four coincide with the IR features**. The $T_1$ fundamental is silent. The dimensions are $2+4+3+12=21$.

Thus the predicted IR/Raman/coincidence counts are **$6/7/0$ for the square and $4/8/4$ for the tetrahedron**. These are numbers of distinct ideal fundamental frequencies: each $E$ or $T$ multiplet contributes one feature, and different copies of the same [irreducible representation](../../../../../../irreducible-representation.md) generally have different frequencies. Accidental degeneracy, overtones and combination bands are outside this count.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [A4](../../../a4.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the chemistry A course of the University of Cambridge](../../../../../split.md)
7. [Chemistry A course of the University of Cambridge](../../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
