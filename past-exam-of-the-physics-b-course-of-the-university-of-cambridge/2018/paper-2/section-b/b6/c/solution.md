<h1 id="section-b/b6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An [electrical transformer](../../../../../../transformer-electrical-engineering.md) transfers alternating electrical [power](../../../../../../power.md) between windings through a shared changing [magnetic flux](../../../../../../magnetic-flux.md). A core with large [magnetic permeability](../../../../../../permeability-electromagnetism.md) confines most of the flux, so both windings link approximately the same flux $\Phi(t)$. [Faraday's law](../../../../../../faraday-s-law-of-induction.md) gives induced electromotive [forces](../../../../../../force-split.md)

$$
\mathcal E_p=-N_p\frac{d\Phi}{dt},\qquad
\mathcal E_s=-N_s\frac{d\Phi}{dt}.
$$

For an ideal [electrical transformer](../../../../../../transformer-electrical-engineering.md), negligible winding resistance and leakage flux imply the terminal-voltage magnitude ratio

$$
\boxed{\frac{V_s}{V_p}=\frac{N_s}{N_p}.}
$$

The relative phase depends on the winding sense and terminal convention. At a loaded secondary, Lenz's law makes the secondary current oppose the flux change. The primary draws an additional current which approximately cancels the secondary magnetomotive [force](../../../../../../force-split.md): $N_pI_p\simeq N_sI_s$ in magnitude when the magnetizing current is negligible. Consequently

$$
\boxed{V_pI_p=V_sI_s,\qquad \frac{I_s}{I_p}=\frac{N_p}{N_s}}
$$

for a resistive load, using [root mean square](../../../../../../root-mean-square.md) values. More generally the ideal device conserves instantaneous [power](../../../../../../power.md), with the appropriate current signs. A load impedance $Z_L$ appears at the primary as $Z_{\rm in}=(N_p/N_s)^2Z_L$, enabling [impedance matching](../../../../../../impedance-matching.md) and electrical isolation.

For sinusoidal flux, $\Phi=\Phi_{\max}\sin\omega t$ gives $V_{\rm rms}=\omega N\Phi_{\max}/\sqrt2$. At a given supply voltage, reducing [frequency](../../../../../../frequency.md) increases the required peak flux and can drive the core into [magnetic saturation](../../../../../../magnetic-saturation.md). Real losses include winding [Joule heating](../../../../../../joule-heating.md), magnetic [hysteresis](../../../../../../hysteresis.md), [eddy currents](../../../../../../eddy-current.md) and leakage flux; a laminated core suppresses eddy-current loops. A steady [direct current](../../../../../../direct-current.md) produces no continuing secondary electromotive [force](../../../../../../force-split.md), while its small winding resistance can allow a damaging primary current after switching transients.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
