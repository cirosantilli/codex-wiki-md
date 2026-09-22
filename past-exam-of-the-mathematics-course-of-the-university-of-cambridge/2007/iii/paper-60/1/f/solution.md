<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The individual rates describe [population relaxation](../../../../../../population-relaxation.md): $\gamma_{12}$ transfers population from level one to level two, and $\gamma_{21}$ transfers it back. With $p_1+p_2=1$ and the conventional qubit coordinate $r_z=p_1-p_2$,

$$
\dot p_1=-\gamma_{12}p_1+\gamma_{21}p_2,\qquad \dot r_z=-(\gamma_{12}+\gamma_{21})r_z+(\gamma_{21}-\gamma_{12}).
$$

Thus $T_1^{-1}=\gamma_{12}+\gamma_{21}$ is the longitudinal relaxation rate. The parameter $\Gamma=T_2^{-1}$ is the [transverse relaxation](../../../../../../transverse-relaxation.md) rate: it damps the off-diagonal coherence, or the $x,y$ components of the [Bloch vector](../../../../../../bloch-vector.md). In the usual completely positive two-level model,

$$
\Gamma=\frac12(\gamma_{12}+\gamma_{21})+\gamma_\phi,\qquad\gamma_\phi\geq0,
$$

so $\Gamma$ includes both the coherence loss caused by [population relaxation](../../../../../../population-relaxation.md) and additional pure [dephasing](../../../../../../dephasing-channel.md).

There is a normalization switch in the displayed qubit [Affine Bloch equation](../../../../../../affine-bloch-equation.md). Its constant term is appropriate to the conventional [Pauli matrices](../../../../../../pauli-matrices.md) and unit-radius coordinate $r_k=\operatorname{Tr}(\rho\sigma_k^{\mathrm{Pauli}})$. With the orthonormal generators used earlier, $s=r/\sqrt2$, the same physical rates would instead give a constant term $(\gamma_{21}-\gamma_{12})/\sqrt2$. The drift matrix is unchanged. We interpret the supplied qubit equation in its conventional $r$ coordinates.

With zero controls and $g=\gamma_{12}+\gamma_{21}>0$, $\Gamma>0$, the [steady state](../../../../../../steady-state.md) is unique:

$$
\boxed{r_*=(0,0,(\gamma_{21}-\gamma_{12})/g),\qquad \rho_* =\operatorname{diag}(\gamma_{21}/g,\gamma_{12}/g).}
$$

The earlier normalized vector is $s_*=r_*/\sqrt2$. Indeed $r_x,r_y$ decay as $e^{-\Gamma t}$ and $r_z-r_{*,z}$ as $e^{-gt}$.

For vanishing rates, the full equilibrium conditions of the [Affine Bloch equation](../../../../../../affine-bloch-equation.md) are $\Gamma r_x=\Gamma r_y=0$ and $g r_z=\gamma_{21}-\gamma_{12}$, together with $\|r\|\leq1$. In particular, for nonnegative rates, $g=0$ means both population rates vanish. If then $\Gamma>0$, all diagonal [density operators](../../../../../../density-matrix.md) are stationary; if also $\Gamma=0$, every [density operator](../../../../../../density-matrix.md) is stationary. The formal case $g>0$, $\Gamma=0$ permits extra transverse equilibrium coordinates, but is excluded by the completely positive rate bound above.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
