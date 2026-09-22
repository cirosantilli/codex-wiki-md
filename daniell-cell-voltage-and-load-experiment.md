# Daniell cell voltage and load experiment

↑ **Parent:** [Daniell cell](daniell-cell.md)

The motivating observation is that a [chemical reaction](chemical-reaction-split.md) can produce a signed electrical reading even when its reacting materials occupy separate vessels. UC San Diego's teaching demonstration places a [copper](copper.md) strip in $0.1\,\mathrm{mol\,L^{-1}}$ $\mathrm{CuSO_4}$ and a [zinc](zinc.md) strip in $0.1\,\mathrm{mol\,L^{-1}}$ $\mathrm{ZnSO_4}$, using two $400\,\mathrm{mL}$ beakers with about $300\,\mathrm{mL}$ of [chemical solution](solution-chemistry.md) in each. The strips connect to a voltage meter. Initially there is no ionic connection; the demonstration specifies a zero reading. A filter-paper [salt bridge](salt-bridge.md) containing aqueous $\mathrm{Na_2SO_4}$ then connects the [chemical solutions](solution-chemistry.md). With the meter's positive lead on [copper](copper.md) and negative lead on [zinc](zinc.md), its reported readings are about $+1.1\,\mathrm V$; exchanging the leads reverses the reading. These are observations reported by the university, not data generated for this article. See [UC San Diego, demonstration 9B: apparatus, bridge control and meter polarity](https://chemistryandbiochemistry.ucsd.edu/undergraduate/teaching-labs/demos/demo9b).

The controls answer different questions. Exchanging only the meter leads checks the sign convention; it does not reverse the [chemical reaction](chemical-reaction-split.md) or swap the [anode](anode.md) and [cathode](cathode.md). Interrupting only the [salt bridge](salt-bridge.md) tests the need for an ionic return path. Its absence prevents sustained cell [electric current](electric-current.md), but a very high-input-resistance meter may still show a transient or unstable reading while interfaces store [electric charge](electric-charge-split.md). The zero reading specified for the university's apparatus is therefore not a universal theorem for every meter. Reconnecting the same [salt bridge](salt-bridge.md) distinguishes a reversible interruption from a disconnected wire or exhausted [chemical solution](solution-chemistry.md). This interpretation follows from [electric charge conservation](charge-conservation.md) in a model allowing interfacial [electric charge](electric-charge-split.md) storage; see [IUPAC Gold Book: integral capacitance of an electrode](https://goldbook.iupac.org/terms/view/I03068) for the [capacitance](capacitance.md) associated with [electrode](electrode.md) charge.

To distinguish terminal [electric potential difference](electric-potential-difference.md) from delivered [power](power.md), compare the nearly open-circuit reading with readings across a known [resistor](resistor.md) load. In the nearly open-circuit condition, a meter with input [electrical resistance](electrical-resistance.md) much larger than the cell's effective internal [electrical resistance](electrical-resistance.md) draws little [electric current](electric-current.md). With a load, measure its terminal [electric potential difference](electric-potential-difference.md) $V$ and infer $I=V/R$ using [Ohm's law](ohm-s-law.md); track the readings over [time](time-in-physics.md) and repeat the nearly open-circuit reading afterwards. Keep the [temperature](temperature-split.md), [chemical solution](solution-chemistry.md) compositions, immersed [electrode](electrode.md) areas, bridge geometry and electrical contacts comparable. This is a model-based extension of the documented demonstration, not a claim that UC San Diego published a load sweep. A finite-current drop can reflect ionic [electrical resistance](electrical-resistance.md), changes of interfacial [reaction rates](reaction-rate.md), or depletion near an [electrode](electrode.md); a single voltage reading cannot identify which dominates. The interfacial and composition contributions are distinguished in [IUPAC Gold Book: overpotential](https://goldbook.iupac.org/terms/view/O04358) and [IUPAC Gold Book: concentration overpotential](https://goldbook.iupac.org/terms/view/C01230).

For a deliberately simplified calculation, model the cell by a constant [electromotive force](electromotive-force.md) $\mathcal E$ in series with a constant internal [electrical resistance](electrical-resistance.md) $r$, and a passive load $R>0$. Take $I$ positive from the [cathode](cathode.md) through the load to the [anode](anode.md). Then

$$
I=\frac{\mathcal E}{R+r},\qquad V=IR=\mathcal E-Ir,\qquad P_{\rm load}=IV=I^2R.
$$

The nearly open-circuit limit $R\to\infty$ gives $V\to\mathcal E$ but $I\to0$ and $P_{\rm load}\to0$. A straight $V$-versus-$I$ line is a prediction of constant $r$, not a general law for [electrochemistry](electrochemistry-split.md). See [Ling, Sanny and Moebs, University Physics II, §10.1: internal resistance, terminal voltage and load](https://openstax.org/books/university-physics-volume-2/pages/10-1-electromotive-force).

<a id="image-toy-daniell-cell-load-calculation-terminal-electric-potential-difference-electric-charge-and-available-work"></a>
![](galvanic-electrodes-load-budget.png)

**[Figure 2](#image-toy-daniell-cell-load-calculation-terminal-electric-potential-difference-electric-charge-and-available-work). Toy Daniell cell load calculation: terminal electric potential difference, electric charge and available work**. Calculated line and energy bars, not measurements. Chosen inputs are $\mathcal E=1.10\,\mathrm V$, $r=100\,\Omega$, $R=100\,\Omega$ and a $600\,\mathrm s$ interval. The fixed-composition approximation and unit efficiency for the two intended [half-reactions](half-reaction.md) are assumed. The open-circuit marker is an ideal limit; no fit to experimental data is made.

For the chosen values, $I=5.50\,\mathrm{mA}$ and $V=0.550\,\mathrm V$. Holding these toy parameters fixed for $600\,\mathrm s$ gives transported [electric charge](electric-charge-split.md) $Q=It=3.30\,\mathrm C$ and an [extent of reaction](extent-of-reaction.md) $\xi=Q/(2F)\simeq17.1\,\mathrm{\mu mol}$, assuming all the [electric current](electric-current.md) serves the two specified [half-reactions](half-reaction.md). The same $\xi$ counts [zinc](zinc.md) consumed and [copper](copper.md) deposited, rather than equal [masses](mass.md). The energy budget is

$$
\mathcal E Q=3.630\,\mathrm J
=\underbrace{VQ}_{1.815\,\mathrm J\text{ delivered to load}}
+\underbrace{I^2rt}_{1.815\,\mathrm J\text{ internal dissipation}}.
$$

The load's electrical [work](work.md) also becomes [Joule heating](joule-heating.md) when the load is a [resistor](resistor.md). Here $\mathcal E Q$ accounts for the reaction's available reversible electrical [work](work.md); a full cell thermal budget would also require its thermodynamic [entropy](entropy-split.md) contribution. Real measurements need uncertainty estimates, a specified meter input [electrical resistance](electrical-resistance.md) and calibration, and allowance for changing composition and unwanted [chemical reactions](chemical-reaction-split.md). The toy value $r=100\,\Omega$ is not a measured property of the university's cell.

## ↑ Ancestors (5)

1. [Daniell cell](daniell-cell.md)
2. [Galvanic cell](galvanic-cell.md)
3. [Electrochemistry](electrochemistry-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Electrolytic cell](electrolytic-cell.md)
- [Galvanic cell](galvanic-cell.md)
