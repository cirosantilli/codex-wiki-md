<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a smooth positive discharge on the flat bed, differentiate the constant specific energy. With $q(x)=Q/b(x)$,

$$
(1-F^2)h_x+\frac{q q_x}{gh^2}=0.
$$

At a regular critical point, $F=1$ and $q>0$, so $q_x=0$. Since $Q$ is constant, this requires $b_x=0$. The given width has $b_x=2b_0x/L^2$, proving that **a regular [hydraulic control](../../../../../../hydraulic-control.md) can occur only at $x=0$**.

The throat is the unique width minimum and hence the maximum of the critical-energy envelope

$$
E_c(x)=\frac32\left(\frac{Q^2}{gb(x)^2}\right)^{1/3}.
$$

A steady positive-depth flow must have its conserved energy at least as large as every local minimum energy. To be controlled smoothly at the throat it must satisfy

$$
\boxed{h_c(0)=\left(\frac{Q^2}{gb_0^2}\right)^{1/3},\qquad
\mathcal B=E=\frac32\left(\frac{Q^2}{gb_0^2}\right)^{1/3}.}
$$

Equivalently the controlled discharge at a prescribed head is $Q=b_0\sqrt g\,(2\mathcal B/3)^{3/2}$. If the head is larger than this critical value at fixed $Q$, the two depth branches remain separate everywhere and the flow need not be controlled. If it is smaller, no smooth steady solution carrying that discharge through the throat exists; upstream head or discharge must adjust.

Boundary conditions must also select the appropriate connected branches. A local expansion about the throat gives

$$
E-E_c(0)=\frac{3}{2h_c}(h-h_c)^2-\frac{h_c x^2}{L^2}+	ext{higher-order terms}.
$$

At the controlled head, $h_x(0)=\pm\sqrt{2/3}\,h_c/L$. The usual accelerating positive-discharge connection uses the negative slope: deep [subcritical flow](../../../../../../subcritical-flow.md) upstream becomes shallow [supercritical flow](../../../../../../supercritical-flow.md) downstream. The throat is a maximum of the critical-head envelope, as required for a real smooth transcritical connection in [hydraulic control in a variable-width channel](../../../../../../hydraulic-control-in-a-variable-width-channel.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
