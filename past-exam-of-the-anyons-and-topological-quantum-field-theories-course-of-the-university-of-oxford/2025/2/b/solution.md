<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $K=\sum_aN_aN_{\bar a}$. The [Verlinde formula](../../../../verlinde-formula.md) diagonalizes every [anyon fusion matrix](../../../../anyon-fusion-matrix.md) using the same [modular S-matrix](../../../../modular-s-matrix.md):

$$
N_a=S\,\operatorname{diag}_x\left(\frac{S_{ax}}{S_{1x}}\right)S^\dagger.
$$

Because $S_{\bar a x}=S_{ax}^*$, the [eigenvalue](../../../../eigenvalue.md) of $K$ in column $x$ is

$$
\kappa_x=\sum_a\frac{S_{ax}S_{\bar a x}}{S_{1x}^2}=\frac{\sum_a|S_{ax}|^2}{S_{1x}^2}=\frac1{S_{1x}^2}.
$$

The last equality uses [unitary matrix](../../../../unitary-matrix.md) orthogonality. Therefore

$$
(K^g)_{11}=\sum_x|S_{1x}|^2\kappa_x^g=\sum_xS_{1x}^{2-2g}.
$$

Finally, insert $S_{1x}=d_x/\mathcal D$, where $d_x$ is the [quantum dimension](../../../../quantum-dimension.md) and $\mathcal D^2=\sum_xd_x^2$ is the squared [total quantum dimension](../../../../total-quantum-dimension.md):

$$
\boxed{\operatorname{GSD}(\Sigma_g)=\mathcal D^{2g-2}\sum_xd_x^{2-2g}=\left(\sum_xd_x^2\right)^{g-1}\sum_xd_x^{2-2g}.}
$$

Although only [quantum dimensions](../../../../quantum-dimension.md) remain, the result is an integer because [a](../a.md) counts an [anyon fusion space](../../../../anyon-fusion-space.md).

The [sphere](../../../../sphere.md) value is $\mathcal D^{-2}\sum_xd_x^2=1$, and the [torus](../../../../torus.md) value is $\sum_x1$. If all $n$ simple [anyons](../../../../anyon.md) have [quantum dimension](../../../../quantum-dimension.md) one, the answer is $n^g$, agreeing with the Abelian handle count. These checks also fix the exponent $2g-2$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the anyons and topological quantum field theories course of the University of Oxford](../../../split.md)
5. [Anyons and topological quantum field theories course of the University of Oxford](../../../../anyons-and-topological-quantum-field-theories-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
