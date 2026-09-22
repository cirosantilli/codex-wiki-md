<h1 id="18b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the ideal one-dimensional pipe model: constant density, steady inviscid flow, approximately uniform endpoint speeds $u_1,u_2$, and equal body-force potential at the two ends. [Conservation of mass](../../../../../../mass-conservation.md) gives the constant [volumetric flow rate](../../../../../../volumetric-flow-rate.md) $q=u_1S_1=u_2S_2$, and the [mass flow rate](../../../../../../mass-flow-rate.md) is $m=\rho q$. The steady [Bernoulli equation](../../../../../../bernoulli-equation.md) gives

$$
\Delta p=\frac\rho2(u_2^2-u_1^2)=\frac\rho2q^2\left(\frac1{S_2^2}-\frac1{S_1^2}\right).
$$

For flow from a wider to a narrower section, $S_1>S_2$ and $\Delta p>0$. Solving for the positive mass throughput gives the [Venturi effect](../../../../../../venturi-effect.md) formula

$$
\boxed{m=S_1S_2\sqrt{\frac{2\rho\Delta p}{S_1^2-S_2^2}}.}
$$

The formula requires these hydraulic assumptions; steady incompressibility alone does not impose uniform endpoint profiles or equal potential. If $V_1\neq V_2$, the same derivation replaces $\Delta p$ by $\Delta p+\rho(V_1-V_2)$. Viscous losses would also modify the pressure balance. The equal-area case is singular in this pressure-based determination: in the ideal equal-potential model its pressure difference must vanish and does not determine the throughput.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [18B](../../18b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
