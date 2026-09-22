# Stoichiometric imbalance in step growth

↑ **Parent:** [Carothers equation](carothers-equation.md)

For a strictly bifunctional $AA+BB$ feed, label the limiting [functional groups](functional-group.md) $A$, set $0<r=A_0/B_0\leq1$, and define $p=J/A_0$ as in [functional-group conversion in step growth](functional-group-conversion-in-step-growth.md). The initial [molecule](molecule.md) count is $N_0=(A_0+B_0)/2$, and each intermolecular join consumes one $A$ and one $B$. Thus

$$
N=\frac{A_0+B_0}{2}-pA_0,\qquad
X_n=\frac{1+r}{1+r-2rp}.
$$

This version of the [Carothers equation](carothers-equation.md) uses limiting-group conversion, not the fraction of all groups reacted.[Introduction, equations (2)–(6), especially the paragraph before equation (3): A is the limiting reactant used to define p](generalization-of-the-carothers-equation-for-linear-step-growth-polymers-by-emilio-meaurio.md)

As an original finite example, mix $95$ $AA$ [monomer molecules](monomer-molecule.md) with $100$ $BB$ [monomer molecules](monomer-molecule.md). Then $(N_0,A_0,B_0)=(195,190,200)$ and $r=0.95$. At $p=0.90$, $171$ joins leave $24$ [molecules](molecule.md), giving $X_n=195/24=8.125$. At $p=1$, $190$ joins leave five chains and ten unreacted $B$ groups; every chain has two $B$ ends, and $X_n=39$. Continuing to wait cannot remove the missing-$A$ constraint within this model.

For $r<1$, complete limiting-group conversion gives the ceiling $X_{n,\max}=(1+r)/(1-r)$. Reaching a target $X_n=K>1$ therefore requires $r\geq(K-1)/(K+1)$, even before considering incomplete conversion. For $K=200$, $r\geq199/201\approx0.99005$. Equality requires $p=1$; any lower conversion demands closer balance. The imbalance $1-r$ is measured relative to the initial number of $B$ groups, not relative to the total number of groups. A monofunctional impurity changes the initial groups-per-[molecule](molecule.md) count, so it cannot be inserted into this strictly bifunctional formula by retaining an unexamined $r$.

<a id="image-step-growth-conversion-stoichiometry-sensitivity"></a>
![](step-growth-conversion-stoichiometry-sensitivity.png)

**[Figure 37](#image-step-growth-conversion-stoichiometry-sensitivity). Carothers equation sensitivity to limiting-group conversion and initial stoichiometric imbalance in step growth**. Original analytic model curves with logarithmic vertical axes. Left: $X_n=(1+r)/(1+r-2rp)$ and the balanced example points. Right: $X_{n,\max}=(1+r)/(1-r)$ versus $100(1-r)$, the initial excess-$B$ fraction relative to $B_0$. These are ideal linear no-ring calculations, not fits to the [polyurethane](polyurethane.md) study.

## ↑ Ancestors (6)

1. [Carothers equation](carothers-equation.md)
2. [Step-growth polymerization](step-growth-polymerization.md)
3. [Polymerization](polymerization.md)
4. [Polymer](polymer.md)
5. [Chemistry](chemistry-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Residual-group monitoring of polyurethane formation](residual-group-monitoring-of-polyurethane-formation.md)
- [Stoichiometric imbalance in step growth](stoichiometric-imbalance-in-step-growth.md)
