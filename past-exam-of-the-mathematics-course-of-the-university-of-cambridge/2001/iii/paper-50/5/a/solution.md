<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the conservative [continuity equation](../../../../../../continuity-equation.md) and momentum balance, with $\sigma_{ij}$ the viscous stress:

$$
\rho_t+\partial_i(\rho u_i)=0,\qquad \partial_t(\rho u_i)+\partial_j(\rho u_iu_j)=-\partial_i p+\partial_j\sigma_{ij}.
$$

Differentiate the first equation in time and take the divergence of the second. Eliminating momentum gives

$$
\rho_{tt}=\partial_i\partial_j(\rho u_iu_j+p\delta_{ij}-\sigma_{ij}).
$$

Subtract $c_0^2\Delta\rho$, and define the [Lighthill stress tensor](../../../../../../lighthill-stress-tensor.md) by

$$
\boxed{T_{ij}=\rho u_iu_j+[(p-p_0)-c_0^2(\rho-\rho_0)]\delta_{ij}-\sigma_{ij}.}
$$

The constant reference subtraction has no double divergence. The exact [Lighthill acoustic analogy](../../../../../../lighthill-acoustic-analogy.md) is

$$
\boxed{(\partial_t^2-c_0^2\Delta)\rho'=\partial_i\partial_jT_{ij},\qquad \rho'=\rho-\rho_0.}
$$

This is an exact rearrangement; linearization is not used to eliminate the nonlinear source tensor.

Convolving with the [retarded acoustic Green function](../../../../../../retarded-acoustic-green-function.md) and transferring the source derivatives by [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\rho'(\mathbf x,t)=\frac1{4\pi c_0^2}\partial_{x_i}\partial_{x_j}\int\frac{T_{ij}(\mathbf y,t-|\mathbf x-\mathbf y|/c_0)}{|\mathbf x-\mathbf y|}\,d^3y.
$$

The [acoustic compact-source approximation](../../../../../../acoustic-compact-source-approximation.md) requires source size $\ell$ to satisfy $\Omega\ell/c_0\ll1$ for its characteristic frequency $\Omega$; the [acoustic far field](../../../../../../acoustic-far-field.md) additionally requires $r\gg\ell$ and $\Omega r/c_0\gg1$. Internal retardation is then negligible at leading order, and the radiating parts of the two observer derivatives act on the common [retarded time](../../../../../../retarded-time.md). With $n_i=x_i/r$ and $S_{ij}=\int T_{ij}\,d^3y$, the [far-field acoustic force and stress moments](../../../../../../far-field-acoustic-force-and-stress-moments.md) give

$$
\boxed{\rho'(\mathbf x,t)\sim\frac{n_in_j}{4\pi c_0^4r}\ddot S_{ij}(t-r/c_0).}
$$

The two spatial derivatives supply two factors of $1/c_0$, in addition to the $1/c_0^2$ in the Green function.

For a subsonic fluctuating source of velocity scale $V$, size $\ell$ and turnover time $\ell/V$, suppose its stress scale is $T_{ij}=O(\rho_0V^2)$. Then $S_{ij}=O(\rho_0V^2\ell^3)$ and $\ddot S_{ij}=O(\rho_0V^4\ell)$. The [compact acoustic quadrupole Mach-number scaling](../../../../../../compact-acoustic-quadrupole-mach-number-scaling.md) is therefore

$$
\boxed{\frac{\rho'}{\rho_0}=O\left(\frac\ell r\left(\frac V{c_0}\right)^4\right)=O((\ell/r)m^4).}
$$

This fourth-power statement concerns the acoustic density amplitude under the specified eddy-time and stress scaling. With an independently imposed frequency, the general estimate instead retains $V^2\Omega^2\ell^3/c_0^4r$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
