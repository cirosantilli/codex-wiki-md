<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $z=0$ at the base and assume gas leaves freely at the liquid surface, without being retained as foam. There is no new bubble production after filling. Neglecting the liquid velocity, gas-volume conservation is a [scalar conservation law](../../../../../../scalar-conservation-law.md)

$$
\phi_t+\partial_zj(\phi)=0,\qquad j(\phi)=V_s\phi(1-\phi).
$$

An impermeable base has no incoming bubbles. Thus a clear region develops below the uniform bubbly region. The clearing discontinuity satisfies the [Rankine-Hugoniot condition](../../../../../../rankine-hugoniot-conditions.md), with states $0$ and $\phi_0$:

$$
s=\frac{j(\phi_0)-j(0)}{\phi_0-0}=V_s(1-\phi_0).
$$

For the dilute regime $0<\phi_0<1/2$, the characteristic speeds obey $j'(0)>s>j'(\phi_0)$, so this is the admissible compressive [shock](../../../../../../shock-wave.md). Before it reaches the surface,

$$
\phi(z,t)=\begin{cases}0,&0<z<st,\\ \phi_0,&st<z<H.\end{cases}
$$

The remaining bubbles move upwards at $s$ and escape at the top. Averaging the [void fraction](../../../../../../void-fraction.md) over the entire cylindrical volume gives

$$
\boxed{\Phi(t)=\phi_0\max\left(1-\frac{V_s(1-\phi_0)t}{H},0\right),\qquad
 t_{\rm clear}=\frac{H}{V_s(1-\phi_0)}.}
$$

This [bubble clearing in a cylindrical vessel](../../../../../../bubble-clearing-in-a-cylindrical-vessel.md) describes bubbles in the liquid, not a hypothetical retained gas layer above it. A closed surface or long-lived foam would require a different upper boundary condition.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
