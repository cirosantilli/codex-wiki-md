# Glucose mutarotation experiment

↑ **Parent:** [Monosaccharide ring-chain interconversion](monosaccharide-ring-chain-interconversion.md)

An endpoint experiment uses a [polarimeter](polarimeter.md) with a $1.0\,\mathrm{dm}$ sample cell and supplied $4\%$, $6\%$ and $8\%$ D-[glucose](glucose.md) [chemical solutions](solution-chemistry.md). Collect about $15\,\mathrm{mL}$ of each. Fill the cell first with distilled [water](water.md), dry its windows, move bubbles to the air trap, and retain its orientation. Scan [light intensity](light-intensity.md) against [polarimeter analyzer](polarimeter-analyzer.md) [angle](angle.md) through $360^\circ$. The protocol fits a [Gaussian function](gaussian-function.md) to the upper third of a symmetric peak to locate its maximum. Rinse with the next sample, repeat for each [glucose](glucose.md) [chemical solution](solution-chemistry.md), and subtract the [water](water.md) maximum's [angle](angle.md) from each sample maximum. This is an operational peak-location method; the [Gaussian function](gaussian-function.md) is not the physical transmission law.[PASCO, Equilibrium of Sugar Mutarotation, p. 1 path length; pp. 2–4 Materials and Equipment and Procedure 1–18](equilibrium-of-sugar-mutarotation-by-pasco.md)

The existing [optical activity](optical-activity.md) and [polarimetry](polarimetry.md) articles explain the apparatus, [Malus's law](malus-s-law.md) and instrument limitations. For an extension that observes [mutarotation](mutarotation.md) in time, freshly dissolve a specified crystalline [anomer](anomer.md), record the mixing time, and repeat the [optical rotation](optical-rotation.md) readout at fixed [concentration](concentration.md), path length, [wavelength](wavelength.md) and recorded [temperature](temperature-split.md). Keep [pH](ph.md) consistent and record the delay before the first reading. These are proposed additions to the endpoint protocol, not its published steps or a claim of measured results. Recheck the [water](water.md) blank, repeat the preparation, and compare with a separately equilibrated portion under the same conditions. A stable endpoint alone does not show the time evolution.

Interpret each [concentration](concentration.md) separately. If $\theta$ is blank-corrected [optical rotation](optical-rotation.md), $l$ is path length and $c$ is total [glucose](glucose.md) [mass](mass.md) [concentration](concentration.md), first calculate [specific rotation](specific-rotation.md) $r=\theta/(lc)$. In an additive two-[anomer](anomer.md) approximation, let $r_\alpha,r_\beta$ be reference [specific rotations](specific-rotation.md) under the same conditions and $x_\alpha$ the [mole fraction](mole-fraction.md) of alpha within that pair. Equal [molar masses](molar-mass.md) make its [mass](mass.md) fraction equal to $x_\alpha$, so

$$
r=x_\alpha r_\alpha+(1-x_\alpha)r_\beta,\qquad x_\alpha=\frac{r-r_\beta}{r_\alpha-r_\beta}.
$$

This is a population estimate from an assumed response model, not direct imaging of an [anomer](anomer.md). For a simple consistency check, doubling $c$ at fixed $l$ and unchanged composition doubles $\theta$ in this model while leaving $r$ unchanged. Averaging raw [optical rotations](optical-rotation.md) at different [concentrations](concentration.md) would fail this test; normalize first.

Changing [temperature](temperature-split.md), [pH](ph.md), contamination, incomplete dissolution, window stress, bubbles or instrumental drift can imitate or obscure a changing signal. Reference [specific rotations](specific-rotation.md) must match the sample conditions. Minor open-chain and other ring forms limit the two-[anomer](anomer.md) approximation; a single [optical rotation](optical-rotation.md) cannot separately determine every population. Also, these [anomers](anomer.md) are [diastereomers](diastereomer.md), not an [enantiomer](enantiomer.md) pair: the equal-and-opposite cancellation formula for [enantiomeric excess](enantiomeric-excess.md) does not apply.

## ↑ Ancestors (7)

1. [Monosaccharide ring-chain interconversion](monosaccharide-ring-chain-interconversion.md)
2. [Monosaccharide](monosaccharide.md)
3. [Sugar](sugar.md)
4. [Carbohydrate](carbohydrate.md)
5. [Chemical substance](chemical-substance-split.md)
6. [Chemistry](chemistry-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Mutarotation](mutarotation.md)
