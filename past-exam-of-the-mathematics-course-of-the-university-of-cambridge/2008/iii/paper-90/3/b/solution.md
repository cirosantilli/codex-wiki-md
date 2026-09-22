<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the upward coordinate of the preceding [kinematic sedimentation](../../../../../../kinematic-sedimentation.md) calculation, with the given smooth profile on $0\le\zeta\le h$ and clear fluid above. This asks for the first characteristic breaking of that profile; a separately imposed packed-bed discontinuity would be a different boundary problem.

Substitution of the initial [concentration](../../../../../../concentration.md) into the [characteristic speed](../../../../../../characteristic-speed.md) gives

$$
c_0(\zeta)=-\frac{V_s}{3}-\frac{2V_s\zeta^2}{3h^2},\qquad
z(\zeta,t)=\zeta+c_0(\zeta)t.
$$

The characteristic Jacobian is

$$
\frac{\partial z}{\partial\zeta}=1-\frac{4V_s\zeta t}{3h^2}.
$$

It first vanishes at the upper edge $\zeta=h$. That edge has zero [concentration](../../../../../../concentration.md) and descends initially at $V_s$, so

$$
\boxed{t_s=\frac{3h}{4V_s},\qquad z_s=h-V_st_s=\frac h4.}
$$

Although the derivative of the initial profile jumps to zero in the clear region, the [concentration](../../../../../../concentration.md) itself is continuous there. The [shock](../../../../../../shock-wave.md) starts with vanishing amplitude. Both limiting concentrations at onset are zero, and the [Rankine-Hugoniot condition](../../../../../../rankine-hugoniot-conditions.md) consequently gives

$$
\boxed{\dot s(t_s^+)=-V_s.}
$$

This is a downward speed $V_s$.

After formation the upper state remains clear, $\phi_R=0$, and the lower state is positive. The [parabolic-profile sedimentation shock](../../../../../../parabolic-profile-sedimentation-shock.md) has

$$
\dot s=-V_s\left(1-\frac{\phi_L}{\phi_{\max}}\right).
$$

It therefore initially slows down in magnitude: its signed upward-coordinate speed increases from $-V_s$. One can also verify that its captured left state increases. Write $r=\zeta_L/h$, where $\zeta_L$ labels the incident lower characteristic. Conservation of the particle volume initially above that characteristic gives

$$
\frac{V_s t}{\phi_{\max}}\phi_0(\zeta_L)^2=\int_{\zeta_L}^h\phi_0(\zeta)\,d\zeta,
\qquad
\frac{V_st}{h}=\frac{r+2}{(r+1)^2}.
$$

The derivative of the right-hand side with respect to $r$ is $-(r+3)/(r+1)^3<0$. Thus $r$ decreases as time increases, and $\phi_L=\phi_{\max}(1-r^2)/3$ increases. The downward [shock](../../../../../../shock-wave.md) speed continues to decrease on this branch until a bed or another boundary interacts with it. No later boundary behavior is needed for the requested conclusion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 90](../../../paper-90-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
