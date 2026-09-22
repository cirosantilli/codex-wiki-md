# Serial dilution

↑ **Parent:** [Dilution](dilution.md)

[Serial dilution](serial-dilution.md) repeatedly transfers a measured portion of one well-mixed [chemical solution](solution-chemistry.md) and dilutes that portion to a new final [volume](volume-thermodynamics.md). With transferred [volume](volume-thermodynamics.md) $v_j$ and final [volume](volume-thermodynamics.md) $V_j$ at step $j$, conserved [solute](solute.md) gives

$$
n_j=c_{j-1}v_j,\qquad c_j=\frac{n_j}{V_j}=c_{j-1}\frac{v_j}{V_j},\qquad
c_k=c_0\prod_{j=1}^k\frac{v_j}{V_j}.
$$

This [product](product-of-numbers.md) follows by repeated substitution. Each step conserves the [solute](solute.md) in the portion transferred into its receiving flask, not the entire inventory in the preceding flask. Uniform mixing makes the selected fraction representative.

Continue the original [solution mass and volume bookkeeping](solution-mass-and-volume-bookkeeping.md) example. A $10.00\,\mathrm{mL}$ portion of the $0.2000\,\mathrm{mol\,L^{-1}}$ stock contains $0.002000\,\mathrm{mol}$ of analytical [sodium chloride](sodium-chloride.md), corresponding to $0.11688\,\mathrm g$ before rounding. After [dilution](dilution.md) to $100.0\,\mathrm{mL}$, its [analytical concentration](analytical-concentration.md) is $0.02000\,\mathrm{mol\,L^{-1}}$. A new $5.000\,\mathrm{mL}$ portion of that mixed [chemical solution](solution-chemistry.md) contains $0.0001000\,\mathrm{mol}$; [dilution](dilution.md) to $50.00\,\mathrm{mL}$ gives $0.002000\,\mathrm{mol\,L^{-1}}$. The two factors $10.00/100.0$ and $5.000/50.00$ multiply to $1/100$.

<a id="image-volumetric-solution-dilution-accounting"></a>
![](volumetric-solution-dilution-accounting.png)

**[Figure 2](#image-volumetric-solution-dilution-accounting). Final chemical solution volume and transferred solute in a serial dilution**. Original illustrative account, not experimental data. Calibration marks denote final contained [volumes](volume.md); arrows denote measured portions transferred. The first arrow carries $0.002000\,\mathrm{mol}$; the second carries $0.0001000\,\mathrm{mol}$. Each receiving flask conserves the inventory in its incoming portion. Equal dilution factors give successively tenfold lower [analytical concentrations](analytical-concentration.md).

The remaining stock holds $0.05000-0.002000=0.04800\,\mathrm{mol}$; the remaining first [dilution](dilution.md) holds $0.002000-0.0001000=0.001900\,\mathrm{mol}$. Including the final flask restores the starting inventory:

$$
0.04800+0.001900+0.0001000=0.05000\,\mathrm{mol}.
$$

This is a direct check that making a dilute final sample does not destroy the [solute](solute.md). Most of it remains in earlier vessels.

[Serial dilution](serial-dilution.md) makes a small final [concentration](concentration.md) accessible using measurable portions instead of a single extremely small transfer. Its limitation is that systematic errors propagate: if each transferred [volume](volume-thermodynamics.md) is $1\%$ below its intended value while final [volumes](volume.md) are correct, two steps give $0.99^2=0.9801$ times the intended [concentration](concentration.md), a $1.99\%$ deficit. Repeated readings alone do not remove that bias. The gain in manageable [volume](volume-thermodynamics.md) therefore depends on calibrated transfer and representative mixing.

## ↑ Ancestors (5)

1. [Dilution](dilution.md)
2. [Solution (chemistry)](solution-chemistry.md)
3. [Mixture](mixture-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Beer-Lambert measurement controls](beer-lambert-measurement-controls.md)
- [Serial dilution](serial-dilution.md)
