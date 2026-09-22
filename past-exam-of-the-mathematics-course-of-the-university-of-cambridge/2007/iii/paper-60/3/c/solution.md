<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With $B_y=0$, a pulse of the $x$ field realizes $R_x(\theta)=e^{-i\theta\sigma_x/2}$ when $\int B_x(t)dt=\theta/2$. Similarly the $y$ field realizes $R_y(\theta)$ with area $\theta/2$. These are instances of the [quantum pulse area](../../../../../../quantum-pulse-area.md) rule. A [rotation about the z-axis](../../../../../../rotation-about-the-z-axis.md) can be synthesized from the two available axes:

$$
R_z(\theta)=R_x(\pi/2)R_y(\theta)R_x(-\pi/2),
$$

because $R_x(\pi/2)\sigma_yR_x(-\pi/2)=\sigma_z$.

For a target $V=\begin{pmatrix}u&v\\-v^*&u^*\end{pmatrix}$, one convenient construction is

$$
V=R_z(\alpha)R_y(\beta)R_z(\gamma),\qquad
u=e^{-i(\alpha+\gamma)/2}\cos(\beta/2),\quad v=-e^{-i(\alpha-\gamma)/2}\sin(\beta/2).
$$

Take $\beta=2\operatorname{atan2}(|v|,|u|)$ and choose $\alpha+\gamma=-2\arg u$, $\alpha-\gamma=-2\arg(-v)$ when both entries are nonzero; if an entry vanishes its phase constraint can be omitted. Substitute the three-pulse construction for each $z$ rotation. Apply the factors from right to left in time. **Pulses along the available $x,y$ axes therefore implement every single-qubit gate up to global phase**. Negative angles use negative field area, or an equivalent full-period rotation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
