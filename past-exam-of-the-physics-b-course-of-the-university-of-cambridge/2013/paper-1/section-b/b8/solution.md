<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

For a moving loop, [Faraday's law of induction](../../../../../faraday-s-law-of-induction.md) is $\mathcal E=\oint(\mathbf E+\mathbf u\times\mathbf B)\cdot d\mathbf l=-d\Phi_B/dt$, where $\mathbf u$ is the local wire [velocity](../../../../../velocity.md), $\Phi_B=\int\mathbf B\cdot d\mathbf S$, and the oriented boundary and surface follow the right-hand rule. For a fixed loop the motional term vanishes. [Lenz's law](../../../../../lenz-s-law.md) is the minus sign: the induced response opposes the change of linked flux, not necessarily the applied field itself.

Let $s$ increase downhill and choose positive current $I$ to produce an uphill magnetic [force](../../../../../force-split.md). The normal component of the imposed field is $B\cos\theta$, so the changing external flux is $Bl\cos\theta\,s$. With initially zero current and no resistance, conservation of [flux linkage](../../../../../magnetic-flux-linkage.md) gives $LI=Bl\cos\theta\,s$. The rod feels gravity vertically downward, a rail reaction normal to the slope, and magnetic [force](../../../../../force-split.md) of magnitude $IlB$ horizontally uphill. Its downhill component is $-IlB\cos\theta$; its normal component presses the rod into the rails, giving $N=mg\cos\theta+IlB\sin\theta$.

The [inductive oscillation of a sliding rod on inclined rails](../../../../../inductive-oscillation-of-a-sliding-rod-on-inclined-rails.md) follows from

$$
m\ddot s=mg\sin\theta-\frac{B^2l^2\cos^2\theta}{L}s,
\qquad\boxed{\kappa=\frac{l^2\cos^2\theta}{L}.}
$$

The magnetic [force](../../../../../force-split.md) is not itself parallel to the rails. Defining $\omega_B=Bl\cos\theta/\sqrt{mL}$ and $s_e=mg\sin\theta/(m\omega_B^2)$, release from rest gives

$$
s(t)=s_e(1-\cos\omega_Bt),\qquad
\boxed{s_{\rm first\ stop}=2s_e=\frac{2mgL\sin\theta}{B^2l^2\cos^2\theta}.}
$$

The first stop occurs at $t=\pi/\omega_B$; the rod then returns and oscillates between $0$ and $2s_e$. At $s_e$ the [force](../../../../../force-split.md) is zero but the [speed](../../../../../speed.md) is maximal. Mechanical [potential energy](../../../../../potential-energy.md) is reversibly exchanged with [kinetic energy](../../../../../kinetic-energy.md) and $LI^2/2$; a perfectly conducting circuit provides no damping.

For the [resistive long-time drift of an inductive sliding rod](../../../../../resistive-long-time-drift-of-an-inductive-sliding-rod.md), with loop resistance $R>0$, use

$$
L\dot I+RI=Bl\cos\theta\,\dot s,\qquad
m\ddot s=mg\sin\theta-Bl\cos\theta\,I.
$$

[Joule heating](../../../../../joule-heating.md) damps the transient oscillation. On sufficiently long rails the asymptotic motion is steady sliding, not permanent rest:

$$
\boxed{I_\infty=\frac{mg\sin\theta}{Bl\cos\theta},\qquad
v_\infty=\frac{Rmg\sin\theta}{B^2l^2\cos^2\theta}.}
$$

The zero-resistance model has persistent oscillations; its late-time limit cannot be interchanged with taking $R\to0$. These results assume $B\cos\theta\ne0$, smooth contacts, negligible rod self-inductance and constant geometry.

<a id="section-b/b8/image-original-rod-force-resolution-and-calculated-ideal-inductive-oscillation-along-the-slope"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-1-inductive-rails.png)

**[Figure 3](#section-b/b8/image-original-rod-force-resolution-and-calculated-ideal-inductive-oscillation-along-the-slope). Original rod force resolution and calculated ideal inductive oscillation along the slope**.

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
