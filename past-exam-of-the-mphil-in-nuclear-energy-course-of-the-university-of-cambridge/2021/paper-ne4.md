# Module NE4

↑ **Parent:** [2021](../2021.md)

Original worked solutions cover all four printed questions, including the optional choices. The source is the University of Cambridge release at physical PDF pages 90–95; the questions occupy pages 91–94. [Original public PDF, physical pages 90–95](https://www.whatdotheyknow.com/request/past_exam_papers_16/response/2088673/attach/3/FOI%202022%20471%20Smith%20materials.pdf?cookie_passthrough=1#page=90)

The chemical-separation answer is deliberately conceptual. Numerical answers state their accounting and gas-residence assumptions at the affected parts.

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Module NE4](paper-ne4.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The distinction is between **partitioning reusable fuel constituents from fission-product waste**, and subsequently **partitioning [uranium](../../chemical-substance.md#uranium) from [plutonium](../../chemical-substance.md#plutonium)**. In the first operation, chemical selectivity transfers selected [actinides](../../chemical-substance.md#actinide) into a different stream while most [fission products](../../physics.md#fission-product) remain in the waste stream. In the second, differences in [chemical speciation](../../mixture.md#chemical-speciation) allow the two recovered elements to follow different streams. Neither operation separates [uranium](../../chemical-substance.md#uranium) [isotopes](../../chemical-substance.md#isotope): [uranium enrichment](../../engineering.md#uranium-enrichment) and chemical element separation are different tasks.

At a conceptual level, [solvent extraction](../../engineering.md#solvent-extraction) exploits unequal affinities of dissolved species for immiscible liquid phases. [complexation](../../chemistry.md#complexation) changes those affinities, while a change in [oxidation state](../../chemical-reaction.md#oxidation-state) can change an element's preferred phase without changing its identity. This explains why a stream bearing [actinides](../../chemical-substance.md#actinide) can first be separated from much of its accompanying waste, and why [uranium](../../chemical-substance.md#uranium) and [plutonium](../../chemical-substance.md#plutonium) need not subsequently remain together. Dissolved and undissolved residues, contaminated solvents and off-gases remain waste-management obligations; a recovery percentage alone is not a complete material balance.

Equipment must provide phase contact and phase disengagement within shielded, confined systems. Remotely maintained contactors and settlers are equipment categories serving those functions; sealed transfer systems, shielded cells and monitored off-gas handling limit contamination and exposure. Cooling manages residual [decay heat](../../physics.md#decay-heat), and [nuclear material accountancy](../../engineering.md#nuclear-material-accountancy) follows inventories and losses. [criticality control in radioactive waste](../../engineering.md#criticality-control-in-radioactive-waste) is essential because [solvent extraction](../../engineering.md#solvent-extraction) can redistribute fissile constituents. **Scoped limitation:** this answer gives the chemical principles and equipment functions; operational fissile-separation recipes, reagent sequences, contactor design details and process conditions are intentionally not supplied.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

[burnup](../../engineering.md#nuclear-fuel-burnup) refers to thermal energy per initial heavy-metal mass. Correct the electrical rating for [thermal efficiency](../../thermodynamics.md#thermal-efficiency) before using it, and apply the [capacity factor](../../physics.md#capacity-factor) once:

$$
P_{\rm th}=\frac{1600}{0.33}=4848.48 \mathrm{MW},\qquad
E_{\rm th}=P_{\rm th}(365)(0.9)=1.592727\times10^6 \mathrm{MW\,d\,yr^{-1}}.
$$

Consequently the annual initial heavy-metal fuel requirement is

$$
M=\frac{E_{\rm th}}{45000}=\boxed{35.394 \mathrm{t\,HM\,yr^{-1}}}.
$$

Let $F,P,W$ be feed, enriched product and [enrichment tails](../../engineering.md#enrichment-tails) masses, all measured as [uranium](../../chemical-substance.md#uranium), and $x_f,x_p,x_w$ the corresponding [uranium-235](../../chemical-substance.md#uranium-235) [mass fractions](../../mixture.md#mass-fraction). The [isotopic mass balance](../../continuum-mechanics.md#isotopic-mass-balance) gives

$$
F=P+W,\qquad Fx_f=Px_p+Wx_w,\qquad
\frac FP=\frac{x_p-x_w}{x_f-x_w}=\frac{0.040-0.003}{0.007-0.003}=9.25.
$$

With $P=M$, the [uranium oxide concentrate](../../engineering.md#uranium-oxide-concentrate) requirement is therefore

$$
F=9.25M=\boxed{327.394 \mathrm{t\,U\,yr^{-1}}},\qquad W=292.000 \mathrm{t\,U\,yr^{-1}}.
$$

These are [uranium](../../chemical-substance.md#uranium) or heavy-metal masses, **not tonnes of [uranium](../../chemical-substance.md#uranium) oxide**. The check $327.394(0.007)=35.394(0.040)+292.000(0.003)$ closes the [uranium-235](../../chemical-substance.md#uranium-235) balance as well as the total mass balance.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use the recovered [uranium](../../chemical-substance.md#uranium) inventory, rather than the initial fuel mass, as the recycle feed. Its available mass is

$$
F_r=33(1-0.015)=32.505 \mathrm{t\,U\,yr^{-1}}.
$$

Assuming the same [enrichment tails](../../engineering.md#enrichment-tails) assay and the specified higher recycled-fuel assay, the [isotopic mass balance](../../continuum-mechanics.md#isotopic-mass-balance) gives

$$
P_r=F_r\frac{0.0085-0.003}{0.043-0.003}=4.4694375 \mathrm{t\,U\,yr^{-1}},\qquad W_r=28.0355625 \mathrm{t\,U\,yr^{-1}}.
$$

Treat this fuel as replacing the same heavy-metal mass of ordinary fresh fuel: the stipulated higher [uranium-235](../../chemical-substance.md#uranium-235) content compensates for [uranium-236](../../chemical-substance.md#uranium-236). The displaced natural feed is

$$
\Delta F=9.25P_r=\boxed{41.3423 \mathrm{t\,U\,yr^{-1}}},
$$

about **12.63% of the once-through natural-uranium requirement**. The residual natural feed demand is $286.052 \mathrm{t\,U\,yr^{-1}}$.

For separative work accounting define

$$
V(x)=(1-2x)\ln\frac{1-x}{x},\qquad S=PV(x_p)+WV(x_w)-FV(x_f).
$$

Using kilograms in this expression gives kg-SWU. For ordinary fresh fuel the work per product kilogram is

$$
s_f=V(0.040)+8.25V(0.003)-9.25V(0.007)=5.34661 \mathrm{kg\!\text{-}\!SWU\,kg^{-1}}.
$$

The fresh work avoided by substituting $P_r$ is $23896.3 \mathrm{kg\!\text{-}\!SWU\,yr^{-1}}$, but producing that recycled product still requires

$$
S_r=1000\big[P_rV(0.043)+W_rV(0.003)-F_rV(0.0085)\big]
=22409.6 \mathrm{kg\!\text{-}\!SWU\,yr^{-1}}.
$$

Hence the **net** saving is

$$
\Delta S=1000P_rs_f-S_r=\boxed{1486.73 \mathrm{kg\!\text{-}\!SWU\,yr^{-1}}}.
$$

The work saving is only about **0.786%** of the original annual separative work. Crediting the whole avoided fresh-fuel work without charging the recycle work would substantially overstate the saving. This is an annual resource account at the supplied assays, with no isotope-separation equipment model.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

An economic threshold requires all unit costs to have an explicit mass basis. Let $p_U$ be the concentrate price per kilogram of [uranium](../../chemical-substance.md#uranium), and let $C_{\rm net}$ denote the annual incremental fabrication-and-disposal cost of the closed cycle relative to the open cycle. The break-even annual cash balance is

$$
p_U(41342.2969)+50(1486.7266)=1000M_{\rm rep}+C_{\rm net},
$$

where $M_{\rm rep}$ is the charged [nuclear fuel reprocessing](../../engineering.md#nuclear-fuel-reprocessing) throughput in kilograms of initial heavy metal. Use $M_{\rm rep}=35393.9394$: the stated $33$ tonnes is the remaining [uranium](../../chemical-substance.md#uranium) inventory, not the whole initial heavy-metal throughput. Thus

$$
\boxed{p_U=\frac{35393939.4+C_{\rm net}-74336.3}{41342.2969} \mathrm{dollars\,kg_U^{-1}}}.
$$

If the quoted combined $400$ dollars per kilogram is a **net additional charge on that same reprocessed-HM basis**, $C_{\rm net}=400M_{\rm rep}$, giving **1,196.77 dollars per kg U**. Under this explicit convention, the saving in purchased separative work is small and the resource saving must pay nearly all the additional [nuclear fuel reprocessing](../../engineering.md#nuclear-fuel-reprocessing) cost.

The wording does not identify the mass basis or counterfactual sign of the combined recycled-fuel and spent-fuel-disposal term. If instead $400$ dollars is a net charge per kilogram of the $4469.4375$ kg recycled product, the same balance gives **897.56 dollars per kg U**. If it denotes a net avoided charge of $400$ dollars per kilogram of discharged HM, the threshold is **511.87 dollars per kg U**. These are alternative accounting conventions, not three simultaneous economic thresholds; the general balance makes the ambiguity visible.

All prices here are per [uranium](../../chemical-substance.md#uranium) mass, not per gross concentrate mass. This simplified comparison assigns no [plutonium](../../chemical-substance.md#plutonium) credit, financing, conversion-cost difference or change in repository liability, and takes the quoted charges as incremental. A closed fuel cycle can save natural [uranium](../../chemical-substance.md#uranium) without being the cheaper option: at a price below the threshold under the chosen cost convention, the additional charges exceed the resource credit. No contemporary uranium-market price is needed for that conclusion.

## 2

↑ **Parent:** [Module NE4](paper-ne4.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

**[evaporation](../../critical-phenomenon.md#evaporation)** transfers water to a vapour stream and retains mainly nonvolatile solutes in a concentrate. It can give substantial volume reduction and works across many dissolved-solute compositions. Its disadvantages are heat demand, scaling and [corrosion](../../engineering.md#corrosion); [aerosols](../../chemistry.md#aerosol), entrainment or volatile radioactive species can contaminate the condensate. Condensate must therefore be sampled or monitored rather than assumed releasable, while the concentrate requires [radioactive waste conditioning](../../engineering.md#radioactive-waste-conditioning). A demister limits droplet carryover but does not remove a genuinely volatile contaminant.

**[ion exchange](../../engineering.md#ion-exchange)** transfers dissolved radioactive [ions](../../chemistry.md#ion) to an exchanger, often an [ion-exchange resin](../../engineering.md#ion-exchange-resin). It is useful for polishing relatively dilute aqueous streams and can provide selective removal without evaporating the bulk water. Competing inactive [ions](../../chemistry.md#ion) consume capacity, suspended particles foul the bed, and a neutral or poorly retained species may pass through. Breakthrough measurements determine when the exchanger ceases to meet its target; exhausted resin or regeneration liquors become secondary [radioactive waste](../../engineering.md#radioactive-waste). Separation performance must be established for the actual feed chemistry, not inferred from the name of the radionuclide alone.

**Chemical [precipitation](../../chemical-reaction.md#precipitation-chemistry) with solid–liquid separation** uses [precipitation](../../chemical-reaction.md#precipitation-chemistry), [coprecipitation](../../chemical-reaction.md#coprecipitation) and [adsorption](../../physical-chemistry.md#adsorption) to carry contaminants into solids, followed by settling or [filtration](../../mixture.md#filtration-chemistry). It can treat substantial volumes and complex feeds at moderate equipment cost. Its disadvantages are a relatively bulky sludge, incomplete removal of soluble species, and sensitivity to [pH](../../acid-base-chemistry.md#ph), [complexation](../../chemistry.md#complexation) and competing [ions](../../chemistry.md#ion). The sludge must be dewatered and conditioned, and the clarified liquid checked for residual [radioactive activity](../../physics.md#radioactive-activity). Polishing by another method may still be needed.

In each case, measure both the treated stream and the residue so that the radioactive inventory balance can be checked. Treatment transfers or concentrates [radioactive activity](../../physics.md#radioactive-activity); **only [radioactive decay](../../physics.md#radioactive-decay) reduces the number of radioactive parent nuclei**. These methods and the distinction between treatment and conditioning are set out in the institutional waste-management framework.[SSG-40, section 6, especially paragraph 6.42 and the liquid-waste treatment discussion](../../engineering.md#predisposal-management-of-radioactive-waste-from-nuclear-power-plants-and-research-reactors-by-the-international-atomic-energy-agency)

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The useful mechanism is [radioactive decay](../../physics.md#radioactive-decay) during retention, not chemical destruction of [carbon dioxide](../../chemical-substance.md#carbon-dioxide). With the time in seconds,

$$
\lambda=\frac{\ln 2}{20.3(60)}=5.69086\times10^{-4} \mathrm{s^{-1}},\qquad
a(t)=10^{14}e^{-\lambda t} \mathrm{Bq\,m^{-3}}.
$$

Here $a$ is a [radioactive activity concentration](../../physics.md#radioactive-activity-concentration); the supplied units are per volume rather than per mass. The original plot follows this [concentration](../../mathematical-physics.md#concentration) over four hours.

<a id="2/b/image-carbon-11-activity-concentration-during-ideal-radioactive-gas-holdup"></a>
![](../../past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge/2021/paper-ne4-carbon11-delay.png)

**[Figure 1](#2/b/image-carbon-11-activity-concentration-during-ideal-radioactive-gas-holdup). Carbon-11 activity concentration during ideal radioactive gas holdup**.

A practical illustrative choice is **a three-hour guaranteed [residence time](../../engineering.md#residence-time)**, at which $a/a_0=0.00214175$, giving about a factor $467$ reduction. On a plug-flow basis, the carbon-dioxide-equivalent hold-up volume is

$$
V_{\mathrm{CO_2}}=Q\tau=(3.7\times10^{-7})(3\times3600)=\boxed{3.996\times10^{-3} \mathrm{m^3}=4.00 \mathrm L}.
$$

Use a contained delay line or a validated retention arrangement that prevents early breakthrough, followed by monitored discharge. A retention bed could instead hold the radioactive [carbon dioxide](../../chemical-substance.md#carbon-dioxide), but its capacity and breakthrough performance would have to be established. Gas retention and monitored discharge are waste-treatment functions, independent of the eventual use of the [isotope](../../chemical-substance.md#isotope).[SSG-40, section 6, gaseous-waste treatment and selection of decay devices](../../engineering.md#predisposal-management-of-radioactive-waste-from-nuclear-power-plants-and-research-reactors-by-the-international-atomic-energy-agency)

**The $4.00$ L result is a flow-delay volume, not a fill-and-immediately-dump tank specification.** It credits [radioactive decay](../../physics.md#radioactive-decay) during the guaranteed transit time and no subsequent storage after discharge from the delay system. Gas entering a filling tank near the end of filling has not aged for the entire filling time. For a literal tank filled for $T$ and immediately emptied, the [radioactive activity](../../physics.md#radioactive-activity) at emptying is instead

$$
A_{\rm fill}(T)=\int_0^T a_0Qe^{-\lambda(T-s)}\,ds=\frac{a_0Q}{\lambda}(1-e^{-\lambda T}).
$$

That alternative must not be analysed by multiplying the whole collected inventory by $e^{-\lambda T}$. If “no post filling [radioactive decay](../../physics.md#radioactive-decay)” is intended to prescribe this literal fill-and-dump arrangement, the three-hour calculation does not establish compliance for it.

The [nitrogen](../../chemical-substance.md#nitrogen) fraction is also unspecified. If $y$ is the [carbon dioxide](../../chemical-substance.md#carbon-dioxide) volume fraction at the stated volume reference conditions, a gas delay line requires $V_{\rm mixture}=V_{\mathrm{CO_2}}/y$, not necessarily $4.00$ L of physical vessel volume. The graph alone does not define a unique optimum: a cost objective, operating calendar and residence-time model are needed. Parts (c) and (d) quantify the discharge constraint for the stated guaranteed-delay design.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For six hours of operation at the maximum stated carbon-dioxide-equivalent flow, the daily input volume and untreated [radioactive activity](../../physics.md#radioactive-activity) inventory are

$$
V_d=Q(6)(3600)=7.992\times10^{-3} \mathrm{m^3},\qquad
D_{d,0}=a_0V_d=7.992\times10^{11} \mathrm{Bq}.
$$

For the three-hour guaranteed delay, every element of the incoming stream acquires the same [radioactive decay](../../physics.md#radioactive-decay) factor. The [radioactive activity](../../physics.md#radioactive-activity) released per operating day, attributing the delayed tail to its production day, is

$$
D_d=D_{d,0}e^{-\lambda(10800)}=\boxed{1.712\times10^9 \mathrm{Bq}}.
$$

Even on the conservative assumption of operation on all $365$ days,

$$
D_y=365D_d=\boxed{6.248\times10^{11} \mathrm{Bq\,yr^{-1}}},
$$

so the annual discharge is below the supplied $10^{12}$ Bq limit. For $250$ operating days it is $4.279\times10^{11}$ Bq. This sums [radioactive activity](../../physics.md#radioactive-activity) inventories discharged over the year; it does not credit [radioactive decay](../../physics.md#radioactive-decay) in the environment after release. It also retains the final delayed gas after production stops, rather than bypassing the retention system to empty it.

The residence-time qualification matters numerically. A single tank filled for six hours and released immediately, with [radioactive decay](../../physics.md#radioactive-decay) during filling but no later hold, would contain

$$
A_{\rm fill}(21600)=6.502\times10^{10} \mathrm{Bq}.
$$

Repeating that operation on $250$ days releases $1.625\times10^{13}$ Bq, **above the limit**. A well-mixed or fill-and-dump system therefore cannot inherit the plug-flow compliance result just because its nominal volume divided by flow equals the selected delay time. The total [nitrogen](../../chemical-substance.md#nitrogen) flow and any unretained radioactive carbon species must also be included in a real measured release account.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For the ideal guaranteed-delay model, the total untreated yearly input at $250$ operating days is

$$
D_{y,0}=250(7.992\times10^{11})=1.998\times10^{14} \mathrm{Bq}.
$$

Since the discharge is a decreasing function of the [residence time](../../engineering.md#residence-time), the minimum is obtained at equality:

$$
D_{y,0}e^{-\lambda\tau_{\min}}=10^{12},\qquad
\tau_{\min}=\frac{\ln(199.8)}{\lambda}=9308.46 \mathrm s
=\boxed{155.14 \mathrm{min}=2.586 \mathrm h}.
$$

This is $7.642$ [half-lives](../../analysis.md#half-life) and corresponds to **$3.444$ L of carbon-dioxide-equivalent delay volume**. The three-hour choice provides margin; operating every day instead would require at least $166.22$ minutes under the same assumptions.

This minimum is conditional on a guaranteed [residence time](../../engineering.md#residence-time). More generally the surviving fraction is

$$
\frac{a_{\rm out}}{a_0}=\int_0^\infty E(t)e^{-\lambda t}\,dt,
$$

where $E(t)$ is the [residence time distribution](../../engineering.md#residence-time-distribution). Because the [exponential function](../../calculus.md#exponential-function) is [convex function](../../real-analysis.md#convex-function), a spread of transit times gives more surviving [radioactive activity](../../physics.md#radioactive-activity) than [plug flow](../../engineering.md#plug-flow) at the same mean time. A perfectly mixed continuously flowing vessel has a steady-state survival fraction $1/(1+\lambda V/Q)$, not $e^{-\lambda V/Q}$. Thus no unique minimum _tank filling time_ follows without specifying the filling, retention and emptying schedule. The boxed minimum applies to the explicitly specified delay system, and must not be represented as approval of an unspecified tank.

## 3

↑ **Parent:** [Module NE4](paper-ne4.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

**[Synroc](../../engineering.md#synroc) immobilises waste [ions](../../chemistry.md#ion) in selected durable crystalline hosts**, rather than trying to put the whole inventory into one universal site. The underlying philosophy is that [minerals](../../planetary-science.md#mineral) retaining analogous elements over geological times suggest useful [crystal structures](../../physical-chemistry.md#crystal-structure) for engineered containment. These natural analogues motivate the choice; their survival does not prove that every synthetic composition, damaged microstructure or groundwater environment will behave identically. This was the rationale of the original mineral-analogue proposal.[Nature 278, 219–223, abstract and mineral-analogue argument](../../engineering.md#immobilisation-of-high-level-nuclear-reactor-wastes-in-synroc-by-a-e-ringwood-and-others)

A representative [Synroc-C](../../engineering.md#synroc-c) assemblage includes [zirconolite](../../planetary-science.md#zirconolite), $\mathrm{CaZrTi_2O_7}$, as an [actinide](../../chemical-substance.md#actinide) host; a [hollandite waste-form phase](../../engineering.md#hollandite-waste-form-phase), represented by $\mathrm{BaAl_2Ti_6O_{16}}$, whose tunnels accommodate large [cations](../../chemistry.md#cation) such as [caesium](../../chemical-substance.md#caesium); and a [perovskite waste-form phase](../../engineering.md#perovskite-waste-form-phase), $\mathrm{CaTiO_3}$, which can accept [strontium](../../chemical-substance.md#strontium) on [calcium](../../chemical-substance.md#calcium) sites and other constituents with suitable [charge compensation in a crystal](../../chemical-substance.md#charge-compensation-in-a-crystal). Titanium-oxide phases provide additional accommodation and composition flexibility. The actual phases are [solid solutions](../../chemical-substance.md#solid-solution), not simply pure end-member [minerals](../../planetary-science.md#mineral) mixed with an inert waste powder.[Key Engineering Materials 48–50, 717–721; ANSTO abstract identifying the multiphase titanate assemblage](../../engineering.md#crystal-chemistry-and-phase-manipulation-in-synroc-by-e-r-vance-and-others)

Manufacture combines a characterised waste feed with selected oxide-forming precursors, converts the mixture to a suitable powder or [calcination](../../engineering.md#calcination) product, and consolidates it while forming the host phases. [hot pressing](../../engineering.md#hot-pressing) and [hot isostatic pressing](../../engineering.md#hot-isostatic-pressing) are consolidation approaches; the latter uses pressure acting approximately equally in all directions. The objective is a dense [ceramic](../../engineering.md#ceramic) with the intended phase assemblage and low connected [porosity](../../porous-media-flow.md#porosity), contained in an appropriate [radioactive waste package](../../engineering.md#radioactive-waste-package). Verify density and phase composition, use [microscopy](../../optics.md#microscopy) to find segregated constituents or pores, and test [leaching](../../engineering.md#leaching) of the actual product. Successful densification alone does not establish radionuclide retention.[Institutional technology overview, waste-form design, characterisation and hot isostatic pressing](../../engineering.md#ansto-synroc-radioactive-waste-treatment-technology-by-the-australian-nuclear-science-and-technology-organisation)

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The host is **[zirconolite](../../planetary-science.md#zirconolite)**, with ideal end-member composition $\mathrm{CaZrTi_2O_7}$. In the proposed formula, the substitution is formally

$$
\mathrm{Zr^{4+}\longleftrightarrow Pu^{4+}}.
$$

It is an [isovalent substitution](../../chemical-substance.md#isovalent-substitution): the mean charge of the mixed [zirconium](../../chemical-substance.md#zirconium)/[plutonium](../../chemical-substance.md#plutonium) site remains $+4$, so

$$
2+\big[0.2(4)+0.8(4)\big]+2(4)=14=7(2).
$$

No compensating oxygen vacancy or aliovalent co-substituent is required by this particular charge account. Suitable [oxidation state](../../chemical-reaction.md#oxidation-state) is essential; the same formula interpreted with only trivalent [plutonium](../../chemical-substance.md#plutonium) would not be charge balanced.

In [zirconolite-2M](../../planetary-science.md#zirconolite-2m) the [zirconium](../../chemical-substance.md#zirconium) site has an oxygen [coordination number](../../ionic-bonding.md#coordination-number) of seven. The [ionic radius](../../chemistry.md#ionic-radius) of [plutonium](../../chemical-substance.md#plutonium)(IV) is larger than that of [zirconium](../../chemical-substance.md#zirconium)(IV), so increasing its occupancy changes local strain and the preferred arrangement of the [cation](../../chemistry.md#cation) layers. The observed progression in the investigated substitution series was **[zirconolite-2M](../../planetary-science.md#zirconolite-2m) → [zirconolite-4M](../../planetary-science.md#zirconolite-4m) → [pyrochlore structure](../../physical-chemistry.md#pyrochlore-structure)**, rather than unlimited substitution in one unchanged monoclinic lattice. The primary study found a 2M [solid-solution limit](../../chemical-substance.md#solid-solution-limit) near $x=0.15$, a narrow 4M range near $x=0.41$, and a pyrochlore composition at $x=0.60$ in $\mathrm{CaZr}_{1-x}\mathrm{Pu}_x\mathrm{Ti_2O_7}$. These are experimental observations for that series, not universal boundaries independent of preparation and [oxidation state](../../chemical-reaction.md#oxidation-state).[MRS Proceedings 663, 259; abstract, seven-coordinate site and reported polytype transitions](../../engineering.md#structural-effect-of-pu-substitutions-on-the-zr-site-in-zirconolite-by-b-d-begg-and-others)

Consequently the nominal $x=0.20$ composition identifies a zirconolite-based waste-form design, but **does not by itself prove a pure 2M product**. Diffraction and phase-composition measurements are needed. At larger substitution, the fluorite-related pyrochlore arrangement accommodates a different [cation](../../chemistry.md#cation) distribution and coordination environment.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

**[gadolinium](../../chemical-substance.md#gadolinium) is primarily a strong [neutron](../../neutron.md) absorber.** The supplied thermal cross section for [gadolinium-157](../../chemical-substance.md#gadolinium-157) is very large, so capture removes [neutrons](../../neutron.md) that could otherwise sustain [nuclear fission](../../physics.md#nuclear-fission). This is a criticality-control role rather than a requirement to complete the host formula. The isotope-specific number must not be assigned unchanged to natural [gadolinium](../../chemical-substance.md#gadolinium).

**[hafnium](../../chemical-substance.md#hafnium) supplies an additional [neutron poison](../../physics.md#neutron-poison) with favourable retention chemistry.** Its supplied natural-abundance thermal cross section is much smaller than that of [gadolinium-157](../../chemical-substance.md#gadolinium-157) but still appreciable. Chemically, tetravalent [hafnium](../../chemical-substance.md#hafnium) resembles [zirconium](../../chemical-substance.md#zirconium) and can remain associated with a durable titanate host. Keeping the absorber with the fissile inventory during alteration is as important as its initial [neutron capture](../../physics.md#neutron-capture) strength: a highly absorbing constituent offers poor long-term protection if it is preferentially lost. These considerations explain using complementary absorbers rather than ranking them solely by their initial thermal cross sections.

**[uranium](../../chemical-substance.md#uranium) addition chiefly addresses isotopic dilution, including the long-term daughter inventory.** [plutonium-239](../../chemical-substance.md#plutonium-239) [alpha decay](../../physics.md#alpha-decay) produces [uranium-235](../../chemical-substance.md#uranium-235). Added [uranium-238](../../chemical-substance.md#uranium-238) lowers the [uranium-235](../../chemical-substance.md#uranium-235) fraction of that future [uranium](../../chemical-substance.md#uranium) inventory; [depleted uranium](../../chemical-substance.md#depleted-uranium) adds less [uranium-235](../../chemical-substance.md#uranium-235) initially than natural [uranium](../../chemical-substance.md#uranium). [uranium-238](../../chemical-substance.md#uranium-238) also absorbs some [neutrons](../../neutron.md), but its small listed cross section does not make it a substitute for the strong absorbers. The long-term daughter issue and the retention of [gadolinium](../../chemical-substance.md#gadolinium) and [hafnium](../../chemical-substance.md#hafnium) are explicit concerns in [ceramic](../../engineering.md#ceramic) waste-form development.[Section 2, plutonium-immobilisation ceramic development, uranium-235 ingrowth and neutron-absorber retention](../../engineering.md#immobilisation-of-higher-activity-wastes-from-nuclear-reactor-production-of-99mo-by-m-w-a-stewart-and-others)

These are complementary physical purposes, **not proof of [criticality control in radioactive waste](../../engineering.md#criticality-control-in-radioactive-waste) from three cross-section values**. [neutron](../../neutron.md) energy, isotopic composition, geometry, moderation, absorber distribution and their coupled evolution matter. Incorporation in the same durable waste form helps maintain association, but neither [uranium](../../chemical-substance.md#uranium) addition nor chemical immobilisation makes deliberate element separation physically impossible.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $c(t)$ be the fraction still crystalline. Under the [direct-impact amorphization model](../../engineering.md#direct-impact-amorphization-model), damage events occur randomly and independently; an event striking already amorphous material does not create that much additional amorphous volume. Only the crystalline fraction can be newly converted, so

$$
\frac{dc}{dt}=-Rvc,\qquad c(0)=1,\qquad f_a(t)=1-c(t)=1-e^{-Rvt}.
$$

The product of the given event rate density and damage volume has units of inverse time:

$$
k=Rv=(5.685\times10^{14})(1.706\times10^{-25})
=9.69861\times10^{-11} \mathrm{s^{-1}}.
$$

For $99\%$ [radiation-induced amorphization](../../engineering.md#radiation-induced-amorphization), $c=0.01$, giving

$$
t_{99}=\frac{-\ln(0.01)}{k}=4.74828\times10^{10} \mathrm s
=\boxed{1504.64 \mathrm{yr}}.
$$

Using $365.25$ days per year, the corresponding calendar date is **approximately 3555 CE**, measured from disposal preparation in 2050.

<a id="3/d/image-random-overlap-prediction-for-radiation-induced-amorphization-of-the-waste-form"></a>
![](../../past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge/2021/paper-ne4-amorphization.png)

**[Figure 2](#3/d/image-random-overlap-prediction-for-radiation-induced-amorphization-of-the-waste-form). Random-overlap prediction for radiation-induced amorphization of the waste form**.

A linear estimate $f_a=Rvt$ misses repeated hits to already damaged regions and therefore predicts too rapid an approach to $99\%$. The [exponential function](../../calculus.md#exponential-function) model never reaches exactly $100\%$ in finite time. Its assumptions include constant dose rate, fixed effective damage volume, no [annealing](../../engineering.md#annealing-materials-science) and no spatial correlation of damage. Actual [alpha decay](../../physics.md#alpha-decay) generates recoil damage as well as the [alpha particle](../../atomic-nucleus.md#alpha-particle)'s track; the stated damage volume must be understood as the effective volume per [radioactive decay](../../physics.md#radioactive-decay) for the chosen model.

**Amorphous is not synonymous with dissolved or failed containment.** Radiation damage can change swelling, connected [porosity](../../porous-media-flow.md#porosity) and leach behaviour, so testing must compare structural evolution with element release. Accelerated self-irradiation and parallel dissolution measurements are useful precisely because crystallinity alone is not the performance endpoint.[1994 primary conference abstract, accelerated self-irradiation and parallel aqueous-dissolution investigations](../../engineering.md#jaeri-ansto-co-operative-research-on-radiation-damage-and-actinide-behaviour-in-synroc-by-s-muraoka-and-others)

## 4

↑ **Parent:** [Module NE4](paper-ne4.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A useful three-product account is **a demonstrated site end state, recovered materials, and wastes requiring disposal or continuing management**. It keeps the land outcome distinct from the material streams.

The first product is the land and any retained buildings in the specified [nuclear decommissioning](../../engineering.md#nuclear-decommissioning) end state. Characterisation and final surveys must show that the remaining inventory is consistent with the intended reuse and any retained restrictions. Demolition is a possible means of reaching that state, not its definition. The associated records and final radiological evidence are part of the handover.

The second product is reusable or recyclable material and equipment. Segregation and, where appropriate, [decontamination](../../engineering.md#decontamination) prevent clean bulk material from being unnecessarily mixed with contaminated material. Release from radiological control requires demonstrated [radiological clearance](../../engineering.md#radiological-clearance); conventional chemical hazards still need their own management.

The third product is waste: both ordinary unrecoverable demolition debris and [radioactive waste](../../engineering.md#radioactive-waste) that remains under control. Activated structures, contaminated components and secondary cleaning wastes may require different treatment and packages. [spent nuclear fuel](../../engineering.md#spent-nuclear-fuel), if still present, requires its own inventory and management route rather than being counted as ordinary scrap. Thus **the material outputs can alternatively be tabulated as reusable material, conventional waste and [radioactive waste](../../engineering.md#radioactive-waste)**, while the restored site is the overarching project deliverable. The source does not define a unique named three-product taxonomy.[WS-R-5, paragraph 1.4 on implementation, waste management and demonstrated end-state criteria](../../engineering.md#decommissioning-of-facilities-using-radioactive-material-by-the-international-atomic-energy-agency)

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The traditional threefold classification is **[immediate dismantling](../../engineering.md#immediate-dismantling), [deferred dismantling](../../engineering.md#deferred-dismantling) and [entombment of a nuclear facility](../../engineering.md#entombment-of-a-nuclear-facility)**. It appears in the older IAEA WS-R-5 classification.[2006, paragraph 1.5, historical descriptions of the three approaches](../../engineering.md#decommissioning-of-facilities-using-radioactive-material-by-the-international-atomic-energy-agency)

With [immediate dismantling](../../engineering.md#immediate-dismantling), [decontamination](../../engineering.md#decontamination) and removal follow permanent shutdown without a prolonged safe-storage interval. Operating staff, drawings and knowledge remain available, the project can reach its end state sooner, and the site can return to use earlier. Against this, substantial funds and waste-management routes are needed early, and less time has elapsed for short-lived activation products to [radioactive decay](../../physics.md#radioactive-decay). Exposure and remote-handling requirements may therefore be greater for a particular task.

With [deferred dismantling](../../engineering.md#deferred-dismantling), the facility is put into a maintained safe condition before later dismantling. [radioactive decay](../../physics.md#radioactive-decay) can reduce some later radiation fields and permit better tools or disposal routes to become available. However, deferral does not remove the waste or responsibility: surveillance, security, building maintenance and preservation of records continue. Deterioration or loss of institutional knowledge can offset the benefit. Long-lived constituents may obtain little useful reduction over a practicable delay.

[entombment of a nuclear facility](../../engineering.md#entombment-of-a-nuclear-facility) encases radioactive structures within a long-lived barrier. It can reduce the need for immediate intrusive work in exceptional circumstances, but leaves a persistent in-situ inventory, restricts site use and requires confidence in barriers, groundwater behaviour and long-term institutional arrangements. It transfers management obligations rather than simply completing ordinary unrestricted site release.

There is an important qualification to the historical wording: **GSR Part 6, published in 2014 and therefore already applicable to interpreting a 2021 question, recognises the first two planned strategies and excludes [entombment of a nuclear facility](../../engineering.md#entombment-of-a-nuclear-facility) for planned permanent shutdown.** Paragraph 1.10 allows it to be considered only exceptionally, such as after a severe accident. It would therefore be misleading to present all three historical labels as equally acceptable normal planned strategies.[GSR Part 6, paragraphs 1.9–1.10, particularly the explicit entombment qualification](../../engineering.md#decommissioning-of-facilities-by-the-international-atomic-energy-agency)

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $c_e$ be the measured mass [concentration](../../mathematical-physics.md#concentration) of element $e$, $c_{e,b}$ its blank [concentration](../../mathematical-physics.md#concentration), $V$ the leachate volume, $f_e$ the element's [mass fraction](../../mixture.md#mass-fraction) in the original [glass](../../chemical-substance.md#glass), and $S$ the exposed [glass](../../chemical-substance.md#glass) [surface area](../../differential-geometry.md#surface-area). For one closed test, the [normalised elemental release](../../engineering.md#normalised-elemental-release) is

$$
\boxed{NL_e=\frac{(c_e-c_{e,b})V}{f_eS}}.
$$

If [concentration](../../mathematical-physics.md#concentration) is in $\mathrm{g\,L^{-1}}$, volume in litres and area in square metres, $NL_e$ is in **$\mathrm{g\,m^{-2}}$ of glass-equivalent release**. Dividing by $f_e$ removes the trivial difference caused by loading different amounts of the measured element; dividing by $S$ removes the first-order geometrical scale difference. Normalising only by initial element content or reporting raw solution [concentration](../../mathematical-physics.md#concentration) does not accomplish both corrections.

For repeated sampling with leachant replacement, use cumulative released mass: add the mass removed in all earlier aliquots to the mass present in the final remaining solution, with the corresponding blank correction. A flow-through experiment instead integrates $Q(t)[c_{e,\rm out}(t)-c_{e,\rm in}(t)]$ over time. State how [surface area](../../differential-geometry.md#surface-area) was determined and whether it is held at its initial value in the reported normalisation; cracks, fines and alteration can change the genuinely reactive area.

Compare $NL_e(t)$ for several constituents. In [congruent glass dissolution](../../engineering.md#congruent-glass-dissolution), the different element-normalised curves coincide, provided the released elements remain in solution. Preferential early alkali release can indicate [ion exchange](../../engineering.md#ion-exchange), whereas lower dissolved [silicon](../../chemical-substance.md#silicon) or [actinide](../../chemical-substance.md#actinide) release can reflect an alteration layer, sorption or secondary-phase [precipitation](../../chemical-reaction.md#precipitation-chemistry). [boron](../../chemical-substance.md#boron) is often useful as a relatively mobile dissolution tracer, but not if the leachant contains a large [boron](../../chemical-substance.md#boron) background or if it is itself retained. A low aqueous [concentration](../../mathematical-physics.md#concentration) of one constituent is therefore **not automatically a low glass-dissolution rate**.

A near-linear $NL_e(t)$ interval gives an approximately constant [normalised elemental release](../../engineering.md#normalised-elemental-release) rate. A square-root time dependence can be consistent with diffusion-limited transport, and decreasing slopes can indicate saturation or a protective alteration layer; no one curve shape proves a unique mechanism. Compare solution inventories with the altered solid by [microscopy](../../optics.md#microscopy), composition and phase analysis. Differences in [pH](../../acid-base-chemistry.md#ph), [temperature](../../temperature.md), leachant composition, duration and surface-area-to-volume ratio remain even after this mass-and-area normalisation. Careful background subtraction and control of solution conditions are experimentally consequential, as demonstrated in primary flow-through measurements.[Journal of Nuclear Materials 249, 175–189; abstract on duration, background subtraction and solution-condition dependence](../../engineering.md#measurement-of-kinetic-rate-law-parameters-on-a-na-ca-al-borosilicate-glass-for-low-activity-waste-by-b-p-mcgrail-and-others)

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Use a **[single-pass flow-through leach test](../../engineering.md#single-pass-flow-through-leach-test)**. A controlled leachant passes once over a known [glass](../../chemical-substance.md#glass) [surface area](../../differential-geometry.md#surface-area), and successive effluent samples are analysed after the initial transient. [temperature](../../temperature.md) and [pH](../../acid-base-chemistry.md#ph) are controlled, and fresh solution removes dissolved products so that they do not accumulate towards saturation with respect to the dissolving [glass](../../chemical-substance.md#glass). This approaches the [forward glass dissolution rate](../../engineering.md#forward-glass-dissolution-rate) at those specified conditions.

At steady state, with $Q$ expressed as volume per time,

$$
\boxed{r_e=\frac{Q(c_{e,\rm out}-c_{e,\rm in})}{f_eS}}.
$$

Increase $Q/S$ across a series of tests until the normalised rate becomes independent of further dilution, within analytical uncertainty. A genuine plateau supports approach to the dilute-solution limit; it should not be assumed from one arbitrarily chosen flow rate. Check blanks, inlet [concentrations](../../mathematical-physics.md#concentration), [temperature](../../temperature.md), [pH](../../acid-base-chemistry.md#ph), actual flow, fines and exposed [surface area](../../differential-geometry.md#surface-area). At high flow the [concentration](../../mathematical-physics.md#concentration) increment becomes small, so an uncorrected background can manufacture an apparent rate increase.

The resulting **maximum is the forward rate for the specified [temperature](../../temperature.md), [pH](../../acid-base-chemistry.md#ph) and [glass](../../chemical-substance.md#glass)**, not an absolute maximum over every possible environment. It also differs from the lower residual rate that can develop in a static, product-rich leachate. Primary measurements demonstrate the method and the importance of background subtraction and flow variation.[1997, experimental method and abstract, including the nonphysical flow-rate increase caused by inadequate background subtraction](../../engineering.md#measurement-of-kinetic-rate-law-parameters-on-a-na-ca-al-borosilicate-glass-for-low-activity-waste-by-b-p-mcgrail-and-others)

## ↑ Ancestors (7)

1. [2021](../2021.md)
2. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
3. [MPhil in nuclear energy course of the University of Cambridge](../../university-of-cambridge.md#mphil-in-nuclear-energy-course-of-the-university-of-cambridge)
4. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
5. [University of Cambridge](../../university-of-cambridge.md)
6. [List of universities](../../README.md#list-of-universities)
7. [Codex Wiki](../../README.md)
