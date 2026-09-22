<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A model must track polymer age as well as its position. Polymer enters during $s\in[t_a,t_a+\Delta t]$ and activates at age $\tau$. The first activation in laboratory time is $t_a+\tau$, not $\tau$ measured from initial water injection. Assume activation permanently changes the local [dynamic viscosity](../../../../../../dynamic-viscosity.md) from $\mu$ to $\lambda\mu$, with $\lambda>1$, and neglect polymer diffusion, retention and shear-dependent rheology.

Let $X_i(t)=\int_0^t u_i(r)\,dr$ be cumulative pore-fluid displacement. A fluid particle entering at time $s$ has position $X_i(t)-X_i(s)$ until it exits. At time $t\ge t_a+\tau$, the youngest activated polymer was injected at $s_y=\min(t_a+\Delta t,t-\tau)$. The length of activated polymer still inside layer $i$ is exactly

$$
\ell_i(t)=\left[\min\{L,X_i(t)-X_i(t_a)\}
-\max\{0,X_i(t)-X_i(s_y)\}\right]_+.
$$

Set $\ell_i=0$ when $t<t_a+\tau$. This accounts both for gradual activation of the slug and its later exit. Hydraulic resistances add in series, so [delayed polymer diversion in parallel porous layers](../../../../../../delayed-polymer-diversion-in-parallel-porous-layers.md) is described by

$$
\boxed{\dot X_i(t)=\frac{k_i\Delta P}
{\phi\mu[L+(\lambda-1)\ell_i(t)]},
\quad Q_i(t)=\frac{A_i k_i\Delta P}
{\mu[L+(\lambda-1)\ell_i(t)]}.}
$$

These history-dependent equations close the model and can be integrated forwards, retaining previously computed values of $X_i$. The overall volume discharge and low-permeability inflow fraction are

$$
Q_{\rm tot}=Q_1+Q_2,
\qquad f_2=\frac{A_2k_2/[L+(\lambda-1)\ell_2]}
{\sum_i A_ik_i/[L+(\lambda-1)\ell_i]}.
$$

The original displacement front reaches the distal well when $X_i(t)=L$. Consequently the injected-fluid outflow is $\sum_iQ_i(t)\mathbf1_{X_i(t)\ge L}$, and the complementary sum gives original-fluid production.

The mechanism is especially transparent if $\Delta t<\tau$, so the entire slug is injected before activation begins, and it activates before leaving the high-permeability layer. Before activation, its lengths are $u_i^0\Delta t$. While each complete activated slug remains in its layer, those lengths stay fixed and

$$
\frac{Q_i}{Q_i^0}=\frac1{1+(\lambda-1)\Delta t/t_i},
\qquad t_1=t_a,\quad t_2=t_s.
$$

The fractional resistance increase is larger in the fast layer. An effective selective regime is $\Delta t<t_a$ and $\Delta t<\tau<t_a$, with $(\lambda-1)\Delta t/t_a$ appreciable while $(\lambda-1)\Delta t/t_s$ is small; the full delay model handles the activation ramps and the later exits. The relative share entering the slow layer then increases, although its absolute discharge cannot increase at fixed pressure. The total discharge decreases during polymer occupancy and returns to its original value once the activated slugs leave. A fixed-total-injection-rate experiment would have a different pressure response and cannot be substituted for this fixed-pressure model.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
