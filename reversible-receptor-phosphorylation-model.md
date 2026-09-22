# Reversible receptor phosphorylation model

↑ **Parent:** [Receptor tyrosine kinase](receptor-tyrosine-kinase.md)

[Protein kinase](protein-kinase.md) activity adds modification, while [protein tyrosine phosphatase](protein-tyrosine-phosphatase.md) activity can remove it. An original one-site model shows why a [receptor phosphorylation assay](receptor-phosphorylation-assay.md) cannot determine either process from a single modified fraction. Let $f(t)\in[0,1]$ be the fraction of a fixed [receptor](receptor-biochemistry.md) population carrying one selected [phosphotyrosine residue](phosphotyrosine-residue.md). Stipulate constant effective first-order [rate constants](rate-constant.md) $k_+,k_->0$, with [ATP](adenosine-triphosphate.md) availability absorbed into $k_+$, and no [receptor](receptor-biochemistry.md) synthesis, degradation or trafficking:

$$
\frac{df}{dt}=k_+(1-f)-k_-f,\qquad
f_* = \frac{k_+}{k_++k_-},\qquad
\tau=\frac{1}{k_++k_-}.
$$

Here $f_*$ is the [steady state](steady-state.md) fraction and $\tau$ the [time constant](time-constant.md). The [ordinary differential equation](ordinary-differential-equation.md) has the [exponential function](exponential-function.md) solution

$$
f(t)=f_*+(f(0)-f_*)e^{-t/\tau}.
$$

The balance equation and a single relaxation step give this result; it is an illustrative model, rather than a fit or a claim about every [RTK](receptor-tyrosine-kinase.md).

With stipulated [rate constants](rate-constant.md) $(k_+,k_-)=(2,1)\,\mathrm{min}^{-1}$, $f_*=2/3$ and $\tau=1/3\,\mathrm{min}$. Doubling both [rate constants](rate-constant.md) leaves $f_*=2/3$ but changes $\tau$ to $1/6\,\mathrm{min}$. The balanced [phosphate](phosphate.md) turnover per site,

$$
J_*=k_+(1-f_*)=k_-f_*=\frac{k_+k_-}{k_++k_-},
$$

doubles from $2/3$ to $4/3\,\mathrm{min}^{-1}$. Identical [steady state](steady-state.md) modification therefore permits different catalytic fluxes. Removing the addition term instead gives $f(t)=f(0)e^{-k_-t}$; this illustrates why a perturbation that stops [protein kinase](protein-kinase.md) activity can expose removal dynamics, subject to the model's unchanged-removal assumption. A maintained [steady state](steady-state.md) with ongoing [ATP](adenosine-triphosphate.md) consumption is not [chemical equilibrium](chemical-equilibrium.md).

## ↑ Ancestors (6)

1. [Receptor tyrosine kinase](receptor-tyrosine-kinase.md)
2. [Cell-surface receptor](cell-surface-receptor.md)
3. [Receptor (biochemistry)](receptor-biochemistry.md)
4. [Protein](protein.md)
5. [Biology](biology-split.md)
6. [Codex Wiki](split.md)
