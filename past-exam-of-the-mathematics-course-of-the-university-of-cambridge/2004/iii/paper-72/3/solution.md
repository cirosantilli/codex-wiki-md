<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Work in the fixed reference domain $\Omega_0$, and write $v_i=\delta x_i$. For the unconstrained [hyperelastic material](../../../../../hyperelastic-material.md) considered here, the material-first [nominal stress](../../../../../nominal-stress-tensor.md) is $N_{\alpha i}=W_{,A_{i\alpha}}$. The increment of the [deformation gradient](../../../../../deformation-gradient.md) and the [incremental elastic moduli](../../../../../incremental-elastic-moduli.md) are

$$
\delta A_{i\alpha}=v_{i,\alpha},\qquad c_{\alpha i\beta j}=\frac{\partial^2W}{\partial A_{i\alpha}\partial A_{j\beta}},\qquad \delta N_{\alpha i}=c_{\alpha i\beta j}v_{j,\beta}.
$$

All coefficients are evaluated at the base deformation. The [Hessian](../../../../../hessian-matrix.md) symmetry is $c_{\alpha i\beta j}=c_{\beta j\alpha i}$; minor interchange symmetry is unnecessary. Linearizing the momentum equation gives

$$
\boxed{(c_{\alpha i\beta j}v_{j,\beta})_{,\alpha}+\rho_0\delta g_i=\rho_0\ddot v_i\quad\text{in }\Omega_0.}
$$

The reference [mass density](../../../../../density.md) and reference outward unit [normal vector](../../../../../normal-vector.md) are fixed, so the incremental boundary conditions are

$$
\boxed{\nu_\alpha c_{\alpha i\beta j}v_{j,\beta}=\delta t_i^0\quad\text{or}\quad v_i=\delta x_i^0.}
$$

In particular, no variation of a current surface normal belongs in this material-coordinate [traction](../../../../../traction.md) condition. If a material constraint were imposed, one would additionally linearize its [constraint reaction in hyperelastic stress](../../../../../constraint-reaction-in-hyperelastic-stress.md) and its admissibility equation; the present moduli formula is the unconstrained one.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 72](../../paper-72-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
