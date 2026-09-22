<h1 id="section-ii/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

**A plausible hypothesis is that broad specificity emerges from a flexible, chemically heterogeneous binding cavity containing overlapping recognition sites, coupled to an energy-driven cycle that exports many different bound molecules.** The cavity recognizes combinations of physical properties rather than one unique chemical structure. Different [substrates](../../../../../substrate-biochemistry.md) can use different subsets of contacts and different routes through the same [multidrug efflux pump](../../../../../multidrug-efflux-pump.md). This is a testable mechanism, not a claim that every pump has identical architecture.

The hypothesis has three parts. First, a large cavity contains patches providing [hydrophobic](../../../../../hydrophobicity.md) contacts, aromatic contacts, [hydrogen bonds](../../../../../hydrogen-bond.md) and [electrostatics](../../../../../electrostatics-split.md). A chemically diverse set of [substrates](../../../../../substrate-biochemistry.md) may share an aromatic region, a charged group or the ability to partition into the [lipid bilayer](../../../../../lipid-bilayer.md). Each can make a favorable but different combination of contacts. Internal [water](../../../../../water.md) can mediate alternative interactions rather than requiring a rigidly preorganized set of donors and acceptors. Second, local side-chain and backbone flexibility allows several cavity shapes. Third, the large-scale transport cycle changes accessibility and affinity so that occupancy of a permissive binding region can be converted into release on the far side.

These ideas have structural precedents. [X-ray crystallography](../../../../../x-ray-crystallography.md) of [AcrB](../../../../../acrb.md) identified an aromatic, multisite drug-binding region and different conformations in its three subunits, consistent with a functional rotation through binding and export states.[Figs. 1–5, substrate contacts, asymmetric trimer and proposed transport cycle](../../../../../crystal-structures-of-a-multidrug-transporter-reveal-a-functionally-rotating-mechanism-by-satoshi-murakami-and-others.md) Further structures distinguished an access pocket and a deeper binding pocket separated by a flexible switch loop.[Figs. 1–4, pocket occupancy and switch-loop architecture](../../../../../transport-of-drugs-by-the-multidrug-transporter-acrb-involves-an-access-and-a-deep-binding-pocket-that-are-separated-by-a-switch-loop-by-thomas-eicher-and-others.md) The observation supports overlapping recognition and staged movement; the proposed energetic and kinetic roles of each contact still require testing. [AcrB](../../../../../acrb.md) is the proton-coupled inner-membrane component of a larger bacterial export assembly, rather than an [ATP](../../../../../adenosine-triphosphate.md)-powered pump by itself.

A [conformational ensemble](../../../../../conformational-ensemble.md) makes the hypothesis quantitative. Let the unbound pump occupy conformations $j$ with probabilities $p_j$, and let [substrate](../../../../../substrate-biochemistry.md) $s$ have an association constant $K_{a,j,s}$ in conformation $j$. If these states equilibrate rapidly before significant transport, a simple equilibrium binding polynomial gives

$$
K_{a,\mathrm{app},s}=\sum_j p_j K_{a,j,s},\qquad \sum_j p_j=1.
$$

The expression follows by adding the bound population contributed by each unbound state at low free [substrate](../../../../../substrate-biochemistry.md) [concentration](../../../../../concentration.md). Distinct [substrates](../../../../../substrate-biochemistry.md) can bind well overall even when their favorable conformations are different. For example, with $p_1=0.9$, $p_2=0.1$, $K_{a,1,s}=10^4\,\mathrm{M^{-1}}$ and $K_{a,2,s}=10^7\,\mathrm{M^{-1}}$, the apparent constant is $1.009\times10^6\,\mathrm{M^{-1}}$. A minority state dominates the binding contribution. These are illustrative numbers, not measured pump parameters. A working pump is driven and may not equilibrate rapidly, so its transport kinetics cannot in general be reduced to this binding expression.

Permissive recognition is compatible with directional transport only when the cycle is coupled to a driving reaction. For an [ATP-binding cassette transporter](../../../../../atp-binding-cassette-transporter.md), [ATP](../../../../../adenosine-triphosphate.md) binding and [ATP hydrolysis](../../../../../atp-hydrolysis.md) couple rearrangement of nucleotide-binding and transmembrane regions. For a proton-driven pump such as [AcrB](../../../../../acrb.md), proton movement down its [electrochemical gradient](../../../../../electrochemical-gradient.md) couples to structural changes. Neither [substrate](../../../../../substrate-biochemistry.md) affinity alone nor random thermal motion supplies sustained uphill transport. In a tightly coupled model exporting one drug molecule while importing $n$ protons, the molar cycle [Gibbs free energy](../../../../../gibbs-free-energy.md) is

$$
\Delta G_{\mathrm{cycle}}=\Delta\mu_{D,\mathrm{out}}+n\Delta\mu_{H,\mathrm{in}},
$$

where

$$
\Delta\mu_{H,\mathrm{in}}=RT\ln\frac{a_{H,\mathrm{in}}}{a_{H,\mathrm{out}}}+F(\psi_{\mathrm{in}}-\psi_{\mathrm{out}}),\qquad
\Delta\mu_{D,\mathrm{out}}=RT\ln\frac{a_{D,\mathrm{out}}}{a_{D,\mathrm{in}}}+z_DF(\psi_{\mathrm{out}}-\psi_{\mathrm{in}}).
$$

Here $a$ denotes dimensionless [thermodynamic activity](../../../../../thermodynamic-activity.md), $F$ the [Faraday constant](../../../../../faraday-constant.md), $\psi$ [electric potential](../../../../../electric-potential.md), and $z_D$ the charge of the transported drug species. Forward operation requires $\Delta G_{\mathrm{cycle}}<0$; equilibrium stall has equality. This states an energetic bound under the stated coupling assumption, not a measured proton-to-drug ratio for [AcrB](../../../../../acrb.md). Mixed [protonation](../../../../../protonation.md) states, coupling slippage and alternative pathways require a more detailed model.

Several predictions distinguish flexible multisite recognition from an indiscriminately sticky cavity. A [mutation](../../../../../mutation.md) removing one aromatic contact should disproportionately affect a subset of [substrates](../../../../../substrate-biochemistry.md) that use that region, while leaving others relatively intact. Altering a common gating element may impair many [substrates](../../../../../substrate-biochemistry.md) despite preserving some equilibrium binding. Rigidifying a flexible recognition loop could narrow the range even when transport of a favored [substrate](../../../../../substrate-biochemistry.md) survives. Different drugs may compete strongly, weakly or asymmetrically depending on overlap and pathway occupancy; failure of simple competitive kinetics would not alone prove distinct sites in a driven, multi-state system.

Test these predictions with a chemically varied panel, including transported compounds and matched nontransported controls. Measure direct transport in [lipid vesicles](../../../../../lipid-vesicle.md) or another defined system while controlling orientation, pump amount, membrane leak and the driving gradient. For a proton-coupled pump, vary [pH](../../../../../ph.md) and [membrane potential](../../../../../membrane-potential-split.md) separately where possible and include an energy-collapse control; establish that the collapse does not merely destroy membrane integrity. For an [ATP](../../../../../adenosine-triphosphate.md)-driven pump include no-[ATP](../../../../../adenosine-triphosphate.md) and hydrolysis-defective controls. Measure binding and driving-energy consumption independently, because drug-stimulated [ATP hydrolysis](../../../../../atp-hydrolysis.md) or proton flow can be uncoupled from productive export. Growth-based resistance alone is insufficient: altered drug uptake, metabolism and expression also change survival.

Use [cryo-electron microscopy](../../../../../cryo-electron-microscopy.md) or [X-ray crystallography](../../../../../x-ray-crystallography.md) with several chemically different drugs to test different contact maps and cavity shapes, then validate those differences by targeted [mutations](../../../../../mutation.md). Confirm expression, assembly, membrane localization and [protein folding](../../../../../protein-folding.md) for every altered pump. [molecular dynamics](../../../../../molecular-dynamics.md) can predict alternative entry routes and local reorganization, but force-field choices, drug [protonation](../../../../../protonation.md) and limited sampling must be varied or checked; a docking score alone is not evidence of transport. [single-molecule Förster resonance energy transfer](../../../../../single-molecule-forster-resonance-energy-transfer.md) or [electron paramagnetic resonance](../../../../../electron-paramagnetic-resonance.md) can test whether different drugs stabilize different dynamic states and whether the driving reaction changes state occupancy.

Finally, membrane partitioning may explain part of the apparent range: a pump can collect chemically varied compounds that share access to the same membrane-facing route. Measure drug partitioning and free aqueous [concentration](../../../../../concentration.md), since equal added concentrations need not give equal local exposure at the pump. **The strongest support would be substrate-specific contact and dynamics changes, preserved transport energetics, and direct export measurements showing that one adaptable recognition apparatus feeds a shared directional cycle.**

## ↑ Ancestors (13)

1. [6](../6.md)
2. [Section II](../../section-ii.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the biochemistry course of the University of Cambridge](../../../../split.md)
6. [Biochemistry course of the University of Cambridge](../../../../../biochemistry-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
