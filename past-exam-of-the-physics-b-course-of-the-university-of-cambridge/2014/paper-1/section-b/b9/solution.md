<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

$Z$ is the terminating load impedance, $Z_0$ the line's [characteristic impedance](../../../../../characteristic-impedance.md), and $k$ the propagation [wave number](../../../../../wavenumber.md); $l$ is its [length](../../../../../length.md). In the lossless convention printed, an open circuit gives $Z_{\rm in}=-iZ_0\cot kl$, a short circuit gives $iZ_0\tan kl$, and a matched load $Z=Z_0$ gives **$Z_{\rm in}=Z_0$ for every [length](../../../../../length.md)**. The divergent or zero limits at isolated electrical [lengths](../../../../../length.md) are understood continuously.

Put $\theta=kl$, $c_\theta=\cos\theta$, $s_\theta=\sin\theta$. The voltage/current [matrix](../../../../../matrix.md) of one section is

$$
M_j=\begin{pmatrix}c_\theta&iZ_js_\theta\\is_\theta/Z_j&c_\theta\end{pmatrix}.
$$

For a pair beginning with $Z_1$, write $M_1M_2=\left(\begin{smallmatrix}A&B\\C&D\end{smallmatrix}\right)$. Its entries are $A=c_\theta^2-(Z_1/Z_2)s_\theta^2$, $D=c_\theta^2-(Z_2/Z_1)s_\theta^2$, $B=i(Z_1+Z_2)s_\theta c_\theta$, and $C=i(1/Z_1+1/Z_2)s_\theta c_\theta$. The [alternating-impedance transmission line](../../../../../alternating-impedance-transmission-line.md) has unchanged input $X$, its [Bloch impedance](../../../../../bloch-impedance.md), obeying $X=(AX+B)/(CX+D)$. Hence, away from the removable dividing zeros,

$$
iX^2(Z_1+Z_2)+X(Z_1^2-Z_2^2)\tan\theta-iZ_1Z_2(Z_1+Z_2)=0,
$$



$$
\boxed{X=\frac{i(Z_1-Z_2)\tan\theta\ \pm\sqrt{4Z_1Z_2-(Z_1-Z_2)^2\tan^2\theta}}2.}
$$

For real positive $Z_1,Z_2$, select the branch carrying [energy](../../../../../energy-split.md) into the line or decaying into it. A positive real part selects the pass-band root; infinitesimal passive loss resolves the stop-band branch. At $\theta=m\pi$ the cell [matrix](../../../../../matrix.md) is the identity, so the exact fixed-point condition alone does not determine $X$; at odd quarter-wave [lengths](../../../../../length.md) the appropriate limiting impedance can be zero or infinite.

In a [transmission-line stop band](../../../../../transmission-line-stop-band.md), a lossless semi-infinite ladder totally reflects because its physical input is reactive. Equivalently its cell has

$$
\tfrac12\operatorname{tr}M=1-\frac{(Z_1+Z_2)^2}{2Z_1Z_2}\sin^2\theta<-1.
$$

Thus, for nonzero contrast, the stop-band interiors satisfy

$$
\boxed{|\tan kl|>\frac{2\sqrt{Z_1Z_2}}{|Z_1-Z_2|},\quad\text{equivalently}\quad
\sin^2kl>\frac{4Z_1Z_2}{(Z_1+Z_2)^2}.}
$$

With $\theta_c=\arcsin[2\sqrt{Z_1Z_2}/(Z_1+Z_2)]$, these are $m\pi+\theta_c<kl<(m+1)\pi-\theta_c$; band-edge reflection follows by a limit. If $k=\omega/u$, multiply the endpoints by $u/l$ for [angular frequencies](../../../../../angular-frequency.md). Identical impedances have no stop band. A finite ladder can transmit by tunnelling, unlike the semi-infinite idealization.

<a id="section-b/b9/image-calculated-bloch-trace-and-reflected-power-for-a-chosen-alternating-impedance-line"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-1-periodic-line.png)

**[Figure 2](#section-b/b9/image-calculated-bloch-trace-and-reflected-power-for-a-chosen-alternating-impedance-line). Calculated Bloch trace and reflected power for a chosen alternating-impedance line**.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
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
