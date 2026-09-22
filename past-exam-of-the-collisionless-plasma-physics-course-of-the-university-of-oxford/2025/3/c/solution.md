<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose the [drift-kinetic equation](../../../../drift-kinetic-equation.md) in $(\mathbf r,\mu,v_\parallel)$ with $v_\parallel$ the laboratory parallel [velocity](../../../../velocity.md) along the exact $\mathbf b$. To first order, before discarding terms small in the stated steep-gradient ordering, it is

$$
\begin{aligned}
(-i\omega+ik_\parallel v_\parallel)\delta f_\alpha
&+(u_x+v_\parallel\delta b_x)\partial_x f_{0\alpha}\\
&+\left[\frac{q_\alpha}{m_\alpha}\delta E_\parallel
-\mu(ik_\parallel\delta B+\delta b_xB_0')
+v_\parallel\mathbf u_\perp\cdot\boldsymbol\kappa_0\right]\partial_{v_\parallel}f_{0\alpha}=0,
\qquad\boldsymbol\kappa_0=-\frac{\hat{\mathbf x}}R.
\end{aligned}
$$

The last term is the linear acceleration associated with the moving curved field. Terms quadratic in the perturbations have already been removed. A formulation using parallel [velocity](../../../../velocity.md) relative to the common flow gives the same physical result after transforming back to these variables.

The two mirror terms and the curvature acceleration are subleading here. Their relative sizes are controlled by $h\ll\delta p/p_0$ and $L_p/L_B,L_p/R\ll1$. **The field-direction perturbation multiplying the steep equilibrium [gradient](../../../../gradient.md) must remain:**

$$
\delta(\mathbf b\cdot\nabla f_{0\alpha})=\delta b_x\partial_x f_{0\alpha}.
$$

Using $u_x=-i\omega\xi_x$ and $\delta b_x=ik_\parallel\xi_x$ therefore gives the leading equation

$$
\boxed{(-i\omega+ik_\parallel v_\parallel)(\delta f_\alpha+\xi_x\partial_xf_{0\alpha})
+\frac{q_\alpha}{m_\alpha}\delta E_\parallel\partial_{v_\parallel}f_{0\alpha}=0.}
$$

The displaced branch satisfying [quasineutrality](../../../../quasineutrality.md) has $\delta E_\parallel=0$ to this order: its species [number densities](../../../../number-density.md) are $\delta n_\alpha=-\xi_xn_{0\alpha}'$, so $\sum_\alpha q_\alpha\delta n_\alpha=-\xi_x\partial_x\sum_\alpha q_\alpha n_{0\alpha}=0$. More explicitly, putting $\mathcal D=-i\omega+ik_\parallel v_\parallel$ gives

$$
\delta f_\alpha=-\xi_x f_{0\alpha}'-\frac{iq_\alpha\delta E_\parallel}{m_\alpha}\frac{\partial_{v_\parallel}f_{0\alpha}}{\omega-k_\parallel v_\parallel},\qquad
0=-i\delta E_\parallel\sum_\alpha\frac{q_\alpha^2}{m_\alpha}\int\frac{\partial_{v_\parallel}f_{0\alpha}}{\omega-k_\parallel v_\parallel}\,d^3v.
$$

Away from an independent longitudinal eigenfrequency, the summed susceptibility is nonzero, giving $\delta E_\parallel=0$. An independent longitudinal eigenmode is not forced by the interchange displacement. The required solution is thus

$$
\boxed{\delta f_\alpha=-\xi_x\partial_x f_{0\alpha}.}
$$

The apparent streaming denominator cancels identically, including at $\omega=k_\parallel v_\parallel$; this response has no leading [Landau damping](../../../../landau-damping.md) singularity.

To see the temperature and density contributions explicitly, differentiate at fixed $\mu,v_\parallel$ and neglect $B_0'$ at this order:

$$
\partial_xf_{0\alpha}=f_{0\alpha}\left[\frac{n_{0\alpha}'}{n_{0\alpha}}+
\left(\frac{m_\alpha(v_\parallel^2+2\mu B_0)}{2T_{0\alpha}}-\frac32\right)\frac{T_{0\alpha}'}{T_{0\alpha}}\right].
$$

The gyrotropic [velocity-space measure](../../../../velocity-space-measure.md) is $d^3v=2\pi B_0\,d\mu\,dv_\parallel$. The species [perpendicular plasma pressure](../../../../perpendicular-plasma-pressure.md) and [parallel plasma pressure](../../../../parallel-plasma-pressure.md) are the [moments](../../../../moment.md)

$$
p_{\perp\alpha}=m_\alpha\int\mu B f_\alpha\,d^3v,\qquad
p_{\parallel\alpha}=m_\alpha\int v_\parallel^2 f_\alpha\,d^3v.
$$

Explicit perturbations of the measure and of $\mu B$ produce terms proportional to $h$, which are subleading in these [pressure](../../../../pressure-split.md) moments; derivatives of the equilibrium measure produce the discarded $B_0'$ terms. The remaining [Maxwell-Boltzmann distribution](../../../../maxwell-boltzmann-distribution.md) integrals give

$$
\delta p_{\perp\alpha}=\delta p_{\parallel\alpha}=-\xi_xp_{0\alpha}',\qquad
\boxed{\delta p_\perp=\delta p_\parallel=\frac{p_0}{L_p}\xi_x.}
$$

Insertion into [b](../b.md) proves

$$
\boxed{\omega^2=k_\parallel^2v_A^2-\frac{2p_0}{\rho_0RL_p}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the collisionless plasma physics course of the University of Oxford](../../../split.md)
5. [Collisionless plasma physics course of the University of Oxford](../../../../collisionless-plasma-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
