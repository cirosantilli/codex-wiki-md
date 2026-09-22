<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A spherical bubble displaces liquid volume $4\pi a^3/3$. Neglect its own weight compared with the liquid [buoyancy](../../../../buoyancy.md), as required by the stated gas/liquid approximation. Equating $4\pi a^3\rho_lg/3$ with the quadratic drag gives

$$
\boxed{(u_1-u_2)|u_1-u_2|=\frac{4ag}{3C_D}.}
$$

Retaining a nonnegligible [gas density](../../../../gas-density.md) would add the factor $1-\rho_g/\rho_l$. Let $V_s=\sqrt{4ag/(3C_D)}>0$, so the upward slip is $u_1-u_2=V_s$.

With constant phase densities, adding the two volume balances gives $\partial_x[\alpha u_1+(1-\alpha)u_2]=0$. The closed lower end fixes the total volume flux to zero. Solving it together with the slip relation yields

$$
\boxed{u_1=V_s(1-\alpha),\quad u_2=-V_s\alpha,\quad\alpha_t+V_s[\alpha(1-\alpha)]_x=0.}
$$

Individual bubbles move upward for $0\leq\alpha<1$, while small phase-fraction disturbances move at the [characteristic speed](../../../../characteristic-speed.md) $q'(\alpha)=V_s(1-2\alpha)$. The latter is negative when $\alpha>1/2$: wave speed and bubble speed are different quantities.

A cleared region starts at the closed bottom, with $\alpha_L=0$ and $\alpha_R=3/4$. Its [Rankine-Hugoniot condition](../../../../rankine-hugoniot-conditions.md) speed is $[q]/[\alpha]=V_s/4$. The intended clearing solution is therefore

$$
\boxed{\alpha(x,t)=\begin{cases}0,&0<x<V_st/4,\\3/4,&V_st/4<x<1,\end{cases}\qquad0<t<4/V_s.}
$$

It is an [entropy shock](../../../../entropy-shock.md) for the concave [conservation law flux](../../../../conservation-law-flux.md), since $q'(0)=V_s>V_s/4>q'(3/4)=-V_s/2$. Its speed also equals the bubble speed on its uncleared side, so it follows the last layer of bubbles. Under this continuation the last bubble reaches the outlet when

$$
\boxed{t_{\rm clear}=\frac4{V_s}=\sqrt{\frac{12C_D}{ag}},}
$$

after which $\alpha=0$ throughout the pipe.

There is a boundary qualification for this dense initial mixture. The [characteristics](../../../../characteristic-of-a-field.md) in the uncleared state point into the pipe from the top. To continue the displayed solution all the way to the stated clearance time, its incoming top trace must remain $\alpha(1^-,t)=3/4$ until clearing. Initial [characteristics](../../../../characteristic-of-a-field.md) alone cover the [shock](../../../../shock-wave.md) only until $t=4/(3V_s)$, when its backward right-state [characteristic](../../../../characteristic-of-a-field.md) first meets the top boundary. Atmospheric pressure by itself is not a [boundary condition](../../../../boundary-condition.md) for this scalar phase-fraction equation. Thus the displayed formula and printed clearance time give the intended maintained-trace branch; a different top phase-fraction closure could change the later evolution. This is the [incoming boundary condition in dense bubble clearing](../../../../incoming-boundary-condition-in-dense-bubble-clearing.md), and is separate from the local derivation of the [conservation law](../../../../conservation-law.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../split.md)
5. [Topics in fluid mechanics course of the University of Oxford](../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
