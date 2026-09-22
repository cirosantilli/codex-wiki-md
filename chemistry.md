# Chemistry

↑ **Parent:** [Codex Wiki](README.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemistry)

**Table of contents**

- [Polymer](#polymer)
  - [Flory approximation](#flory-approximation)
  - [Polymerization](#polymerization)
  - [Monomer](#monomer)
  - [Deoxyribonucleic acid](#deoxyribonucleic-acid)
  - [Radius of gyration](#radius-of-gyration)
- [Ion](#ion)
  - [Counterion](#counterion)
- [Electrochemistry](#electrochemistry)
  - [Electrolyte](#electrolyte)
- [Chemical reaction](#chemical-reaction)
  - [Substrate (chemistry)](#substrate-chemistry)
  - [Thermal dissociation](#thermal-dissociation)
  - [Stoichiometry](#stoichiometry)
- [Chemical substance](#chemical-substance)
  - [Hydrogen deuteride](#hydrogen-deuteride)
  - [Chemical element](#chemical-element)
    - [Sodium](#sodium)
    - [Atomic number](#atomic-number)
    - [Beryllium](#beryllium)
      - [Beryllium-7](#beryllium-7)
    - [Lithium](#lithium)
      - [Lithium-7](#lithium-7)
    - [Isotope](#isotope)
    - [Uranium](#uranium)
    - [Lead](#lead)
    - [Barium](#barium)
    - [Silicon](#silicon)
    - [Magnesium](#magnesium)
    - [Neon](#neon)
    - [Cobalt](#cobalt)
    - [Nickel](#nickel)
      - [Nickel-56 decay chain](#nickel-56-decay-chain)
    - [Iron](#iron)
    - [Oxygen](#oxygen)
      - [Oxygen-16](#oxygen-16)
      - [Molecular oxygen](#molecular-oxygen)
    - [Nitrogen](#nitrogen)
    - [Carbon](#carbon)
      - [Carbon-12](#carbon-12)
    - [Helium](#helium)
      - [Helium-3](#helium-3)
      - [Helium-4](#helium-4)
    - [Hydrogen](#hydrogen)
      - [Metallic hydrogen](#metallic-hydrogen)
      - [Deuterium](#deuterium)
      - [Hydrogen anion](#hydrogen-anion)
  - [Molecular nitrogen](#molecular-nitrogen)
  - [Molecular hydrogen](#molecular-hydrogen)
  - [Chemical compound](#chemical-compound)
    - [Chloromethane](#chloromethane)
    - [Dimethyl sulfide](#dimethyl-sulfide)
    - [Ozone](#ozone)
    - [Nitrous oxide](#nitrous-oxide)
    - [Phosphine](#phosphine)
    - [Vanadium(II) oxide](#vanadium-ii-oxide)
    - [Titanium monoxide](#titanium-monoxide)
    - [Acetylene](#acetylene)
    - [Hydrogen cyanide](#hydrogen-cyanide)
    - [Carbon dioxide](#carbon-dioxide)
    - [Carbon monoxide](#carbon-monoxide)
    - [Ammonia](#ammonia)
    - [Methane](#methane)
      - [Methanogenesis](#methanogenesis)
    - [Water](#water)
      - [Ice](#ice)
        - [Snowflake](#snowflake)
          - [Dendritic growth of a snowflake](#dendritic-growth-of-a-snowflake)
- [Steady state (chemistry)](#steady-state-chemistry)

## Polymer

↑ **Parent:** [Chemistry](chemistry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polymer)

A [polymer](#polymer) is a large molecular chain or network built from many chemically linked repeating units. Statistical chain models idealize its microscopic structure by segment vectors and describe its conformation through distributions, correlations and scattering. A [freely jointed chain](mathematical-biology.md#ideal-chain) fixes each segment length while allowing independent orientations; a [Gaussian chain](mathematical-biology.md#gaussian-chain) replaces the segment or coarse-grained displacement distribution by a [Gaussian distribution](probability-theory.md#normal-distribution). These ideal models neglect excluded-volume and other segment interactions.

### Flory approximation

↑ **Parent:** [Polymer](#polymer)

The [Flory approximation](#flory-approximation) balances the entropic cost of expanding an [ideal chain](mathematical-biology.md#ideal-chain) against a mean-field [excluded volume](statistical-physics.md#excluded-volume) interaction. For $N$ segments of length $b$ in $d$ spatial dimensions, minimizing $R^2/(Nb^2)+vN^2/R^d$ gives $R^{d+2}\sim vN^3b^2$. This yields the scaling exponents $3/5$ in three dimensions and $3/4$ in two dimensions. It is a scaling approximation, not an exact numerical free energy or proof of critical exponents; confinement replaces $R^d$ by the accessible coil volume.

### Polymerization

↑ **Parent:** [Polymer](#polymer)

[Polymerization](#polymerization) joins molecular units into a [polymer](#polymer). For a filament end exchanging units with a solution, addition and removal rates determine growth, while steric constraints and an applied force can modify those rates.

### Monomer

↑ **Parent:** [Polymer](#polymer)

A [monomer](#monomer) is a molecular unit that can join other units through [polymerization](#polymerization). A statistical link in a coarse-grained chain model need not coincide with one chemical monomer.

### Deoxyribonucleic acid

↑ **Parent:** [Polymer](#polymer)

A [deoxyribonucleic acid](#deoxyribonucleic-acid) molecule is a nucleotide [polymer](#polymer) that stores genetic information. Its double-stranded form is often modeled mechanically as a [worm-like chain](mathematical-biology.md#worm-like-chain), with elasticity and effective excluded volume depending on solvent conditions.

### Radius of gyration

↑ **Parent:** [Polymer](#polymer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radius_of_gyration)

For $N$ equally weighted positions, the squared [radius of gyration](#radius-of-gyration) is the average squared distance from the [center of mass](classical-mechanics.md#center-of-mass): $R_g^2=N^{-1}\sum_n\langle|\mathbf R_n-\mathbf R_{\rm cm}|^2\rangle$, where $\mathbf R_{\rm cm}=N^{-1}\sum_n\mathbf R_n$. Expanding pair differences gives $\sum_{m,n}|\mathbf R_m-\mathbf R_n|^2=2N\sum_n|\mathbf R_n-\mathbf R_{\rm cm}|^2$, and therefore

$$
R_g^2=\frac1{2N^2}\sum_{m,n}\langle|\mathbf R_m-\mathbf R_n|^2\rangle.
$$

For a [Gaussian chain](mathematical-biology.md#gaussian-chain) or [freely jointed chain](mathematical-biology.md#ideal-chain) with these $N$ positions and mean squared link length $b^2$, each pair [variance](variance.md) is $b^2|m-n|$. Summing separations yields $R_g^2=b^2(N^2-1)/(6N)\sim Nb^2/6$. Counting all endpoints of $N$ links instead gives $N+1$ positions and the corresponding finite-size formula.

## Ion

↑ **Parent:** [Chemistry](chemistry.md)

A [chemical atom](physics.md#atom-physics) or molecular entity with nonzero net [electric charge](electromagnetism.md#electric-charge). An [ion](#ion) opposing a fixed charge is called a [counterion](#counterion).

### Counterion

↑ **Parent:** [Ion](#ion)

A mobile [ion](#ion) whose charge has the opposite sign to a charged macromolecule, surface or other fixed species. Its local [concentration](physics.md#concentration) can increase close to that fixed charge; [counterion condensation](electromagnetism.md#counterion-condensation) distinguishes a bound fraction that remains localized in an infinite-dilution limit.

## Electrochemistry

↑ **Parent:** [Chemistry](chemistry.md)

Chemical systems whose reactions, transport or equilibrium couple to [electric charges](electromagnetism.md#electric-charge) and [electric potential](electromagnetism.md#electric-potential). An [electrolyte](#electrolyte) carries mobile [ions](#ion); a [Poisson-Boltzmann equation](electromagnetism.md#poisson-boltzmann-equation) can approximate their equilibrium distributions.

### Electrolyte

↑ **Parent:** [Electrochemistry](#electrochemistry)

A medium with mobile [ions](#ion) capable of carrying [electric charge](electromagnetism.md#electric-charge). Dissolved salts typically supply both positive and negative species; a counterion-only model keeps only the mobile species required to oppose a fixed charge. [Poisson-Boltzmann equations](electromagnetism.md#poisson-boltzmann-equation) use ideal [Boltzmann distributions](thermodynamics.md#boltzmann-distribution) for those species.

## Chemical reaction

↑ **Parent:** [Chemistry](chemistry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemical_reaction)

### Substrate (chemistry)

↑ **Parent:** [Chemical reaction](#chemical-reaction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Substrate_(chemistry))

A chemical species on which a reagent or catalyst acts in a [chemical reaction](#chemical-reaction). An [enzyme](biology.md#enzyme) acts on a biochemical [substrate](biology.md#substrate-biochemistry), a particular instance of this broader reaction role.

### Thermal dissociation

↑ **Parent:** [Chemical reaction](#chemical-reaction)

Thermal dissociation is temperature-driven breaking of a molecule into simpler fragments. The [chemical equilibrium](thermodynamics.md#chemical-equilibrium) abundance depends on pressure as well as temperature: reactions increasing particle number are generally favored at low pressure. In an [exoplanet atmosphere](exoplanet.md#exoplanet-atmosphere), reduced [water](#water) on a very hot dayside does not by itself establish a low planetary oxygen abundance.

### Stoichiometry

↑ **Parent:** [Chemical reaction](#chemical-reaction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stoichiometry)

[Stoichiometry](#stoichiometry) records reactant and product multiplicities in a [chemical reaction](#chemical-reaction) or a [chemical reaction network](mathematical-biology.md#chemical-reaction-network). The change caused by one reaction is its [stoichiometric vector](mathematical-biology.md#stoichiometric-vector); multiplying by the reaction rate gives its contribution to the concentration equations. For two identical reactants the rate-constant convention absorbs any combinatorial factor.

## Chemical substance

↑ **Parent:** [Chemistry](chemistry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemical_substance)

### Hydrogen deuteride

↑ **Parent:** [Chemical substance](#chemical-substance)

The diatomic molecule containing one ordinary hydrogen nucleus and one deuterium nucleus is an isotopic form of [molecular hydrogen](#molecular-hydrogen). It has a weak electric dipole and can supply low-temperature [molecular line cooling](thermodynamics.md#molecular-line-cooling) in primordial gas when its abundance is sufficient.

### Chemical element

↑ **Parent:** [Chemical substance](#chemical-substance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemical_element)

#### Sodium

↑ **Parent:** [Chemical element](#chemical-element)

Sodium is the [chemical element](#chemical-element) of [atomic number](#atomic-number) eleven. Carbon-fusion channels in [carbon burning](stellar-astrophysics.md#carbon-burning) include ${}^{12}\mathrm C+{}^{12}\mathrm C\longrightarrow{}^{23}\mathrm{Na}+p$, producing sodium-23 and a [proton](physics.md#proton). Its abundance in expelled stellar material depends on later reactions and mixing, rather than on this one production channel alone.

#### Atomic number

↑ **Parent:** [Chemical element](#chemical-element)

#### Beryllium

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Beryllium)

Beryllium is the [chemical element](#chemical-element) with atomic number four. Its isotope [beryllium-7](#beryllium-7) provides an important route to primordial [lithium-7](#lithium-7).

##### Beryllium-7

↑ **Parent:** [Beryllium](#beryllium)

Beryllium-7 contains four [protons](physics.md#proton) and three [neutrons](physics.md#neutron). It forms in reactions including $^3\mathrm{He}+{}^4\mathrm{He}\to{}^7\mathrm{Be}+\gamma$ and becomes [lithium-7](#lithium-7) through [electron capture](physics.md#electron-capture). In the early universe its ionization state affects when capture occurs, so the final primordial lithium inventory includes the earlier beryllium inventory rather than just lithium present when nuclear burning ends.

#### Lithium

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lithium)

Lithium is the [chemical element](#chemical-element) with atomic number three. Its stable isotopes include lithium-6 and [lithium-7](#lithium-7). Lithium observed in old stellar atmospheres is an important but processing-sensitive test of [Big Bang nucleosynthesis](cosmology.md#big-bang-nucleosynthesis).

##### Lithium-7

↑ **Parent:** [Lithium](#lithium)

Lithium-7 has three [protons](physics.md#proton) and four [neutrons](physics.md#neutron). In [Big Bang nucleosynthesis](cosmology.md#big-bang-nucleosynthesis) it can form directly or through [beryllium-7](#beryllium-7), which later undergoes [electron capture](physics.md#electron-capture). Competition between direct lithium production, lithium destruction and beryllium production produces a valley in the primordial lithium abundance versus [baryon-to-photon ratio](cosmology.md#baryon-to-photon-ratio). Its measured stellar surface abundance need not equal its birth abundance because stellar transport and nuclear burning can remove lithium.

#### Isotope

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isotope)

Isotopes are atoms of the same [chemical element](#chemical-element), with the same number of [protons](physics.md#proton) but different numbers of [neutrons](physics.md#neutron). Their abundance ratios can distinguish material sources and biological or chemical fractionation, while radioactive isotopes can additionally carry chronological information.

#### Uranium

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uranium)

The [chemical element](#chemical-element) with atomic number 92. Its long-lived radioactive isotopes illustrate actinide production by the [rapid neutron-capture process](physics.md#r-process).

#### Lead

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lead)

The [chemical element](#chemical-element) with atomic number 82. Lead isotopes are important heavy products of the [slow neutron-capture process](stellar-astrophysics.md#s-process) in suitable neutron-exposure conditions.

#### Barium

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Barium)

The [chemical element](#chemical-element) with atomic number 56. Enrichment in barium can reveal transferred [slow neutron-capture process](stellar-astrophysics.md#s-process) products, as in a [barium star](stellar-astrophysics.md#barium-star).

#### Silicon

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Silicon)

The [chemical element](#chemical-element) with atomic number 14. [Oxygen burning](stellar-astrophysics.md#oxygen-burning) produces silicon-group nuclei; subsequent [silicon burning](stellar-astrophysics.md#silicon-burning) is a reaction network approaching an iron-group mixture.

#### Magnesium

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnesium)

The [chemical element](#chemical-element) with atomic number 12. Magnesium isotopes occur among products of [carbon burning](stellar-astrophysics.md#carbon-burning) and alpha-capture neutron-source reactions.

#### Neon

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Neon)

The [chemical element](#chemical-element) with atomic number 10. [Neon burning](stellar-astrophysics.md#neon-burning) uses photodisintegration and alpha capture, while neon-22 can provide neutrons through $^{22}\mathrm{Ne}(\alpha,n){}^{25}\mathrm{Mg}$.

#### Cobalt

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cobalt)

The [chemical element](#chemical-element) with atomic number 27. Cobalt-56 is the intermediate radioactive nucleus in the [nickel-56 decay chain](#nickel-56-decay-chain).

#### Nickel

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nickel)

The [chemical element](#chemical-element) with atomic number 28. Radioactive nickel-56 is produced in explosive burning; the [nickel-56 decay chain](#nickel-56-decay-chain) contributes energy to supernova emission.

##### Nickel-56 decay chain

↑ **Parent:** [Nickel](#nickel)

The radioactive chain converts nickel-56 through cobalt-56 into iron-56, releasing energy that can power supernova light curves. [Electron capture](physics.md#electron-capture) and, where allowed, [beta-plus decay](physics.md#beta-plus-decay) convert protons into neutrons; gamma rays and charged decay products deposit some of the released energy. Ionization and escape of decay radiation affect the observed heating.

#### Iron

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Iron)

The [chemical element](#chemical-element) with atomic number 26. Iron-group [nuclear binding energy](physics.md#nuclear-binding-energy) and [silicon burning](stellar-astrophysics.md#silicon-burning) are central to the termination of ordinary energy-producing stellar fusion.

#### Oxygen

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Oxygen)

##### Oxygen-16

↑ **Parent:** [Oxygen](#oxygen)

##### Molecular oxygen

↑ **Parent:** [Oxygen](#oxygen)

The diatomic form of [oxygen](#oxygen). Modern terrestrial abundance is maintained largely by oxygenic [photosynthesis](biology.md#photosynthesis), balanced by chemical and biological sinks.

#### Nitrogen

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nitrogen)

#### Carbon

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Carbon)

##### Carbon-12

↑ **Parent:** [Carbon](#carbon)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Carbon-12)

#### Helium

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Helium)

##### Helium-3

↑ **Parent:** [Helium](#helium)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Helium-3)

This stable [helium](#helium) isotope contains two [protons](physics.md#proton) and one [neutron](physics.md#neutron). In solar proton-proton burning it is an intermediate: two such nuclei can form [helium-4](#helium-4) and return two [protons](physics.md#proton), or one can capture [helium-4](#helium-4) to enter the second chain branch. The balance between production and destruction determines the [helium-3 equilibrium abundance](stellar-astrophysics.md#helium-3-equilibrium-abundance) and its [helium-3 relaxation time](stellar-astrophysics.md#helium-3-relaxation-time).

##### Helium-4

↑ **Parent:** [Helium](#helium)

Helium-4 is the stable helium isotope with two protons and two neutrons; its nucleus is an alpha particle. Its strong binding makes it the principal neutron-containing product of primordial [Big Bang nucleosynthesis](cosmology.md#big-bang-nucleosynthesis).

#### Hydrogen

↑ **Parent:** [Chemical element](#chemical-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hydrogen)

##### Metallic hydrogen

↑ **Parent:** [Hydrogen](#hydrogen)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Metallic_hydrogen)

Metallic hydrogen is a high-pressure conducting state of [hydrogen](#hydrogen). Its fluid form in the deep interiors of [gas giants](planetary-science.md#gas-giant) supplies a conducting medium for a [planetary dynamo](planetary-science.md#planetary-dynamo), unlike the iron-alloy conducting cores of [terrestrial planets](planetary-science.md#terrestrial-planet).

##### Deuterium

↑ **Parent:** [Hydrogen](#hydrogen)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Deuterium)

This stable [hydrogen](#hydrogen) isotope has one [proton](physics.md#proton) and one [neutron](physics.md#neutron). In the [Proton–proton chain](stellar-astrophysics.md#proton-proton-chain) it is produced by the slow weak proton-pair reaction and is rapidly consumed by [proton](physics.md#proton) capture to make [helium-3](#helium-3). Its short nuclear lifetime inside a stellar core allows a [deuterium quasi-equilibrium in proton-proton burning](stellar-astrophysics.md#deuterium-quasi-equilibrium-in-proton-proton-burning) approximation.

##### Hydrogen anion

↑ **Parent:** [Hydrogen](#hydrogen)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hydrogen_anion)

A negative hydrogen ion is a [hydrogen](#hydrogen) nucleus with two bound electrons. Its weakly bound extra electron permits absorption at visible and infrared wavelengths in cool stellar atmospheres.

### Molecular nitrogen

↑ **Parent:** [Chemical substance](#chemical-substance)

### Molecular hydrogen

↑ **Parent:** [Chemical substance](#chemical-substance)

### Chemical compound

↑ **Parent:** [Chemical substance](#chemical-substance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemical_compound)

#### Chloromethane

↑ **Parent:** [Chemical compound](#chemical-compound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chloromethane)

An organochlorine gas with biological as well as possible nonbiological sources. Its specialized biological production is a [secondary metabolic byproduct](biology.md#secondary-metabolic-byproduct) example.

#### Dimethyl sulfide

↑ **Parent:** [Chemical compound](#chemical-compound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dimethyl_sulfide)

An organic sulfur gas emitted through biological processing, including marine production associated with sulfur-containing metabolites. It is a [secondary metabolic byproduct](biology.md#secondary-metabolic-byproduct) example and a possible [atmospheric biosignature gas](exoplanet.md#atmospheric-biosignature-gas) whose detectability depends on production and photochemical destruction.

#### Ozone

↑ **Parent:** [Chemical compound](#chemical-compound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ozone)

A triatomic form of [oxygen](#oxygen), produced photochemically from [molecular oxygen](#molecular-oxygen). The [ozone layer](exoplanet.md#ozone-layer) absorbs ultraviolet radiation; ozone can trace atmospheric oxygen without being directly emitted by metabolism.

#### Nitrous oxide

↑ **Parent:** [Chemical compound](#chemical-compound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nitrous_oxide)

A nitrogen oxide produced substantially by microbial nitrogen cycling on modern [Earth](planetary-science.md#earth). Its atmospheric abundance and lifetime make it a candidate [atmospheric biosignature gas](exoplanet.md#atmospheric-biosignature-gas), with context-dependent abiotic alternatives.

#### Phosphine

↑ **Parent:** [Chemical compound](#chemical-compound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Phosphine)

Phosphine is $\mathrm{PH}_3$. Its abundance in giant-planet observable atmospheres can depend on transport from deeper layers faster than local chemical destruction.

<h4 id="vanadium-ii-oxide">Vanadium(II) oxide</h4>

↑ **Parent:** [Chemical compound](#chemical-compound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vanadium(II)_oxide)

#### Titanium monoxide

↑ **Parent:** [Chemical compound](#chemical-compound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Titanium_monoxide)

#### Acetylene

↑ **Parent:** [Chemical compound](#chemical-compound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Acetylene)

#### Hydrogen cyanide

↑ **Parent:** [Chemical compound](#chemical-compound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hydrogen_cyanide)

#### Carbon dioxide

↑ **Parent:** [Chemical compound](#chemical-compound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Carbon_dioxide)

#### Carbon monoxide

↑ **Parent:** [Chemical compound](#chemical-compound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Carbon_monoxide)

#### Ammonia

↑ **Parent:** [Chemical compound](#chemical-compound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ammonia)

#### Methane

↑ **Parent:** [Chemical compound](#chemical-compound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Methane)

##### Methanogenesis

↑ **Parent:** [Methane](#methane)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Methanogenesis)

Methanogenesis is biological production of [methane](#methane) by anaerobic microorganisms. Waterlogged soil and lake sediments can favour it. Warming or thaw changes substrate availability, but production is distinct from atmospheric emission because oxidation and transport intervene.

#### Water

↑ **Parent:** [Chemical compound](#chemical-compound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Water)

##### Ice

↑ **Parent:** [Water](#water)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ice)

###### Snowflake

↑ **Parent:** [Ice](#ice)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Snowflake)

A snowflake is an [ice](#ice) crystal or an aggregate of [ice](#ice) crystals grown in atmospheric conditions. Its morphology depends on vapour supersaturation, transport, [temperature](thermodynamics.md#temperature) and crystal anisotropy. Not every snowflake is dendritic.

###### Dendritic growth of a snowflake

↑ **Parent:** [Snowflake](#snowflake)

An exposed tip receives vapour more efficiently than a sheltered surface and can amplify its lead, producing [crystal dendrites](geophysics.md#dendrite-crystal) and side branches. The planar thermal [solidification](critical-phenomenon.md#freezing) mechanism is an analogy, not a complete vapour-growth model. The [hexagonal ice crystal anisotropy](geophysics.md#hexagonal-ice-crystal-anisotropy) selects six preferred directions; an isotropic linear instability alone does not select six arms.

## Steady state (chemistry)

↑ **Parent:** [Chemistry](chemistry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Steady_state_(chemistry))

A [steady state](#steady-state-chemistry) has time-independent concentrations because formation and removal rates balance for the species considered. Nonzero reaction fluxes can continue, so a steady state need not be [chemical equilibrium](thermodynamics.md#chemical-equilibrium). A [quasi-steady-state approximation](mathematical-biology.md#quasi-steady-state-approximation) imposes this balance approximately for a fast intermediate while slower species evolve.

## ↑ Ancestors (1)

1. [Codex Wiki](README.md)
