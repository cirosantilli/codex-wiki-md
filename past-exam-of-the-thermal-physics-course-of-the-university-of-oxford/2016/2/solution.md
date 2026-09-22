<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In the one-mole [Van der Waals equation](../../../van-der-waals-equation.md), $b>0$ represents [excluded volume](../../../excluded-volume.md): the volume available to molecular motion is $V-b$, rather than $V$. Subtracting $b$ in the denominator therefore increases the repulsive contribution to [pressure](../../../pressure-split.md). The $a>0$ term represents intermolecular attraction, which reduces the outward [momentum flux](../../../momentum-flux.md) at a wall and hence appears as the negative correction $-a/V^2$. The two minus signs do not mean that both physical effects lower [pressure](../../../pressure-split.md).

For a reversible [isothermal process](../../../isothermal-process.md) along a homogeneous gas branch with $V_2>V_1>b$, the [work](../../../work.md) done by the gas is

$$
W_{\rm by}=\int_{V_1}^{V_2}\left(\frac{RT}{V-b}-\frac a{V^2}\right)dV
=\boxed{RT\ln\frac{V_2-b}{V_1-b}+a\left(\frac1{V_2}-\frac1{V_1}\right).}
$$

To find the [internal energy](../../../internal-energy-split.md) change without guessing a caloric law, combine $dU=T\,dS-p\,dV$ with the [Helmholtz free energy](../../../helmholtz-free-energy.md) [Maxwell relation](../../../maxwell-relations.md) $(\partial S/\partial V)_T=(\partial p/\partial T)_V$. This gives

$$
\left(\frac{\partial U}{\partial V}\right)_T=T\left(\frac{\partial p}{\partial T}\right)_V-p=\frac a{V^2}.
$$

Therefore

$$
\boxed{\Delta U=a\left(\frac1{V_1}-\frac1{V_2}\right)>0.}
$$

The attractive contribution $-a/V$ becomes less negative as the gas expands: separating attracting particles requires [energy](../../../energy-split.md). This differs from the [ideal gas](../../../ideal-gas-split.md) result $\Delta U=0$ at fixed [temperature](../../../temperature-split.md). The required [heat](../../../heat-split.md) is $Q=\Delta U+W_{\rm by}=RT\ln[(V_2-b)/(V_1-b)]$. Below the critical [temperature](../../../temperature-split.md), an equilibrium path crossing a liquid–gas coexistence region needs the equilibrium coexistence construction rather than the unstable homogeneous [Van der Waals isotherm](../../../van-der-waals-isotherm.md).

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2016](../../2016-split.md)
3. [Past exam of the thermal physics course of the University of Oxford](../../split.md)
4. [Thermal physics course of the University of Oxford](../../../thermal-physics-course-of-the-university-of-oxford.md)
5. [Year 2 of the physics course of the University of Oxford](../../../year-2-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
