<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\omega\ne0$, substitution of the [separated solutions](../../../../../../separated-solution.md) into the [heat equations](../../../../../../heat-equation.md) gives

$$
G_i''+\omega^2\alpha_i^2G_i=0,\qquad
\alpha_i=\sqrt{\frac{\rho_ic_i}{k_i}}.
$$

The zero exterior [boundary values](../../../../../../boundary-value.md) are incorporated by

$$
G_1(x)=A\sin[\omega\alpha_1(x+L)],\qquad
G_2(x)=B\sin[\omega\alpha_2(L-x)].
$$

To obtain a [eigenvalue equation for heat conduction in two joined slabs](../../../../../../eigenvalue-equation-for-heat-conduction-in-two-joined-slabs.md), write $u=\omega\alpha_1L$ and $v=\omega\alpha_2L$. Continuity of [temperature](../../../../../../temperature-split.md) and [heat flux](../../../../../../heat-flux-density.md) at zero gives the homogeneous [linear system](../../../../../../system-of-linear-equations.md)

$$
A\sin u-B\sin v=0,\qquad
k_1\alpha_1A\cos u+k_2\alpha_2B\cos v=0.
$$

A nonzero amplitude pair exists precisely when its [determinant](../../../../../../determinant.md) vanishes, equivalently

$$
\boxed{D(\omega):=k_1\alpha_1\cos u\sin v+k_2\alpha_2\sin u\cos v=0,\qquad\omega\ne0.}
$$

If $\cos u\cos v\ne0$, division by $k_1k_2\alpha_1\alpha_2\cos u\cos v$ gives the printed [transcendental equation](../../../../../../transcendental-equation.md)

$$
\boxed{\frac{\tan(\omega\alpha_1L)}{\alpha_1k_1}
+\frac{\tan(\omega\alpha_2L)}{\alpha_2k_2}=0.}
$$

**The printed necessity claim needs the qualification that both [tangents](../../../../../../tangent.md) are defined.** If just one of $\cos u,\cos v$ vanishes, $D(\omega)\ne0$. If both [cosines](../../../../../../cosine.md) vanish, however, $D(\omega)=0$ and legitimate [normal modes](../../../../../../normal-mode.md) remain. Their [temperature](../../../../../../temperature-split.md) at the [thermal interface](../../../../../../thermal-interface.md) need not be zero; the [temperature](../../../../../../temperature-split.md) condition fixes the amplitude ratio, while each [heat flux](../../../../../../heat-flux-density.md) is zero there.

For a concrete counterexample, take identical slabs: $\rho_1=\rho_2=\rho$, $c_1=c_2=c$, $k_1=k_2=k$, and $\alpha=\sqrt{\rho c/k}$. Then

$$
\boxed{T_1(x,t)=T_2(x,t)=e^{-\omega^2t}\cos\frac{\pi x}{2L},\qquad
\omega=\frac{\pi}{2\alpha L},}
$$

with each formula restricted to its own slab, satisfies both [heat equations](../../../../../../heat-equation.md) and all four [boundary conditions](../../../../../../boundary-condition.md). But $\omega\alpha L=\pi/2$, so neither [tangent](../../../../../../tangent.md) is defined. This directly disproves the unqualified printed assertion. The [determinant](../../../../../../determinant.md) condition retains these missing [normal modes](../../../../../../normal-mode.md).

Finally, $\omega=0$ must be checked before dividing by it. Then $G_1=A(x+L)$, $G_2=B(L-x)$, and interface continuity gives $A=B$, while [heat flux](../../../../../../heat-flux-density.md) continuity gives $k_1A=-k_2B$. Positivity of the [thermal conductivities](../../../../../../thermal-conductivity.md) forces $A=B=0$. Thus $\boxed{\omega=0\text{ gives only the trivial solution}.}$ In the [determinant](../../../../../../determinant.md) formula, its apparent zero at $\omega=0$ is spurious because the chosen sine basis degenerates there.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
