<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Maxwell construction](../../../../../../maxwell-construction.md) replaces a nonconvex homogeneous [free-energy density](../../../../../../free-energy-density.md) by its coexistence envelope. If $U_0(M)$ excludes the source, the coexisting values $M_1,M_2$ satisfy

$$
U_0'(M_1)=U_0'(M_2)=h_*,\qquad
U_0(M_2)-U_0(M_1)=h_*(M_2-M_1).
$$

Thus one straight line is tangent at both endpoints. Equivalently,

$$
\int_{M_1}^{M_2}[U_0'(M)-h_*]dM=0,
$$

the equal-area form of the [common-tangent construction](../../../../../../common-tangent-construction.md). At fixed average $\overline M$ between the endpoints, the [lever rule](../../../../../../lever-rule.md) gives $\overline M=pM_1+(1-p)M_2$. Such a mixture has the tangent-line bulk energy, below the energy of an unstable homogeneous state.

The two phases occupy spatial domains separated by [domain walls](../../../../../../domain-wall.md). The gradient term gives a positive wall energy, but a macroscopic interface has area of order $L^{D-1}$ rather than bulk volume $L^D$, so its cost per volume vanishes in the [thermodynamic limit](../../../../../../thermodynamic-limit.md). For the symmetric quartic example a [scalar quartic domain wall](../../../../../../scalar-quartic-domain-wall.md) obeys $\kappa\phi''=r\phi+u\phi^3$ and interpolates between $\pm M_0$ as $\phi=M_0\tanh(x/\ell)$, with $M_0^2=|r|/u$ and $\ell=\sqrt{2\kappa/|r|}$. Multiplication of the differential equation by $\phi'$ gives the first integral $\kappa(\phi')^2/2=u(\phi^2-M_0^2)^2/4$, explaining the finite positive interface cost. A uniform unconstrained system need not form both domains: phase separation is particularly relevant when the average [order parameter](../../../../../../order-parameter.md) is fixed or boundaries enforce competing phases.

[Hysteresis](../../../../../../hysteresis.md) occurs when the system follows a [metastable](../../../../../../metastability.md) local minimum after another minimum has become the equilibrium one. For $r<0,u>0$, the equation of state is $h=rM+uM^3$. The [hysteresis spinodals of a scalar quartic potential](../../../../../../hysteresis-spinodals-of-a-scalar-quartic-potential.md) follow from $r+3uM^2=0$:

$$
\boxed{M_{\rm sp}=\pm\sqrt{\frac{|r|}{3u}},\qquad |h_{\rm sp}|=\frac{2|r|^{3/2}}{3\sqrt{3u}}.}
$$

Following local minima until these limits gives different switching fields on increasing and decreasing $h$. Equilibrium instead switches at $h=0$. Actual switching can occur before a mean-field spinodal through nucleation, and depends on time scales; hysteresis is not a property of a globally minimized equilibrium potential. The second panel below distinguishes the local branches and their limiting switches.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
