<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [magnetic vector potential](../../../../magnetic-vector-potential.md) is defined by $\mathbf B=\nabla\times\mathbf A$. The [gauge transformation](../../../../gauge-transformation.md)

$$
\boxed{\mathbf A\mapsto\mathbf A+\nabla\chi,\qquad\phi\mapsto\phi-\partial_t\chi}
$$

leaves both $\mathbf B$ and $\mathbf E=-\nabla\phi-\partial_t\mathbf A$ unchanged. In [magnetostatics](../../../../magnetostatics.md) choose the [Coulomb gauge](../../../../coulomb-gauge.md) $\nabla\cdot\mathbf A=0$. Then [Ampère's law](../../../../ampere-s-circuital-law.md) and the curl-of-curl identity give

$$
\mu_0\mathbf J=\nabla\times(\nabla\times\mathbf A)=\nabla(\nabla\cdot\mathbf A)-\nabla^2\mathbf A,\qquad\boxed{\nabla^2\mathbf A=-\mu_0\mathbf J.}
$$

The free-space [Green function](../../../../green-s-function-split.md) identity $\nabla^2|\mathbf r-\mathbf r'|^{-1}=-4\pi\delta^{(3)}(\mathbf r-\mathbf r')$ therefore gives

$$
\boxed{\mathbf A(\mathbf r)=\frac{\mu_0}{4\pi}\int\frac{\mathbf J(\mathbf r')}{|\mathbf r-\mathbf r'|}\,d^3r'.}
$$

The [boundary condition](../../../../boundary-condition.md) selects the homogeneous solution; the usual decay condition assumes suitably localized sources. An infinitely long static wire needs a reference for its logarithmically divergent potential, although its [magnetic field](../../../../magnetic-field-split.md) is finite away from the wire.

For time-dependent sources use the **[Lorenz gauge](../../../../lorenz-gauge-condition.md)**, $\nabla\cdot\mathbf A+c^{-2}\partial_t\phi=0$, and the outgoing [retarded potential](../../../../retarded-potential.md)

$$
\boxed{\mathbf A(\mathbf r,t)=\frac{\mu_0}{4\pi}\int\frac{\mathbf J(\mathbf r',t-|\mathbf r-\mathbf r'|/c)}{|\mathbf r-\mathbf r'|}\,d^3r'.}
$$

The [scalar potential](../../../../scalar-potential.md) has the analogous retarded charge-density integral. The two gauges should not be conflated for a general time-dependent source.[Equations (73)–(76): Lorenz-gauge retarded scalar and vector potentials](../../../../retarded-potentials-by-richard-fitzpatrick.md)

For the prescribed uncharged wire, $\rho=0$ and $\phi=0$ is consistent. Translation invariance makes $\mathbf A=A_z(r,t)\hat{\mathbf z}$ with $\nabla\cdot\mathbf A=0$, so this particular solution satisfies both gauge conditions. With $s=z'-z$,

$$
A_z=\frac{\mu_0 I}{4\pi}\int_{-\infty}^{\infty}\frac{\Theta(t-\sqrt{r^2+s^2}/c)}{\sqrt{r^2+s^2}}\,ds.
$$

It is zero for $t<r/c$. For $t>r/c$, set $L=\sqrt{c^2t^2-r^2}$. The causal interval is $-L<s<L$, giving the [switched infinite-wire retarded potential](../../../../switched-infinite-wire-retarded-potential.md)

$$
\boxed{A_z=\frac{\mu_0I}{2\pi}\operatorname{arsinh}\frac Lr=\frac{\mu_0I}{2\pi}\operatorname{arcosh}\frac{ct}{r}=\frac{\mu_0I}{2\pi}\ln\!\left(\frac{ct+\sqrt{c^2t^2-r^2}}r\right).}
$$

Differentiation gives the fields and [Poynting vector](../../../../poynting-vector.md), for $r>0$, $t>r/c$:

$$
\boxed{\begin{aligned}
\mathbf E&=-\frac{\mu_0Ic}{2\pi\sqrt{c^2t^2-r^2}}\hat{\mathbf z},\\
\mathbf H&=\frac{Ict}{2\pi r\sqrt{c^2t^2-r^2}}\hat{\boldsymbol\phi},\\
\mathbf N=\mathbf E\times\mathbf H&=\frac{\mu_0I^2c^2t}{4\pi^2r(c^2t^2-r^2)}\hat{\mathbf r}.
\end{aligned}}
$$

Here $\mathbf B=\mu_0\mathbf H$ and $B_\phi=-\partial_rA_z$. All three fields vanish before arrival. For positive $I$, $\mathbf E$ opposes the imposed current and the [radial energy flow after switching a line current](../../../../radial-energy-flow-after-switching-a-line-current.md) points **radially outward**: $(-\hat{\mathbf z})\times\hat{\boldsymbol\phi}=\hat{\mathbf r}$.

<a id="3/image-at-fixed-radius-the-causal-fields-start-at-t-equals-r-over-c-and-relax-toward-the-magnetostatic-limit"></a>
![](../../../../past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2016/paper-1-switched-wire.png)

**[Figure 4](#3/image-at-fixed-radius-the-causal-fields-start-at-t-equals-r-over-c-and-relax-toward-the-magnetostatic-limit). At fixed radius the causal fields start at t equals r over c and relax toward the magnetostatic limit**. [Source](paper-1-switched-wire.py).

For the graph, let $u=ct/r$. Normalized to $E_*=\mu_0Ic/(2\pi r)$, $H_*=I/(2\pi r)$ and $N_*=\mu_0I^2c/(4\pi^2r^2)$, the curves are

$$
E_z/E_*=-\frac1{\sqrt{u^2-1}},\qquad H_\phi/H_*=\frac u{\sqrt{u^2-1}},\qquad N_r/N_*=\frac u{u^2-1}\quad(u>1).
$$

At the [wavefront](../../../../wavefront.md), $|E_z|$ and $H_\phi$ diverge as $(u-1)^{-1/2}$ and $N_r$ as $(u-1)^{-1}$. This [abrupt line-current wavefront singularity](../../../../abrupt-line-current-wavefront-singularity.md) reflects the ideal instantaneous turn-on of a line current; a finite rise time smooths the front. At late times,

$$
E_z\sim-\frac{\mu_0I}{2\pi t}\to0,\qquad H_\phi\to\frac I{2\pi r},\qquad N_r\sim\frac{\mu_0I^2}{4\pi^2rt}\to0.
$$

The vector potential grows logarithmically with time in this infinite-wire idealization even as the local [magnetic field](../../../../magnetic-field-split.md) approaches its static limit. The divergent front should not be interpreted as a finite-energy pulse from a real instantaneous switching experiment.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2016](../../split.md)
4. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../split.md)
5. [Optics and Electrodynamics course of the University of Cambridge](../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
