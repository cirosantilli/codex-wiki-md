<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the printed [stellar gas-pressure fraction](../../../../../../stellar-gas-pressure-fraction.md), $\beta=P_g/P$, with $P=P_g+P_{\rm rad}$, and keep composition fixed. For a monatomic [perfect gas](../../../../../../ideal-gas.md) plus equilibrium [blackbody radiation](../../../../../../black-body-radiation.md), the [specific heats of a monatomic gas-radiation mixture](../../../../../../specific-heats-of-a-monatomic-gas-radiation-mixture.md) follow from its [specific internal energy](../../../../../../specific-internal-energy.md) and [specific enthalpy](../../../../../../specific-enthalpy.md):

$$
u=\frac32\mathcal RT+\frac{aT^4}{\rho},\qquad h=u+\frac P\rho=\frac52\mathcal RT+\frac{4aT^4}{3\rho}.
$$

At fixed total [pressure](../../../../../../pressure.md), differentiating the equation of state gives

$$
0=\beta\,d\log\rho+(4-3\beta)\,d\log T,\qquad\left(\frac{\partial\log\rho}{\partial\log T}\right)_P=-\frac{4-3\beta}{\beta}.
$$

In particular, $\beta$ is not held constant during that derivative. The [specific heat capacity at constant pressure](../../../../../../specific-heat-capacity-at-constant-pressure.md) is $c_P=(\partial h/\partial T)_P$, so

$$
c_P=\frac52\mathcal R+\frac{4aT^3}{3\rho}\left(4+\frac{4-3\beta}{\beta}\right).
$$

Since $aT^3/(3\rho)=\mathcal R(1-\beta)/\beta$, this simplifies to

$$
\boxed{c_P=\frac{\mathcal R}{2\beta^2}(32-24\beta-3\beta^2)=\frac{k}{2\mu H\beta^2}(32-24\beta-3\beta^2).}
$$

The pure-gas limit is $5\mathcal R/2$. For a gas with unspecified molecular degrees of freedom, replace $3\mathcal R/2$ in $u$ by its gas heat capacity $c_{V,g}$: then $c_P=c_{V,g}+\mathcal R+4\mathcal R(1-\beta)(4+\beta)/\beta^2$. The boxed formula uses the conventional monatomic stellar-gas interpretation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
