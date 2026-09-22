<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With no mean flow and constant isotropic coefficients, the [mean-field dynamo](../../../../../../mean-field-dynamo.md) equation is

$$
\partial_t\overline{\mathbf B}=\alpha\nabla\times\overline{\mathbf B}+\eta_T\nabla^2\overline{\mathbf B},\qquad \nabla\cdot\overline{\mathbf B}=0,\qquad \eta_T=\eta+\beta>0.
$$

If the symbol $\beta$ already denotes the total diffusivity in the chosen mean-field convention, replace $\eta_T$ by $\beta$. Let $\nabla\times\mathbf B_0=\kappa\mathbf B_0$. This [Beltrami field](../../../../../../beltrami-field.md) is [solenoidal](../../../../../../solenoidal-vector-field.md) for $\kappa\ne0$, and taking its [curl](../../../../../../curl.md) again gives $\nabla^2\mathbf B_0=-\kappa^2\mathbf B_0$. Thus

$$
\boxed{\overline{\mathbf B}(\mathbf x,t)=e^{st}\mathbf B_0(\mathbf x),\qquad s=\alpha\kappa-\eta_T\kappa^2.}
$$

For example, $\mathbf B_0=(\cos kz,-\sin kz,0)$ has $\kappa=k$, whereas reversing the sine sign gives $\kappa=-k$. Choose the helicity sign to agree with $\alpha$. The [homogeneous alpha-squared dynamo growth criterion](../../../../../../homogeneous-alpha-squared-dynamo-growth-criterion.md) is then

$$
\boxed{0<|\kappa|<\frac{|\alpha|}{\eta_T}.}
$$

On an unbounded or suitably periodic domain with freely selectable [wavenumber](../../../../../../wavenumber.md), this gives exponentially growing modes for every $\alpha\ne0$. Maximizing their [growth rate](../../../../../../growth-rate.md) gives $\kappa_* =\alpha/(2\eta_T)$ and $s_{\max}=\alpha^2/(4\eta_T)$. In a specified bounded domain, the permitted modes and boundary conditions impose a threshold; the optimal wavelength must also remain large compared with the turbulent scale for [mean-field electrodynamics](../../../../../../mean-field-electrodynamics.md) to apply.

**A nonzero alpha effect is necessary in this constant-coefficient model.** If $\alpha=0$, the mean equation is pure diffusion and the claimed growing modes do not exist. Positivity of $\beta$ alone does not imply growth.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
