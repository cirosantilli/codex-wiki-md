<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Saturation equation.** Introduce intrinsic [permeability of a porous medium](../../../../../permeability-of-a-porous-medium.md) $K$ and [porosity](../../../../../porosity.md) $\phi$. The relative [porous permeabilities](../../../../../permeability-of-a-porous-medium.md) depend on the wetting [fluid saturation](../../../../../fluid-saturation.md). Define the [phase mobilities](../../../../../phase-mobility.md) and [fractional flow](../../../../../fractional-flow.md)

$$
\lambda_w(s)=\frac{k_w(s)}{\mu_w},\qquad
\lambda_n(s)=\frac{k_{nw}(s)}{\mu_{nw}},\qquad
F(s)=\frac{\lambda_w}{\lambda_w+\lambda_n}.
$$

Use the conventional [capillary pressure](../../../../../capillary-pressure.md) $p_c=p_{nw}-p_w$, generally decreasing as wetting saturation increases. Neglect gravity in this horizontal model. The two [Darcy fluxes](../../../../../darcy-velocity.md) are $q_w=-K\lambda_wp_{w,x}$ and $q_n=-K\lambda_n(p_{w,x}+p_c'(s)s_x)$. Eliminate the common pressure gradient using $q_w+q_n=Q$ to obtain

$$
q_w=QF(s)+K\frac{\lambda_w\lambda_n}{\lambda_w+\lambda_n}p_c'(s)s_x
=QF(s)-D_c(s)s_x,
\qquad
D_c(s)=-K\frac{\lambda_w\lambda_n}{\lambda_w+\lambda_n}p_c'(s).
$$

The wetting-phase [mass conservation](../../../../../mass-conservation.md) law is consequently

$$
\boxed{\phi s_t+Q\partial_xF(s)=\partial_x[D_c(s)s_x].}
$$

For $p_c'\leq0$, $D_c\geq0$ and the [capillary pressure](../../../../../capillary-pressure.md) provides nonlinear diffusion. The initially uniform saturation is $s_0$. Pure wetting-fluid injection prescribes $q_w(0,t)=Q$ and $q_n(0,t)=0$; in the zero-capillarity, zero-residual-nonwetting idealization this corresponds to inlet saturation one. With residual nonwetting fluid, replace one by the appropriate maximum accessible saturation.

**Shock formation and its speed.** Neglect capillarity first. Smooth saturation values travel along [characteristic curves](../../../../../characteristic-curve.md) at speed $(Q/\phi)F'(s)$. When the trailing values have larger [characteristic speeds](../../../../../characteristic-speed.md) than the values ahead, the curves intersect, and the [Buckley-Leverett equation](../../../../../buckley-leverett-equation.md) requires a [shock](../../../../../shock-wave.md) selected as an [entropy solution](../../../../../entropy-solution.md). This is typical for the increasing-convex part of a physical fractional-flow curve; [shocks](../../../../../shock-wave.md) are not inevitable for every possible $F$.

Integrating [mass conservation](../../../../../mass-conservation.md) across a [shock](../../../../../shock-wave.md) from upstream $s_s$ to downstream $s_0$ gives the [Rankine-Hugoniot condition](../../../../../rankine-hugoniot-conditions.md)

$$
\boxed{V_s=\frac Q\phi\frac{F(s_s)-F(s_0)}{s_s-s_0}.}
$$

If an upstream [rarefaction wave](../../../../../rarefaction-wave.md) joins the [shock](../../../../../shock-wave.md) smoothly in similarity coordinates, its terminal characteristic speed equals $V_s$. Therefore the saturation at that join obeys the [fractional-flow tangent construction](../../../../../fractional-flow-tangent-construction.md)

$$
\boxed{F'(s_s)=\frac{F(s_s)-F(s_0)}{s_s-s_0}.}
$$

This is the printed equality. It is a tangent-selection condition, not the dimensional speed by itself; the speed includes $Q/\phi$. An arbitrary [shock](../../../../../shock-wave.md) between prescribed constant states satisfies the jump condition but need not satisfy this additional tangency relation.

Positive [capillary diffusion](../../../../../capillary-diffusion.md) spreads a jump into a transition layer. For a travelling profile $s(x-V_st)$, integration gives

$$
D_c(s)s'=Q[F(s)-F(s_0)]-\phi V_s(s-s_0).
$$

The endpoint states still satisfy the same [Rankine-Hugoniot condition](../../../../../rankine-hugoniot-conditions.md). Thus small capillarity primarily gives the front a finite thickness rather than changing the selected limiting speed; vanishing phase mobility at an endpoint can make the regularization degenerate.

**The specified reciprocal fractional flow.** On its stated branch, $F'=1/s^2$ and $F''=-2/s^3<0$. If $F$ extends continuously to the initial saturation and the inlet is at one, the decreasing saturation from behind to ahead makes [characteristic speeds](../../../../../characteristic-speed.md) increase forwards: there is a [rarefaction wave](../../../../../rarefaction-wave.md), not a compressive [shock](../../../../../shock-wave.md). Write $a=Q/\phi$ and $\xi=x/t$. The [self-similar solution](../../../../../similarity-solution.md) is

$$
\boxed{s(x,t)=\begin{cases}
1,&0\leq\xi\leq a,\\
\sqrt{a/\xi},&a<\xi<a/s_0^2,\\
s_0,&\xi\geq a/s_0^2.
\end{cases}}
$$

The fan connects continuously to the initial state and broadens linearly in time. This interpretation requires $F(s_0)=2-1/s_0$. A nonnegative physical fractional flow on the entire interval $[s_0,1]$ also requires $s_0\geq1/2$.

The PDF specifies the formula only for $s>s_0$ and earlier calls $s_0$ residual. If that means an immobile wetting phase with $F(s_0)=0$, the endpoint is an extra constraint and the continuous-branch answer applies without conflict only at $s_0=1/2$. For $0<s_0<1/2$, the printed branch would give negative fractional flow for $s_0<s<1/2$, so it cannot be the complete physical constitutive law. With an additional admissible extension, for example $F=0$ up to $1/2$ and the given positive branch above it, a compound fan–[shock](../../../../../shock-wave.md) is possible. The tangent condition then gives

$$
s_s=\frac{1+\sqrt{1-2s_0}}2,\qquad
V_s=\frac a{s_s^2}.
$$

The fan $s=\sqrt{a/\xi}$ ends at $\xi=V_s$, followed by a jump to $s_0$. This is a conditional physical extension, not data supplied by the question. For $s_0>1/2$ an immobile residual endpoint is likewise incompatible with a continuous version of the stated branch. These distinctions identify what is, and is not, determined by the printed constitutive assumption.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
