# Intensive and extensive thermodynamic quantities

↑ **Parent:** [Thermodynamics](thermodynamics-split.md)

An [extensive quantity](extensive-quantity.md) measures how much of a [thermodynamic system](thermodynamic-system.md) there is; an [intensive quantity](intensive-quantity.md) describes its state independently of that amount. The clean comparison is replication: take independent identical systems at the same [thermodynamic equilibrium](thermodynamic-equilibrium.md), with the same substance, composition and [thermodynamic phase](thermodynamic-phase.md). Combining their accounting boundaries multiplies [internal energy](internal-energy-split.md) $U$, [entropy](entropy-split.md) $S$, [volume](volume-thermodynamics.md) $V$, [mass](mass.md) $m$ and [amount of substance](amount-of-substance.md) $n$, while leaving [temperature](temperature-split.md) $T$, [pressure](pressure-split.md) $p$ and [chemical potential](chemical-potential-split.md) $\mu$ unchanged.[Statistical Physics, chapter 1 The Fundamentals of Statistical Mechanics, §1.4.3 Extensive and Intensive Quantities](statistical-physics-by-david-tong.md)

For $\lambda$ copies the ledger is

$$
(U,S,V,m,n)\longmapsto\lambda(U,S,V,m,n),
\qquad (T,p,\mu)\longmapsto(T,p,\mu).
$$

An integer $\lambda$ counts actual copies; a positive real $\lambda$ describes the corresponding bulk scaling law. Copies can remain separated: replication need not involve removing a partition, changing a container or performing any [work](work.md). Distinguish $n$, the [amount of substance](amount-of-substance.md) measured in [moles](mole-unit.md), from $N=nN_A$, the dimensionless count of specified entities, where $N_A$ is the [Avogadro constant](avogadro-constant.md) in $\mathrm{mol}^{-1}$. For example, $2\,\mathrm{mol}$ contains $1.204428152\times10^{24}$ specified entities; tripling it gives $6\,\mathrm{mol}$ and $3.613284456\times10^{24}$ entities. This uses the exact [Avogadro constant](avogadro-constant.md) $N_A=6.02214076\times10^{23}\,\mathrm{mol}^{-1}$, which does not triple. In the differential $dU=T\,dS-p\,dV+\mu\,dn$, $\mu$ is a molar [chemical potential](chemical-potential-split.md) in $\mathrm{J\,mol^{-1}}$; the coefficient of $dN$ instead has units of [energy](energy-split.md) per entity.

<a id="image-replication-multiplies-the-extensive-ledger-while-preserving-the-equilibrium-state"></a>
![](thermodynamic-replication-ledger.png)

**[Figure 21](#image-replication-multiplies-the-extensive-ledger-while-preserving-the-equilibrium-state). Replication multiplies the extensive ledger while preserving the equilibrium state**.

As a direct check, the [ideal gas law](ideal-gas-law.md) $pV=nRT$ gives

$$
p'=\frac{(\lambda n)RT}{\lambda V}=p.
$$

For a monatomic [ideal gas](ideal-gas-split.md) with only translational [degrees of freedom](degree-of-freedom.md) active, [internal energy of an ideal gas](internal-energy-of-an-ideal-gas.md) gives $U=3nRT/2$, so $U'=\lambda U$ at unchanged [temperature](temperature-split.md). Here $R$ is the [molar gas constant](molar-gas-constant.md). The scaling distinction lets a small sample supply an [equation of state](equation-of-state.md) for a much larger amount: material state and inventory become separate questions.

Replication does not mean multiplying every linear dimension by $\lambda$: a geometrically similar container then has $\lambda^3$ times the [volume](volume.md). Nor does it mean combining samples at different states. Equal [temperature](temperature-split.md) establishes [thermal equilibrium](thermal-equilibrium-split.md) but does not imply equal [pressure](pressure-split.md), composition or [mass density](density.md). [Density of a composite system](density-of-a-composite-system.md) makes this distinction concrete.

**Table of contents**

- [Extensive quantity](extensive-quantity.md)
  - [Euler relation in thermodynamics](euler-relation-in-thermodynamics.md)
- [Intensive quantity](intensive-quantity.md)
  - [Normalizing extensive quantities](normalizing-extensive-quantities.md)
    - [Density of a composite system](density-of-a-composite-system.md)
    - [Pycnometer density measurement](pycnometer-density-measurement.md)

## ↑ Ancestors (5)

1. [Thermodynamics](thermodynamics-split.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2/37b/a/solution.md)
- [Temperature](temperature-split.md)
- [Thermodynamic limit](thermodynamic-limit.md)
