<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\Delta T=T_0-T_B$, $\Delta C=C_0-C_B$ and assume these scales are nonzero. The two reference [liquidus](../../../../liquidus.md) relations imply $\Delta T=-m\Delta C$. For the [similarity variable](../../../../similarity-variable.md) $\eta=z/(2\sqrt{\kappa t})$ and front $h=2\lambda\sqrt{\kappa t}$,

$$
\eta_t=-\frac{\eta}{2t},\quad\eta_z=\frac1{2\sqrt{\kappa t}},\quad h'=\lambda\sqrt{\kappa/t}.
$$

Thus a [temperature](../../../../temperature-split.md) profile $T=T_*+\Delta T\theta(\eta)$ has $T_t=-\Delta T\eta\theta'/(2t)$ and $\kappa T_{zz}=\Delta T\theta''/(4t)$. Each [heat equation](../../../../heat-equation.md) becomes $\theta''+2\eta\theta'=0$. The solute [diffusion equation](../../../../diffusion-equation-split.md) becomes $\mathcal C^{l\prime\prime}+2Le\eta\mathcal C^{l\prime}=0$, with

$$
\boxed{Le=\kappa/D.}
$$

This [Lewis number](../../../../lewis-number.md) compares thermal and solutal [diffusivities](../../../../diffusion-coefficient.md). Inside the [mushy layer](../../../../mushy-layer.md), $T^s-T_B=-m(C^s-C_B)$ gives $\boxed{\mathcal C^s=\theta^s}$. The wall and far-field conditions become $\theta^s(0)=0$ and $\theta^l,\mathcal C^l\to0$ as $\eta\to\infty$.

At the moving [phase boundary](../../../../phase-boundary.md), equality of [temperatures](../../../../temperature-split.md) gives $\theta^s=\theta^l+(T_\infty-T_B)/\Delta T$. Equality of [concentrations](../../../../concentration.md) gives $\mathcal C^s=\mathcal C^l+1$. Therefore the dimensionless parameters with the convention used here are

$$
\boxed{\mathcal R_\theta=\frac{T_0-T_\infty}{T_0-T_B},\qquad \mathcal R_C=\frac{C_0}{C_0-C_B},\qquad S=\frac{\rho L\kappa}{k(T_0-T_B)}.}
$$

Neither [concentration](../../../../concentration.md) nor [temperature](../../../../temperature-split.md) offsets should be dropped when enforcing continuity. In particular $\mathcal R_\theta$ can be negative. If $k=\rho c_p\kappa$, then $S=L/[c_p\Delta T]$: this is the [inverse Stefan number](../../../../latent-to-sensible-heat-ratio.md), although the paper calls $S$ its Stefan number.

To check every factor of two in the flux conditions, divide the thermal [Stefan condition](../../../../stefan-condition.md) by $k\Delta T/(2\sqrt{\kappa t})$, and the solute balance by $D\Delta C/(2\sqrt{\kappa t})$. This gives

$$
\boxed{2\phi\lambda S=\theta^{s\prime}-\theta^{l\prime},\qquad 2\phi Le\lambda(\mathcal C^l+\mathcal R_C)=-\mathcal C^{l\prime}.}
$$

Finally $T_z^l=-mC_z^l$ and $-m\Delta C=\Delta T$ imply $\boxed{\theta^{l\prime}=\mathcal C^{l\prime}}$. This is [marginal equilibrium at a mush-liquid boundary](../../../../marginal-equilibrium-at-a-mush-liquid-boundary.md). Together these calculations produce all the rescaled differential equations and all three interface balances.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [3](../../3.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../split.md)
5. [Topics in fluid mechanics course of the University of Oxford](../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
