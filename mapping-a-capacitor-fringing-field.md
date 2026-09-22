# Mapping a capacitor fringing field

↑ **Parent:** [Fringing field of a capacitor](fringing-field-of-a-capacitor.md)

The [Field Mapper Kit (PK-9023), Product Manual 012-04346D by PASCO scientific](field-mapper-kit-pk-9023-product-manual-012-04346d-by-pasco-scientific.md) (p. 3, Parallel plate capacitor) proposes a direct investigation of the plate-length-to-gap ratio using [conductive-paper electric potential mapping](conductive-paper-electric-potential-mapping.md). Its finite straight [electrodes](electrode.md) represent a cross-section of the plates. The apparatus is a gridded resistive sheet on a corkboard, silver-ink [electrodes](electrode.md), pushpin electrical contacts, a $5$–$20\,\mathrm V$ direct supply capable of $25\,\mathrm{mA}$, and a [voltmeter](voltmeter.md) with input [electrical resistance](electrical-resistance.md) at least $10\,\mathrm{M\Omega}$. The manual specifies waiting 20 minutes for the ink to reach its maximum [electrical conductivity](electrical-conductivity.md), then checking each [electrode](electrode.md): its internal voltage drop should be no more than $1\%$ of the applied [electric potential difference](electric-potential-difference.md).[pp. 1–2: required equipment, drying, contacts, electrode-conductivity check](field-mapper-kit-pk-9023-product-manual-012-04346d-by-pasco-scientific.md)

For the readout, keep one [voltmeter](voltmeter.md) lead on the reference [electrode](electrode.md) and scan the other across the sheet. Mark points having the same reading to trace an [equipotential](equipotential.md). A second method holds the two probe tips at a fixed separation and pivots them to find the largest [electric potential difference](electric-potential-difference.md); a suggested separation is one centimetre. Avoid printed grid marks when making contact.[pp. 8–10, Parts III–IV: equipotential tracing and paired-probe field-gradient mapping](charge-equipotential-and-field-mapper-es-9060-instruction-manual-by-pasco-scientific.md)

The inference follows from the measured [electric potential](electric-potential.md), rather than assuming straight [electric field](electric-field.md) lines. With probe separation $\Delta s$ and direction $\widehat{\mathbf t}$, a local [finite difference](finite-difference-split.md) gives

$$
\mathbf E\cdot\widehat{\mathbf t}\simeq-\frac{\phi(P+\Delta s\widehat{\mathbf t})-\phi(P)}{\Delta s}.
$$

An arrow toward rising [electric potential](electric-potential.md) follows $+\nabla\phi$, so it must be reversed to show $\mathbf E$. To investigate the [fringing field of a capacitor](fringing-field-of-a-capacitor.md), compare contours well inside the gap with contours near and beyond the ends, then repeat at a changed gap while keeping the sheet boundary and plate length fixed. Curving contours and an outside [gradient](gradient.md) establish nonuniformity in this planar setup. Compare $-E_y d/V$ at recorded positions to distinguish simple voltage rescaling from geometric changes; no measured values are supplied here.

Additional useful controls are repeat reference readings to detect drift, reversal of supply polarity, and repeating selected readings with reduced probe spacing. Keep contact quality and sheet edges fixed during the aspect-ratio comparison. Finite probe separation averages the [gradient](gradient.md); reducing it improves spatial resolution but magnifies the effect of voltage uncertainty. [Voltmeter loading](voltmeter-loading.md), imperfect ink [electrodes](electrode.md), and inhomogeneous sheet [electrical conductivity](electrical-conductivity.md) can mimic distortions. These proposed checks supplement the manufacturer's electrode check, rather than claiming a completed experiment.

The sheet carries a steady [electric current](electric-current.md). For uniform [electrical conductivity](electrical-conductivity.md), [Ohm's law](ohm-s-law.md) and [electric charge conservation](charge-conservation.md) give the two-dimensional [Laplace equation](laplace-equation.md) away from [electrodes](electrode.md), as explained in [conductive-paper electric potential mapping](conductive-paper-electric-potential-mapping.md). Uncontacted sheet edges have zero normal [electric current](electric-current.md), whereas the diagram model fixes zero outer [electric potential](electric-potential.md). These distinct [boundary conditions](boundary-condition.md) must be matched before a quantitative comparison. The apparatus reveals a planar [electric potential](electric-potential.md) map; it does not directly measure the free-space three-dimensional [capacitance](capacitance.md) of metal plates.

## ↑ Ancestors (7)

1. [Fringing field of a capacitor](fringing-field-of-a-capacitor.md)
2. [Parallel-plate capacitor](parallel-plate-capacitor.md)
3. [Capacitor](capacitor.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
