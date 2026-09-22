# Kelvin thermoelectric relation

↑ **Parent:** [Peltier coefficient](peltier-coefficient.md)

With the [Seebeck coefficient](seebeck-coefficient.md) convention $dV=-S\,dT$ at zero [electric current](electric-current.md), and the transported-[heat](heat-split.md) convention of [Peltier coefficient](peltier-coefficient.md), the [Kelvin thermoelectric relation](kelvin-thermoelectric-relation.md) is

$$
\Pi(T)=T S(T),\qquad
\Pi_{A\to B}^{\rm abs}(T)=T\bigl[S_B(T)-S_A(T)\bigr].
$$

$T$ is absolute [temperature](temperature-split.md) in [kelvins](kelvin.md); use consistent material references. This scalar [linear response](linear-response-theory.md) relation assumes local [thermal equilibrium](thermal-equilibrium-split.md) and reciprocal transport without time-reversal-breaking fields or order. [Onsager reciprocal relations](onsager-reciprocal-relation.md) supply the symmetry; [conservation of energy](conservation-of-energy.md) alone is insufficient. A [magnetic field](magnetic-field-split.md) requires a reversed-field reciprocity comparison.[A.11.6: reciprocity and the Peltier–Seebeck relation](thermoelectric-effects-by-leon-van-dommelen.md)

In particular, the A-minus-B [thermocouple](thermocouple.md) coefficient in [Seebeck effect](seebeck-effect.md) is $S_A-S_B$, whereas absorbed junction [heat](heat-split.md) for [conventional current](conventional-current.md) A to B uses $S_B-S_A$. There is no contradiction: terminal voltage order and crossing direction are separate choices. Multiplying a measured voltage by an absolute [temperature](temperature-split.md) without specifying these choices does not determine junction heating.

A short reciprocity calculation makes the factor $T$ visible. At a common reference [temperature](temperature-split.md), write the local [linear response](linear-response-theory.md) with electrical driving field $\mathcal E=-\nabla V$ and [heat flux](heat-flux-density.md) $q$ as

$$
j=L_{11}\frac{\mathcal E}{T}+L_{12}\frac{-\nabla T}{T^2},\qquad
q=L_{21}\frac{\mathcal E}{T}+L_{22}\frac{-\nabla T}{T^2}.
$$

At $j=0$, the [Seebeck coefficient](seebeck-coefficient.md) convention gives $S=L_{12}/(T L_{11})$. At $\nabla T=0$, the [Peltier coefficient](peltier-coefficient.md) is $q/j=L_{21}/L_{11}$. Thus $L_{21}=L_{12}$ gives $\Pi=TS$. The chosen forces are conjugate to the fluxes in the local [entropy production](entropy-production.md), $j\mathcal E/T+q(-\nabla T)/T^2$; arbitrary rescaling of just one force would spoil this argument.

The relation is local. Varying $S(T)$ permits distributed [Thomson effect](thomson-effect.md) heating, with $\tau=T\,dS/dT$; the constant-coefficient model below omits it. Endpoint substitutions into a constant-property formula can therefore break its [energy](energy-split.md) accounting.

## ↑ Ancestors (7)

1. [Peltier coefficient](peltier-coefficient.md)
2. [Peltier effect](peltier-effect.md)
3. [Thermoelectric effect](thermoelectric-effect-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Kelvin thermoelectric relation](kelvin-thermoelectric-relation.md)
- [Peltier coefficient](peltier-coefficient.md)
