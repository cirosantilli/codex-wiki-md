<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

The grounded conducting plane supplies the induced charge needed for a uniform field between the plates and zero field above the upper plate. [Gauss's law](../../../../../gauss-s-law.md) gives $E_z=-\sigma/\epsilon_0$ in the gap. With [electric potential](../../../../../electric-potential.md) zero at the grounded plate,

$$
\boxed{\phi(z)=\frac{\sigma z}{\epsilon_0},\qquad V=\frac{\sigma d}{\epsilon_0}.}
$$

Integrating the [electrostatic energy](../../../../../electrostatic-energy.md) density $\epsilon_0|\mathbf E|^2/2$ across the gap gives the [capacitor energy](../../../../../capacitor-energy.md) per unit area

$$
u=\frac{\sigma^2d}{2\epsilon_0}=\frac{\epsilon_0V^2}{2d}=\frac12\sigma V.
$$

For an isolated upper plate, charge is fixed, so increasing $d$ to $(1+\alpha)d$ gives exactly **$\Delta u=\tfrac12\sigma V\alpha$**, with $V$ its initial value. The positive increase equals the mechanical work done against attraction.

At fixed voltage, the new charge density is $\sigma/(1+\alpha)$, and the energy becomes $u/(1+\alpha)$. Consequently **$\Delta u=-\tfrac12\sigma V\alpha+O(\alpha^2)$**. Charge $\sigma\alpha+O(\alpha^2)$ per unit area flows back to the voltage source, which receives energy $\sigma V\alpha+O(\alpha^2)$. The externally supplied mechanical work is still $\tfrac12\sigma V\alpha+O(\alpha^2)$: the field loses half this returned electrical energy and the mechanical work supplies the other half. Thus the [fixed-voltage capacitor energy balance](../../../../../fixed-voltage-capacitor-energy-balance.md) includes both field and source energy.

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
