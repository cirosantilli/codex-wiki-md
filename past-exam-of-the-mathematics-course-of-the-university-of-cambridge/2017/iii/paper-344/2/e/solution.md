<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the intended regular scaling ansatz: $g(u)\sim C u^y$, $g'(u)\sim Cy u^{y-1}$ and $g''(u)=Cy(y-1)u^{y-2}+o(u^{y-2})$, with $C>0$, $y>0$. Relative to the drag magnitude $g'$, the two inertial contributions obey

$$
\frac{g''}{g'}\sim\frac{y-1}{u},\qquad \frac{g'^2/g}{g'}=\frac{g'}g\sim\frac yu.
$$

Thus both inertial-to-drag ratios tend to zero at large $u$, whatever the positive growth exponent; for $y=1$ the leading acceleration term vanishes identically. The long-time [drag-limited hydrodynamic coarsening](../../../../../../drag-limited-hydrodynamic-coarsening.md) balance is therefore

$$
c_dg'\sim\frac{c_s}{g^2},\qquad g^3(u)\sim3\frac{c_s}{c_d}u,
$$

so

$$
\boxed{g(u)\sim\left(3c_su/c_d\right)^{1/3},\qquad L(t)\sim\left(3\frac{c_s}{c_d}\frac\sigma{\bar\eta}t\right)^{1/3}.}
$$

The leading law is independent of [mass density](../../../../../../density.md). Within the drag-capillary reduction, finite initial data give $L^3(t)-L^3(t_*)=3(c_s/c_d)(\sigma/\bar\eta)(t-t_*)$.

The [derivative](../../../../../../derivative.md) hypotheses are important: bare $g(u)\sim u^y$ does not justify differentiating an asymptotic equivalence. For instance, $g(u)=u+\tfrac12\int_1^u\sin(s^3)\,ds$ is smooth and increasing, with $g(u)/u\to1$, but $g''=\tfrac32u^2\cos(u^3)$ is not small compared with $g'=1+\tfrac12\sin(u^3)$. This is a counterexample to an inference from the bare asymptotic relation, not a solution of the coarsening equation. The physical claim uses the regular self-similar power law, for which the ratio calculation above applies.

This conclusion concerns the model's advective drag-capillary channel. Diffusive [Ostwald ripening](../../../../../../ostwald-ripening.md) can also have a $1/3$ growth exponent; equality of exponents does not establish that diffusion is negligible. If it is retained, the prefactor and crossover function may also depend on [order-parameter mobility](../../../../../../order-parameter-mobility.md), and one must compare transport mechanisms rather than infer the mechanism from the exponent alone.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
