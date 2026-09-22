<h1 id="carnot-s-theorem">Carnot's theorem</h1>

↑ **Parent:** [Second law of thermodynamics](second-law-of-thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Carnot's_theorem_(thermodynamics))

No cyclic [heat engine](heat-engine.md) exchanging [heat](heat.md) only with two fixed [thermal reservoirs](heat-bath.md) at positive absolute [temperatures](temperature.md) $T_h>T_c$ can exceed the [thermal efficiency](thermal-efficiency.md) of an engine whose cycle is a [reversible thermodynamic process](reversible-thermodynamic-process.md) between them. All such reversible engines have the same [thermal efficiency](thermal-efficiency.md), regardless of their working substance. Let $Q_h>0$ be [heat](heat.md) absorbed from the hot [thermal reservoir](heat-bath.md) and $Q_c>0$ the magnitude rejected to the cold one. Then

$$
W=Q_h-Q_c,\qquad
\eta=\frac W{Q_h}\le\eta_C=1-\frac{T_c}{T_h}.
$$

The [work](work.md) convention is the one in the [first law of thermodynamics](first-law-of-thermodynamics.md): $W>0$ is net output by the engine. Use absolute [thermodynamic temperatures](thermodynamic-temperature.md), such as values in [kelvin](kelvin.md); ratios of readings in [degree Celsius](degree-celsius.md) are invalid because their zero is shifted.

For $T_h=600\,\mathrm K$, $T_c=300\,\mathrm K$ and $Q_h=1000\,\mathrm J$, the maximum [thermal efficiency](thermal-efficiency.md) is $50\%$. A reversible engine delivers $W=500\,\mathrm J$ and rejects $Q_c=500\,\mathrm J$. The [thermal reservoirs](heat-bath.md) have [entropy](entropy.md) changes $-1000/600$ and $+500/300\,\mathrm{J\,K^{-1}}$, which cancel. The engine's own [entropy](entropy.md) change is zero over its [thermodynamic cycle](thermodynamic-cycle.md).

<a id="image-carnot-engine-energy-transfers-and-the-reversible-cycle-between-600-k-and-300-k"></a>
![](carnot-engine-efficiency.png)

**[Figure 28](#image-carnot-engine-energy-transfers-and-the-reversible-cycle-between-600-k-and-300-k). Carnot engine energy transfers and the reversible cycle between 600 K and 300 K**.

A short derivation now becomes transparent: the [Second law of thermodynamics](second-law-of-thermodynamics.md) gives $-Q_h/T_h+Q_c/T_c\ge0$, and the [first law of thermodynamics](first-law-of-thermodynamics.md) gives $W=Q_h-Q_c$. Together they yield the bound and, more precisely,

$$
W=Q_h\left(1-\frac{T_c}{T_h}\right)-T_c\Delta S_{\rm tot}.
$$

At fixed $Q_h,T_h,T_c$, every extra unit of total [entropy production](entropy-production.md) reduces output by $T_c$ units of [energy](energy.md). [MIT, Maximum heat-engine work](https://web.mit.edu/16.unified/www/FALL/thermodynamics/notes/node44.html)

Fixed [thermal reservoirs](heat-bath.md) are essential. Finite bodies cool and warm, so their initial [temperature](temperature.md) ratio cannot be used throughout an entire extraction process. As a computed contrast, the bodies with equal constant [heat capacity](heat-capacity.md) in the [entropy](entropy.md) example would reach $T_f=\sqrt{600\times300}=424.26\,\mathrm K$ if a reversible engine extracted [work](work.md) until their [temperatures](temperature.md) matched. Zero total [entropy](entropy.md) change gives this geometric mean; the [first law of thermodynamics](first-law-of-thermodynamics.md) then gives $W_{\max}=C(600+300-2T_f)=5147.19\,\mathrm J$. Direct contact reaches $450\,\mathrm K$ and extracts no [work](work.md).

Carnot's 1824 book asked whether the useful output of machines driven by [heat](heat.md) was fundamentally limited and whether changing the working substance could improve that limit. Its reversible comparisons are the historical setting of [Carnot's theorem](carnot-s-theorem.md). Carnot used the then-current caloric picture, treating [heat](heat.md) as conserved in its passage through an engine; the modern balance $Q_h-Q_c=W$ should not be read back into that text.[pp. 6–7 and 20–23](reflexions-sur-la-puissance-motrice-du-feu-et-sur-les-machines-propres-a-developper-cette-puissance-by-sadi-carnot.md)

**Table of contents**

- [Thermodynamic temperature](thermodynamic-temperature.md)
- [Carnot cycle](carnot-cycle.md)
  - [Isothermal process](isothermal-process.md)
    - [Isothermal ideal-gas work](isothermal-ideal-gas-work.md)
    - [Finite-rate isothermal piston model](finite-rate-isothermal-piston-model.md)
    - [Boyle's law](boyle-s-law.md)
    - [Isothermal compression](isothermal-compression.md)
      - [Isothermal gas syringe experiment](isothermal-gas-syringe-experiment.md)
        - [Gas syringe](gas-syringe.md)
    - [Isothermal expansion](isothermal-expansion.md)

## ↑ Ancestors (6)

1. [Second law of thermodynamics](second-law-of-thermodynamics.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Carnot cycle](carnot-cycle.md)
- [Carnot's theorem](carnot-s-theorem.md)
- [Coefficient of performance](coefficient-of-performance.md)
- [Degree Celsius](degree-celsius.md)
- [Heat engine](heat-engine.md)
- [Heat-engine calorimetry](heat-engine-calorimetry.md)
- [Heat pump](heat-pump.md)
- [Heat-pump calorimetry](heat-pump-calorimetry.md)
- [Kelvin-Planck statement of the second law](kelvin-planck-statement-of-the-second-law.md)
- [Stirling engine](stirling-engine.md)
- [Temperature](temperature.md)
- [Thermodynamics](thermodynamics-split.md)
