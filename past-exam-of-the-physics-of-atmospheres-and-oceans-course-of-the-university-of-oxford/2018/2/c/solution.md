<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume the added gas mixes throughout the convective column and retain constant [mass absorption coefficient](../../../../mass-absorption-coefficient.md) for the original gas. The original absorber column [mass](../../../../mass.md) is unchanged, so its total effective [optical depth](../../../../optical-depth.md) $D=\tau_\infty$ is unchanged. Under [transparent-gas addition at fixed absorber mass](../../../../transparent-gas-addition-at-fixed-absorber-mass.md), the absorber [mass](../../../../mass.md) fraction becomes $q=p_s/p_a$, and consequently $t=Dp/p_a$. The new radiating [pressure](../../../../pressure-split.md) is $p_{{\rm rad},a}\simeq p_a/D$, even though the ratio of surface to radiating [pressure](../../../../pressure-split.md) stays $D$.

The mixture's [mass](../../../../mass.md)-specific constants are

$$
R_a=\frac{p_sR_g+(p_a-p_s)R_t}{p_a},\qquad
c_{pa}=\frac{p_sc_{pg}+(p_a-p_s)c_{pt}}{p_a}.
$$

These [pressure](../../../../pressure-split.md) weights represent column [mass](../../../../mass.md) fractions, not mole fractions. Repeating the adiabatic argument gives

$$
\boxed{T_{s,a}=T_eD^{R_a/c_{pa}}\simeq T_eD^{R_t/c_{pt}}\quad(p_a\gg p_s).}
$$

At fixed $D>1$, this is warmer than the original surface precisely if

$$
\boxed{\frac{R_a}{c_{pa}}>\frac{R_g}{c_{pg}}
\quad\Longleftrightarrow\quad\frac{R_t}{c_{pt}}>\frac{R_g}{c_{pg}}.}
$$

The equivalence follows by cross multiplication of the positive heat capacities; it holds for any positive added [mass](../../../../mass.md). If the two ratios agree, adding a transparent gas leaves this model's surface [temperature](../../../../temperature-split.md) unchanged. Increased total [pressure](../../../../pressure-split.md) alone is not a new opacity in a model that fixes absorber [mass](../../../../mass.md) and [mass absorption coefficient](../../../../mass-absorption-coefficient.md). [Pressure broadening](../../../../pressure-broadening.md) or [collision-induced absorption](../../../../collision-induced-absorption-and-emission.md) could change the answer in a more realistic atmosphere, but neither is part of the stated constant-opacity model.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
