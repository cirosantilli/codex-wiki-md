<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $b=\frac12u^2+\Phi+w$. Because the [specific entropy](../../../../../../specific-entropy.md) is constant along the horizontal flow, the [specific enthalpy](../../../../../../specific-enthalpy.md) identity gives $\mathbf u\cdot\nabla w=\rho^{-1}\mathbf u\cdot\nabla p$. Dotting the [ideal magnetohydrodynamic momentum equation](../../../../../../ideal-magnetohydrodynamic-momentum-equation.md) with $\mathbf u$ therefore gives

$$
\rho\mathbf u\cdot\nabla b=\frac1{\mu_0}\mathbf u\cdot[(\nabla\times\mathbf B)\times\mathbf B].
$$

On the field-aligned horizontal branch, $\mathbf u\times\mathbf B=U\mathbf e_z\times\mathbf B$. Directly evaluating the horizontal components of the curl gives

$$
(\nabla\times\mathbf B)\cdot(\mathbf e_z\times\mathbf B)=-\mathbf B_h\cdot\nabla B_z.
$$

The scalar triple-product identity consequently makes the magnetic work $U\mathbf B_h\cdot\nabla B_z/\mu_0$. Meanwhile $\rho\mathbf u\cdot\nabla b=k\mathbf B_h\cdot\nabla b$. The previously established field-line constancy of $U,k$ now gives the [planar ideal-MHD Bernoulli invariant](../../../../../../planar-ideal-mhd-bernoulli-invariant.md)

$$
\boxed{\mathbf B\cdot\nabla Q=0,\qquad Q=\frac12u^2+\Phi+w-\frac{UB_z}{\mu_0k}}.
$$

This is conservation of total energy transported along a [magnetic field line](../../../../../../magnetic-field-line.md), including electromagnetic work. To see its flux interpretation, the [ideal magnetohydrodynamic energy conservation](../../../../../../ideal-magnetohydrodynamic-energy-conservation.md) law has flux

$$
\mathbf F=\rho\mathbf u\left(\frac12u^2+\Phi+w\right)+\frac1{\mu_0}\left[B^2\mathbf u-(\mathbf u\cdot\mathbf B)\mathbf B\right].
$$

The second term is the [Poynting vector](../../../../../../poynting-vector.md), since $\mathbf E=-\mathbf u\times\mathbf B$. Substitution of $\mathbf u=k\mathbf B/\rho+U\mathbf e_z$ gives

$$
\boxed{\mathbf F_h=k\mathbf B_hQ}.
$$

The steady divergence of this horizontal energy flux is zero. Magnetic stress can change the ordinary hydrodynamic quantity $b$ in the [Bernoulli equation](../../../../../../bernoulli-equation.md) by doing work; the term $-UB_z/(\mu_0k)$ accounts for the accompanying Poynting flux. When $U=0$, the velocity is completely field-aligned, $\mathbf E=0$, and the usual hydrodynamic Bernoulli quantity is constant. These conclusions require the field-aligned branch and $k\ne0$; the arbitrary constant-$E_z$ flow from the first part is not covered by this particular invariant.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
