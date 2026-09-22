<h1 id="4/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For a translation with the sign used in the paper, the field variation at fixed coordinates is $\delta A_\rho=\beta\epsilon^\nu\partial_\nu A_\rho$, and $\delta\mathcal L=\partial_\mu(\beta\epsilon^\mu\mathcal L)$. Differentiating the [Maxwell Lagrangian](../../../../../../maxwell-lagrangian.md) with respect to the field gradient gives

$$
\frac{\partial\mathcal L}{\partial(\partial_\mu A_\rho)}=-F^{\mu\rho}.
$$

Thus [Noether's theorem](../../../../../../noether-conserved-quantity-for-a-mechanical-point-symmetry.md) yields $j^\mu=\epsilon_\nu T^{\mu\nu}$, where the [canonical stress-energy tensor of the Maxwell field](../../../../../../canonical-stress-energy-tensor-of-the-maxwell-field.md) is

$$
\boxed{T^{\mu\nu}=-F^{\mu\rho}\partial^\nu A_\rho-\eta^{\mu\nu}\mathcal L
=-F^{\mu\rho}\partial^\nu A_\rho+\frac14\eta^{\mu\nu}F_{\rho\sigma}F^{\rho\sigma}.}
$$

It is conserved on the source-free [Maxwell equations](../../../../../../maxwell-equations.md), but it is not generally symmetric. Indeed,

$$
T^{\mu\nu}-T^{\nu\mu}
=-F^{\mu\rho}\partial^\nu A_\rho+F^{\nu\rho}\partial^\mu A_\rho
$$

need not vanish. For example, take $A_0=a x^1$, $A_2=b x^0$, and the other components zero, with nonzero constants $a,b$. This produces constant field strength and satisfies the source-free equations, but $T^{12}=0$ and $T^{21}=ab$.

Nor is it [gauge-invariant](../../../../../../gauge-invariance.md): while $F$ and $\mathcal L$ are unchanged, a [gauge transformation](../../../../../../gauge-transformation.md) gives

$$
\boxed{\delta_\xi T^{\mu\nu}=-F^{\mu\rho}\partial^\nu\partial_\rho\xi,}
$$

which is generally nonzero. These shortcomings motivate the improvement in part (vi); they do not contradict conservation of the [canonical stress-energy tensor](../../../../../../canonical-stress-energy-tensor.md).

## ↑ Ancestors (11)

1. [V](../v.md)
2. [4](../../4.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
