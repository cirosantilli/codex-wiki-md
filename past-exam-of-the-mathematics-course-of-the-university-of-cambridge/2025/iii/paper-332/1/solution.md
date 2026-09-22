<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put ice in $x<a(t)$ and ocean in $x>a(t)$, with $x$ increasing into the ocean. This is a [saline Stefan problem](../../../../../saline-stefan-problem.md). The ice and liquid temperatures satisfy

$$
T_{s,t}=\kappa T_{s,xx},
\qquad
T_{l,t}=\kappa T_{l,xx},
$$

and the ocean salinity satisfies $C_t=DC_{xx}$. The far-field and interfacial conditions are

$$
T_s(-\infty,t)=T_{-\infty},
\quad T_l(+\infty,t)=T_m,
\quad C(+\infty,t)=C_0,
$$



$$
T_s(a,t)=T_l(a,t)=T_i=T_m-mC_i,
\quad C(a,t)=C_i,
$$



$$
\rho L_f\dot a=k_T(T_{s,x}-T_{l,x})_{x=a},
\qquad
-D C_x(a^+,t)=C_i\dot a.
$$

The last two equations are the [Stefan condition](../../../../../stefan-condition.md) and solute conservation. Salt is taken to be absent from the ice. The field sketch has two broad thermal boundary layers of width $O(\sqrt{\kappa t})$ and a liquid-side salinity layer of width $O(\sqrt{Dt})$.

The [diffusion equation](../../../../../diffusion-equation-split.md) is invariant under $(x,t)\mapsto(cx,c^2t)$, so a solution with constant far-field data and no fixed length has $a/\sqrt{Dt}$ constant. Write

$$
a(t)=2\lambda\sqrt{Dt},
\qquad \epsilon=\sqrt{D/\kappa}.
$$

The [Neumann solution of the Stefan problem](../../../../../neumann-solution-of-the-stefan-problem.md) becomes

$$
T_s=T_{-\infty}+(T_i-T_{-\infty})
\frac{1+\operatorname{erf}(x/(2\sqrt{\kappa t}))}
{1+\operatorname{erf}(\epsilon\lambda)},
$$



$$
T_l=T_m+(T_i-T_m)
\frac{\operatorname{erfc}(x/(2\sqrt{\kappa t}))}
{\operatorname{erfc}(\epsilon\lambda)},
$$



$$
C=C_0+(C_i-C_0)
\frac{\operatorname{erfc}(x/(2\sqrt{Dt}))}
{\operatorname{erfc}(\lambda)}.
$$

Substitution into the salt balance and the [Stefan condition](../../../../../stefan-condition.md) gives the required pair of equations. With $c_p=k_T/(\rho\kappa)$ and

$$
F(z)=\sqrt\pi z e^{z^2}\operatorname{erfc}z,
$$

they are

$$
\boxed{F(\lambda)=1-\frac{C_0}{C_i}
=1-\frac{mC_0}{T_m-T_i},}
$$



$$
\boxed{
\sqrt\pi\frac{L_f}{c_p}\epsilon\lambda e^{\epsilon^2\lambda^2}
=\frac{T_i-T_{-\infty}}{1+\operatorname{erf}(\epsilon\lambda)}
-\frac{T_m-T_i}{\operatorname{erfc}(\epsilon\lambda)}.}
$$

When $\epsilon\ll1$, heat diffuses much farther than salt. The leading heat-flux balance gives

$$
\boxed{T_i\sim\frac{T_m+T_{-\infty}}2,}
\qquad
\boxed{F(\lambda)\sim1-\frac{2mC_0}{T_m-T_{-\infty}}.}
$$

Since $F$ has the sign of $\lambda$, ice grows when $T_m-T_{-\infty}>2mC_0$, is stationary at equality, and ablates when $T_m-T_{-\infty}<2mC_0$.

During growth, salt rejection gives $C_i>C_0$. Moving from the interface into the ocean, the phase-diagram trajectory first moves rapidly toward lower $C$ at nearly fixed $T$ and can fall below the [liquidus](../../../../../liquidus.md); this is [constitutional supercooling](../../../../../constitutional-supercooling.md). During ablation, $C_i<C_0$, so the near-interface trajectory moves toward larger $C$ and into the stable liquid region above the liquidus. Ablation occurs because the heat conducted from the warmer ocean to the interface exceeds the heat that the colder ice can remove; melting and salt diffusion then maintain local liquidus equilibrium.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
