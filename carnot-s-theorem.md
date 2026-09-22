<h1 id="carnot-s-theorem">Carnot's theorem</h1>

↑ **Parent:** [Second law of thermodynamics](second-law-of-thermodynamics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Carnot's_theorem_(thermodynamics))

No cyclic [heat engine](heat-engine.md) exchanging [heat](heat-split.md) only with two fixed [thermal reservoirs](heat-bath.md) at positive absolute [temperatures](temperature-split.md) $T_h>T_c$ can exceed the [thermal efficiency](thermal-efficiency.md) of an engine whose cycle is a [reversible thermodynamic process](reversible-thermodynamic-process.md) between them. All such reversible engines have the same [thermal efficiency](thermal-efficiency.md), regardless of their working substance. Let $Q_h>0$ be [heat](heat-split.md) absorbed from the hot [thermal reservoir](heat-bath.md) and $Q_c>0$ the magnitude rejected to the cold one. Then

$$
W=Q_h-Q_c,\qquad
\eta=\frac W{Q_h}\le\eta_C=1-\frac{T_c}{T_h}.
$$

The [work](work.md) convention is the one in the [first law of thermodynamics](first-law-of-thermodynamics-split.md): $W>0$ is net output by the engine. Use absolute [thermodynamic temperatures](thermodynamic-temperature.md), such as values in [kelvin](kelvin.md); ratios of readings in [degree Celsius](degree-celsius.md) are invalid because their zero is shifted.

For $T_h=600\,\mathrm K$, $T_c=300\,\mathrm K$ and $Q_h=1000\,\mathrm J$, the maximum [thermal efficiency](thermal-efficiency.md) is $50\%$. A reversible engine delivers $W=500\,\mathrm J$ and rejects $Q_c=500\,\mathrm J$. The [thermal reservoirs](heat-bath.md) have [entropy](entropy-split.md) changes $-1000/600$ and $+500/300\,\mathrm{J\,K^{-1}}$, which cancel. The engine's own [entropy](entropy-split.md) change is zero over its [thermodynamic cycle](thermodynamic-cycle.md).

<a id="image-carnot-engine-energy-transfers-and-the-reversible-cycle-between-600-k-and-300-k"></a>
![](carnot-engine-efficiency.png)

**[Figure 1](#image-carnot-engine-energy-transfers-and-the-reversible-cycle-between-600-k-and-300-k). Carnot engine energy transfers and the reversible cycle between 600 K and 300 K**.

A short derivation now becomes transparent: the [Second law of thermodynamics](second-law-of-thermodynamics-split.md) gives $-Q_h/T_h+Q_c/T_c\ge0$, and the [first law of thermodynamics](first-law-of-thermodynamics-split.md) gives $W=Q_h-Q_c$. Together they yield the bound and, more precisely,

$$
W=Q_h\left(1-\frac{T_c}{T_h}\right)-T_c\Delta S_{\rm tot}.
$$

At fixed $Q_h,T_h,T_c$, every extra unit of total [entropy production](entropy-production.md) reduces output by $T_c$ units of [energy](energy-split.md). [MIT, Maximum heat-engine work](https://web.mit.edu/16.unified/www/FALL/thermodynamics/notes/node44.html)

Fixed [thermal reservoirs](heat-bath.md) are essential. Finite bodies cool and warm, so their initial [temperature](temperature-split.md) ratio cannot be used throughout an entire extraction process. As a computed contrast, the bodies with equal constant [heat capacity](heat-capacity.md) in the [entropy](entropy-split.md) example would reach $T_f=\sqrt{600\times300}=424.26\,\mathrm K$ if a reversible engine extracted [work](work.md) until their [temperatures](temperature-split.md) matched. Zero total [entropy](entropy-split.md) change gives this geometric mean; the [first law of thermodynamics](first-law-of-thermodynamics-split.md) then gives $W_{\max}=C(600+300-2T_f)=5147.19\,\mathrm J$. Direct contact reaches $450\,\mathrm K$ and extracts no [work](work.md).

Carnot's 1824 book asked whether the useful output of machines driven by [heat](heat-split.md) was fundamentally limited and whether changing the working substance could improve that limit. Its reversible comparisons are the historical setting of [Carnot's theorem](carnot-s-theorem.md). Carnot used the then-current caloric picture, treating [heat](heat-split.md) as conserved in its passage through an engine; the modern balance $Q_h-Q_c=W$ should not be read back into that text.[pp. 6–7 and 20–23](reflexions-sur-la-puissance-motrice-du-feu-et-sur-les-machines-propres-a-developper-cette-puissance-by-sadi-carnot.md)

**Table of contents**

- [Thermodynamic temperature](thermodynamic-temperature.md)
- [Carnot cycle](carnot-cycle.md)
  - [Carnot efficiency](carnot-efficiency.md)
  - [Isothermal process](isothermal-process.md)
    - [Isotherm](isotherm.md)
    - [Isothermal ideal-gas work](isothermal-ideal-gas-work.md)
    - [Finite-rate isothermal piston model](finite-rate-isothermal-piston-model.md)
    - [Boyle's law](boyle-s-law.md)
      - [Absolute pressure in Boyle's law](absolute-pressure-in-boyle-s-law.md)
      - [Linearized plot of Boyle's law](linearized-plot-of-boyle-s-law.md)
      - [Gas-syringe measurement of Boyle's law](gas-syringe-measurement-of-boyle-s-law.md)
        - [Gas-syringe dead-volume correction](gas-syringe-dead-volume-correction.md)
    - [Isothermal compression](isothermal-compression.md)
      - [Isothermal gas syringe experiment](isothermal-gas-syringe-experiment.md)
        - [Gas syringe](gas-syringe.md)
    - [Isothermal expansion](isothermal-expansion.md)

## ↑ Ancestors (6)

1. [Second law of thermodynamics](second-law-of-thermodynamics-split.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Carnot cycle](carnot-cycle.md)
- [Carnot's theorem](carnot-s-theorem.md)
- [Coefficient of performance](coefficient-of-performance.md)
- [Degree Celsius](degree-celsius.md)
- [Heat engine](heat-engine.md)
- [Heat-engine calorimetry](heat-engine-calorimetry.md)
- [Heat pump](heat-pump.md)
- [Heat-pump calorimetry](heat-pump-calorimetry.md)
- [Kelvin-Planck statement of the second law](kelvin-planck-statement-of-the-second-law.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-2/section-c/c13/solution.md)
- [Stirling engine](stirling-engine.md)
- [Temperature](temperature-split.md)
- [Thermodynamics](thermodynamics-split.md)
