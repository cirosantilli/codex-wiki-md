<h1 id="section-a-iii/19/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the [hydraulic ladder network](../../../../../../hydraulic-ladder-network.md), using the frontier star just defined, start at a single groove with $(x_1,y_1,z_1)=(0,0,R_g)$. Put $B=y_n+R_c$, $C=z_n+R_c$ and $S=B+C+R_g$. The exact update is

$$
\boxed{x_{n+1}=x_n+\frac{BC}{S},\qquad y_{n+1}=\frac{BR_g}{S},\qquad z_{n+1}=\frac{CR_g}{S}.}
$$

After all grooves have been included, the left frontier is a blind end, so no external flow passes through $y_N$. The inlet-to-outlet resistance is **$R_N=x_N+z_N$**. Iterate 49 times to obtain $R_{50}$.

An equivalent closed form, for $R_c,R_g>0$, is

$$
\boxed{R_N=\frac{(N-1)R_c}{2}+\frac{R_c}{\alpha+\sinh\kappa\,\tanh[(N-1)\kappa/2]},\quad \alpha=\frac{R_c}{R_g},\quad\cosh\kappa=1+\alpha.}
$$

Thus substitute $N=50$; no single number follows without $R_c/R_g$. Checks are $R_1=R_g$, $R_2=(R_g+R_c)/2$, and $R_N\to R_g/N$ as $R_c\to0$. The formula counts only the $N-1$ inter-groove segments in each rail; extra inlet/outlet lead resistances, if present, must be added separately. All elements obey linear laminar-flow pressure-drop laws.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [19](../../19.md)
3. [Section A(iii)](../../../section-a-iii.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../split.md)
7. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
