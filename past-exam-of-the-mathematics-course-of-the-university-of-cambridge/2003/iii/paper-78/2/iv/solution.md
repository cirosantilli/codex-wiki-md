<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

At a welded interface, [elastic-interface boundary conditions](../../../../../../elastic-interface-boundary-conditions.md) require continuous SH displacement and shear [traction](../../../../../../traction.md). Incident and reflected vertical slownesses have signs $q_1,-q_1$, giving

$$
1+R_{\rm SH}=T_{\rm SH},\qquad
\mu_1q_1(1-R_{\rm SH})=\mu_2q_2T_{\rm SH}.
$$

Thus the local displacement coefficient is

$$
\boxed{T_{\rm SH}(p)=\frac{2\mu_1q_1}{\mu_1q_1+\mu_2q_2}}.
$$

It multiplies the leading waveform discontinuity as well as a harmonic displacement. At the interface the incident amplitude from [SH ray-tube amplitude transport](../../../../../../sh-ray-tube-amplitude-transport.md) is $C/\sqrt{r_1}$, where $r_1=h/(\beta_1q_1)$ is the incident path length and $C$ is the source normalization from the previous part.

The transmitted geometrical spreading is not simply its total path length. Differentiate the ray position with respect to $p$ at fixed travel time and project onto the unit direction transverse to the transmitted ray, $\mathbf m_2=(\beta_2q_2,-\beta_2p)$. Since $dx_I/dp=h/(\beta_1^2q_1^3)$, the transverse width per unit $p$ is

$$
J_2(t,p)=\mathbf m_2\cdot\partial_p(x,z)
=\beta_2\left[\frac{h q_2}{\beta_1^2q_1^3}+\frac{t-t_1}{q_2}\right].
$$

The derivative of $t_1$ contributes only in the ray direction and drops out of this projection. At entry,

$$
J_{2I}=\frac{\beta_2h q_2}{\beta_1^2q_1^3},\qquad
\frac{J_{2I}}{J_{1I}}=\frac{\cos\theta_2}{\cos\theta_1},\quad
J_{1I}=\frac{h}{\beta_1q_1^2}.
$$

Within uniform medium 2 the leading amplitude varies as $J_2^{-1/2}$, so the required [refraction of a cylindrical SH wavefront](../../../../../../refraction-of-a-cylindrical-sh-wavefront.md) amplitude is

$$
\boxed{a_T(t,p)=\frac{C T_{\rm SH}(p)}{\sqrt{r_1}}
\sqrt{\frac{J_{2I}}{J_2(t,p)}}
=\frac{C T_{\rm SH}(p)}{\sqrt{\displaystyle\frac{h}{\beta_1q_1}+\frac{\beta_1q_1^2}{q_2^2}[t-t_1(p)]}}}.
$$

The local [transmission coefficient](../../../../../../transmission-coefficient.md) and ray-tube spreading together incorporate both impedance contrast and refraction. Indeed the normal energy transmission fraction is $\mu_2q_2|T_{\rm SH}|^2/(\mu_1q_1)$, while the change of transverse width supplies the refraction factor in the conserved tube flux. If the media coincide, $q_1=q_2$ and $T_{\rm SH}=1$, reducing this expression to $C/\sqrt{\beta_1t}$ as required. The formula holds for the stated propagating slownesses, without a critical or head-wave contribution.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
