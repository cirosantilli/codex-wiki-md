<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work in the [shock frame](../../../../../../shock-frame.md), assume a calorically [perfect gas](../../../../../../ideal-gas.md) with fixed [specific-heat ratio](../../../../../../heat-capacity-ratio.md) $\gamma>1$, and neglect magnetic stresses and body forces across the thin shock. The [internal energy](../../../../../../internal-energy.md) per unit mass is $e=p/[(\gamma-1)\rho]$, and the [specific enthalpy](../../../../../../specific-enthalpy.md) is $w=\gamma p/[(\gamma-1)\rho]$. Integrating the local [conservation laws](../../../../../../conservation-law.md) across a thin stationary control volume makes the [mass flux](../../../../../../mass-flux.md) $\rho u$, [momentum flux](../../../../../../momentum-flux.md) $p+\rho u^2$, and [energy flux](../../../../../../energy-flux.md) $u(\rho u^2/2+\gamma p/(\gamma-1))$ continuous. Hence the [Rankine-Hugoniot conditions for a perfect gas](../../../../../../rankine-hugoniot-conditions-for-a-perfect-gas.md) are

$$
\rho_1u_1=\rho_2u_2=m,\qquad p_1+\rho_1u_1^2=p_2+\rho_2u_2^2,\qquad\frac{u_1^2}{2}+\frac{\gamma p_1}{(\gamma-1)\rho_1}=\frac{u_2^2}{2}+\frac{\gamma p_2}{(\gamma-1)\rho_2}.
$$

Multiplication of the last equality by $m$ gives continuity of the stated energy flux. These express that mass, momentum and energy cannot accumulate in an infinitesimally thin steady shock, although [entropy production](../../../../../../entropy-production.md) occurs on the physical compression branch. The same constant in the [polytropic equation of state](../../../../../../polytropic-equation-of-state.md) $p=K\rho^\gamma$ must therefore not be imposed on both sides. For flow from $z>0$ to $z<0$, both signed velocities are negative; the flux equations and ratios remain valid.

In the [Strong-shock Rankine-Hugoniot conditions](../../../../../../strong-shock-rankine-hugoniot-conditions.md), $p_1/(\rho_1u_1^2)=1/(\gamma M_1^2)$ tends to zero. Put $r=\rho_2/\rho_1$. The first two flux balances give $u_2=u_1/r$ and $p_2=\rho_1u_1^2(1-1/r)$ to leading order. The energy balance becomes

$$
\frac12=\frac1{2r^2}+\frac{\gamma}{\gamma-1}\frac{1-1/r}{r},\qquad(r-1)\{(\gamma-1)r-(\gamma+1)\}=0.
$$

Discarding the unchanged-state root $r=1$ gives the compressive [shock compression ratio](../../../../../../shock-compression-ratio.md) and the required limits:

$$
\boxed{\frac{\rho_2}{\rho_1}\longrightarrow\frac{\gamma+1}{\gamma-1},\qquad\frac{u_2}{u_1}\longrightarrow\frac{\gamma-1}{\gamma+1},\qquad\frac{p_2}{\rho_1u_1^2}\longrightarrow\frac2{\gamma+1}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
