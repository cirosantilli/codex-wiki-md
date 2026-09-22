# Module NE4

↑ **Parent:** [2019](../2019.md)

Original worked solutions cover all four printed alternatives. The University of Cambridge release occupies physical PDF pages 17–20; the questions are on pages 18–20. [Original public PDF, physical pages 17–20](https://www.whatdotheyknow.com/request/past_exam_papers_16/response/2088673/attach/3/FOI%202022%20471%20Smith%20materials.pdf?cookie_passthrough=1#page=17)

The glass-release plot is an illustrative model, and the materials arguments state when reversibility, [crystallographic texture](../../physical-chemistry.md#crystallographic-texture), [temperature](../../temperature.md) or exposure history changes the conclusion.

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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

## 1

↑ **Parent:** [Module NE4](paper-ne4.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

**[thermal cycling growth](../../engineering.md#thermal-cycling-growth) is permanent dimensional change remaining after a [temperature](../../temperature.md) cycle; [irradiation growth](../../engineering.md#irradiation-growth) is a radiation-driven change of shape that need not require an applied load.** Neither is simply the reversible increase in dimensions of a warm specimen.

For a crystal in its principal axes, a small unconstrained thermal [strain](../../continuum-mechanics.md#strain) is

$$
\boldsymbol\varepsilon^{\rm th}=\boldsymbol\alpha\Delta T.
$$

[anisotropic thermal expansion](../../thermodynamics.md#anisotropic-thermal-expansion) means that the principal components of $\boldsymbol\alpha$ differ. Adjacent [crystal grains](../../thermodynamics.md#grain-in-a-polycrystal) with different orientations therefore demand different [strain](../../continuum-mechanics.md#strain) tensors during the same [temperature](../../temperature.md) change. Their bonded boundaries impose compatibility and generate internal [stresses](../../continuum-mechanics.md#stress). [plasticity](../../continuum-mechanics.md#plasticity-physics), [creep](../../engineering.md#creep-deformation), boundary motion or microcracking can accommodate this mismatch irreversibly; when the accommodation fails to cancel on cooling, a residual [strain](../../continuum-mechanics.md#strain) remains. Repeated cycles can accumulate directional [thermal ratcheting](../../engineering.md#thermal-ratcheting), surface roughening or distortion. [crystallographic texture](../../physical-chemistry.md#crystallographic-texture), constraints, cycle amplitude and the [temperature](../../temperature.md) dependence of yielding and recovery determine the outcome.

**Anisotropy alone is insufficient.** A freely expanding [single crystal](../../thermodynamics.md#single-crystal) under spatially uniform, fully reversible heating returns to its original dimensions. Even cyclic [plasticity](../../continuum-mechanics.md#plasticity-physics) can settle into a stabilised response rather than ratchet indefinitely. Demonstrating [thermal cycling growth](../../engineering.md#thermal-cycling-growth) means comparing dimensions at the same reference [temperature](../../temperature.md) after successive cycles, while controlling external loads, [temperature](../../temperature.md) gradients and phase changes. [uranium](../../chemical-substance.md#uranium) dimensional instability under cycling was investigated directly in the early reactor-materials programme.[ORNL-1386, 1952, opening discussion of dimensional instability, preferred orientation and observed distortion](../../engineering.md#thermal-cycling-of-uranium-by-nathaniel-stetson-and-melbourne-l-winton)

[irradiation growth](../../engineering.md#irradiation-growth) has a different source of irreversibility. [displacement cascades](../../engineering.md#displacement-cascade) create [vacancies](../../physical-chemistry.md#vacancy) and [self-interstitials](../../physical-chemistry.md#self-interstitial); anisotropic migration, clustering and capture at oriented [dislocations](../../physical-chemistry.md#dislocation) and boundaries can produce unequal [strains](../../continuum-mechanics.md#strain) along crystal directions. For approximately volume-conserving growth,

$$
\varepsilon_1^{g}+\varepsilon_2^{g}+\varepsilon_3^{g}\simeq0,
$$

although a rod may elongate substantially in one direction. The effect can occur at constant [temperature](../../temperature.md) without an external [stress](../../continuum-mechanics.md#stress). Distinguish it from **[void swelling](../../engineering.md#void-swelling)**, which increases volume through cavities, and **[irradiation creep](../../engineering.md#irradiation-creep)**, whose directional deformation is stress-dependent. Experiments should therefore measure axial and transverse dimensions, [density](../../fluid-mechanics.md#density) and the applied [stress](../../continuum-mechanics.md#stress) rather than identifying every increase in length as one mechanism.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The characteristic growth phenomena require an asymmetric material response and a way to retain irreversible change. **Low crystal symmetry and directional defect or deformation behaviour make [uranium](../../chemical-substance.md#uranium) and [zirconium](../../chemical-substance.md#zirconium) important examples**, whereas an ideal cubic material has isotropic linear [thermal expansion](../../thermodynamics.md#thermal-expansion) and no symmetry-selected traceless single-crystal growth tensor in an otherwise isotropic environment.

[alpha uranium](../../chemical-substance.md#alpha-uranium) is orthorhombic and has strongly anisotropic thermal response. In a textured [polycrystalline material](../../thermodynamics.md#polycrystalline-material), incompatible [crystal grain](../../thermodynamics.md#grain-in-a-polycrystal) [strains](../../continuum-mechanics.md#strain) can be accommodated asymmetrically over a thermal cycle and leave macroscopic distortion. The same metal can also show [irradiation growth](../../engineering.md#irradiation-growth) through anisotropic irradiation-defect evolution. [zirconium](../../chemical-substance.md#zirconium) and its hexagonal close-packed alloys are major examples of [irradiation growth](../../engineering.md#irradiation-growth); their basal and c-axis directions need not acquire the same [strain](../../continuum-mechanics.md#strain).

Cubic [austenitic steel](../../chemical-substance.md#austenitic-steel) does not exhibit the same intrinsic orientation-driven response merely because it is irradiated. It can nevertheless undergo [void swelling](../../engineering.md#void-swelling), [irradiation creep](../../engineering.md#irradiation-creep), thermal-stress [plasticity](../../continuum-mechanics.md#plasticity-physics) or distortion under gradients. Thus **absence of this growth mechanism does not imply dimensional stability under all reactor conditions**. Conversely, a noncubic crystal is not guaranteed to grow during every thermal cycle: constraints, inelastic accommodation and the [microstructure](../../engineering.md#microstructure) still matter.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

[crystal grain](../../thermodynamics.md#grain-in-a-polycrystal) structure controls both the source of incompatibility and its conversion into a bulk dimensional change. Separate **orientation distribution, [grain size](../../thermodynamics.md#grain-size), [crystal grain](../../thermodynamics.md#grain-in-a-polycrystal) shape and defect structure** rather than treating “fine grained” as a universal cure.

In thermal cycling, different [crystal grain](../../thermodynamics.md#grain-in-a-polycrystal) orientations rotate the [thermal expansion tensor](../../thermodynamics.md#thermal-expansion-tensor) into different laboratory directions. Bonding prevents each [crystal grain](../../thermodynamics.md#grain-in-a-polycrystal) from following its independent free [strain](../../continuum-mechanics.md#strain). Coarse [crystal grains](../../thermodynamics.md#grain-in-a-polycrystal) can produce larger surface relief and longer local mismatch distances; finer [crystal grains](../../thermodynamics.md#grain-in-a-polycrystal) can distribute the accommodation more uniformly. However, changing [grain size](../../thermodynamics.md#grain-size) also changes strength, boundary-mediated deformation and [creep](../../engineering.md#creep-deformation). A fine but strongly textured material can still show directional growth, and enhanced boundary accommodation can itself be irreversible. [crystallographic texture](../../physical-chemistry.md#crystallographic-texture) and the way mismatch is accommodated must therefore be measured separately.

For [irradiation growth](../../engineering.md#irradiation-growth), [crystallographic texture](../../physical-chemistry.md#crystallographic-texture) determines whether directional single-grain changes reinforce or cancel. An illustrative independent-grain average is

$$
\overline{\boldsymbol\varepsilon}^{g}=\sum_jv_jR_j\boldsymbol\varepsilon_j^{g}R_j^T,
$$

where $v_j$ is a [crystal grain](../../thermodynamics.md#grain-in-a-polycrystal) volume fraction and $R_j$ its orientation. A random orientation average of a traceless growth tensor is zero, whereas [crystallographic texture](../../physical-chemistry.md#crystallographic-texture) can retain a preferred bulk [strain](../../continuum-mechanics.md#strain). For an ideal hexagonal [crystal grain](../../thermodynamics.md#grain-in-a-polycrystal) with principal growth [strains](../../continuum-mechanics.md#strain) $(g,g,-2g)$, the [strain](../../continuum-mechanics.md#strain) along a direction making angle $\theta$ to the c-axis is

$$
\varepsilon_d=g(1-3\cos^2\theta),\qquad
\langle\varepsilon_d\rangle=g\big(1-3\langle\cos^2\theta\rangle\big).
$$

Random [crystallographic texture](../../physical-chemistry.md#crystallographic-texture) has $\langle\cos^2\theta\rangle=1/3$ and cancels this ideal directional growth. This is an orientation model, not proof that real [crystal grain](../../thermodynamics.md#grain-in-a-polycrystal) constraints or volume-changing processes vanish.

[grain boundaries](../../physical-chemistry.md#grain-boundary) also absorb mobile defects. Boundary spacing and aspect ratio change directional sink distances, while [dislocation](../../physical-chemistry.md#dislocation) [density](../../fluid-mechanics.md#density), [cold working](../../continuum-mechanics.md#cold-working) and [recrystallisation](../../engineering.md#recrystallisation) change competing sinks and residual [stresses](../../continuum-mechanics.md#stress). These affect the single-grain response before it is averaged. In one model compared with zirconium-alloy experiments, increasing [grain size](../../thermodynamics.md#grain-size), reducing aspect ratio or reducing [dislocation](../../physical-chemistry.md#dislocation) [density](../../fluid-mechanics.md#density) decreased predicted growth. That result is a useful counterexample to assuming that smaller [crystal grains](../../thermodynamics.md#grain-in-a-polycrystal) always reduce [irradiation growth](../../engineering.md#irradiation-growth).[Transactions of the Japan Institute of Metals 29, 970–976, abstract and stated microstructural trends](../../engineering.md#effects-of-microstructural-factors-on-irradiation-growth-in-zirconium-base-alloys-by-noriyuki-sadaoka-and-motomasa-fuse)

## 2

↑ **Parent:** [Module NE4](paper-ne4.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

**[helium](../../chemical-substance.md#helium) changes cavity stability and [ductility](../../engineering.md#ductility); [void swelling](../../engineering.md#void-swelling) changes bulk volume and component dimensions.** These effects interact, but a [helium](../../chemical-substance.md#helium) bubble and a vacancy-rich void are not interchangeable descriptions.

[neutron](../../neutron.md) reactions produce [helium](../../chemical-substance.md#helium) from alloy constituents and impurities. For example, capture by boron-10 can produce [helium](../../chemical-substance.md#helium) through $^{10}\mathrm B+n\longrightarrow{}^7\mathrm{Li}+{}^4\mathrm{He}$; the production per displacement dose depends on composition and [neutron](../../neutron.md) spectrum. Retained [helium](../../chemical-substance.md#helium) has low solubility and is trapped at defects or in bubbles. Bubble nucleation and growth at [grain boundaries](../../physical-chemistry.md#grain-boundary) can assist intergranular cavitation, lowering tensile [ductility](../../engineering.md#ductility) and creep-rupture resistance, particularly when [temperature](../../temperature.md) permits the relevant transport. This is important even before a large bulk [void swelling](../../engineering.md#void-swelling) is measurable. A primary study linked high-temperature [ductility](../../engineering.md#ductility) loss to observed bubbles and grain-boundary weakening in irradiated [stainless steel](../../chemical-substance.md#stainless-steel).[Nature 211, 291–292, abstract: mechanical observations, thin-foil bubbles and boundary-bubble interpretation](../../engineering.md#high-temperature-embrittlement-of-stainless-steel-irradiated-in-fast-fluxes-by-a-s-fraser-and-others)

[displacement damage](../../engineering.md#displacement-damage) continuously creates [vacancies](../../physical-chemistry.md#vacancy) and [self-interstitials](../../physical-chemistry.md#self-interstitial). Their different capture efficiencies at [dislocations](../../physical-chemistry.md#dislocation) and other sinks can leave a [vacancy supersaturation](../../physical-chemistry.md#vacancy-supersaturation) available to cavities. A stable cavity grows when its net [vacancy](../../physical-chemistry.md#vacancy) uptake exceeds [vacancy](../../physical-chemistry.md#vacancy) emission and interstitial absorption. [helium](../../chemical-substance.md#helium) can help stabilise small nuclei, but the later volume increase is not simply the volume of gas inserted into an unchanged matrix. Changing [helium](../../chemical-substance.md#helium) content can also change cavity number, size and competition for [point defects](../../physical-chemistry.md#point-defect); a universal proportionality between [helium](../../chemical-substance.md#helium) concentration and [void swelling](../../engineering.md#void-swelling) is not justified.

For [nuclear fuel cladding](../../engineering.md#nuclear-fuel-cladding), [void swelling](../../engineering.md#void-swelling) can enlarge the diameter, alter the fuel–[nuclear fuel cladding](../../engineering.md#nuclear-fuel-cladding) gap, reduce clearances and distort [reactor coolant](../../engineering.md#reactor-coolant) channels or nearby structures. Nonuniform [void swelling](../../engineering.md#void-swelling) generates additional [stresses](../../continuum-mechanics.md#stress). Bubble-assisted embrittlement and stress-dependent [creep](../../engineering.md#creep-deformation) then affect the ability of the wall to contain the fuel and internal pressure. The relevant measurements combine [density](../../fluid-mechanics.md#density) or volume change, dimensional [strain](../../continuum-mechanics.md#strain), cavity microscopy and mechanical tests. Pressurised-tube experiments explicitly separated [void swelling](../../engineering.md#void-swelling), [creep](../../engineering.md#creep-deformation), plastic [strain](../../continuum-mechanics.md#strain) and [precipitation](../../chemical-reaction.md#precipitation-chemistry) [strain](../../continuum-mechanics.md#strain); [void swelling](../../engineering.md#void-swelling) itself was approximately isotropic in that study.[Journal of Nuclear Materials 367–370, 954–959; PNNL abstract, separation of strain components](../../engineering.md#the-influence-of-cold-work-level-on-the-irradiation-creep-and-swelling-of-aisi-316-stainless-steel-by-e-r-gilbert-and-f-a-garner)

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

[void swelling](../../engineering.md#void-swelling) has a **[temperature](../../temperature.md) window**, rather than increasing monotonically with irradiation [temperature](../../temperature.md). At sufficiently low [temperature](../../temperature.md), [vacancy](../../physical-chemistry.md#vacancy) migration and cavity growth are slow. At intermediate [temperature](../../temperature.md), mobile defects, stable nuclei and unequal sink capture can support rapid cavity growth. At higher [temperature](../../temperature.md), increased [vacancy](../../physical-chemistry.md#vacancy) emission, recombination and changing sink populations can reduce the [vacancy supersaturation](../../physical-chemistry.md#vacancy-supersaturation) and net [void swelling](../../engineering.md#void-swelling). The precise peak depends on alloy, spectrum, dose rate and starting [microstructure](../../engineering.md#microstructure); lower [void swelling](../../engineering.md#void-swelling) at high [temperature](../../temperature.md) does not mean that [creep](../../engineering.md#creep-deformation) or [helium embrittlement](../../engineering.md#helium-embrittlement) is harmless there.

Distinguish [void swelling](../../engineering.md#void-swelling) $S=\Delta V/V_0$ from its slope. With displacement dose $D$, a simple schematic description is

$$
S(D)\simeq0\quad(D<D_0),\qquad
S(D)\simeq k(T)(D-D_0)\quad(D>D_0),
$$

where $D_0$ represents incubation and $k(T)$ an approximately constant post-transient slope over a limited range. Real nucleation and sink evolution make the transition smooth; neither $D_0$ nor $k$ is a universal material constant. At larger dose, microstructural or compositional evolution may change the slope again.

[neutron fluence](../../neutron.md#neutron-fluence) is an integrated exposure, $\Phi=\int\phi\,dt$. Under an unchanged spectrum it can track displacement dose, but equal fluence does not necessarily imply equal damage or [helium](../../chemical-substance.md#helium) production. Even equal dpa can give different [void swelling](../../engineering.md#void-swelling) at different dose rates because recombination and transport compete in real time. Thus compare specimens at specified [temperature](../../temperature.md), spectrum, dose rate and metallurgical condition; do not transfer one [void swelling](../../engineering.md#void-swelling) curve using fluence alone.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

**Delay cavity nucleation and prevent a large sustained [vacancy](../../physical-chemistry.md#vacancy) flux to growing cavities.** Select an austenitic alloy composition and heat treatment demonstrated to have low [void swelling](../../engineering.md#void-swelling) in the intended spectrum and [temperature](../../temperature.md) range; modest composition changes can alter [precipitation](../../chemical-reaction.md#precipitation-chemistry), segregation and sink evolution. The grade label alone is insufficient.

[cold working](../../continuum-mechanics.md#cold-working) supplies a [dislocation](../../physical-chemistry.md#dislocation) population that can alter defect capture and extend the low-swelling transient. Stable fine precipitates or other engineered sinks can promote defect removal, but capture bias matters as well as sink count. Irradiation and thermal recovery can erase the starting [microstructure](../../engineering.md#microstructure), so an initially favourable state must be checked at relevant dose. Controlled impurity and helium-producing constituent contents can reduce harmful gas effects, subject to [corrosion](../../engineering.md#corrosion) resistance and phase-stability requirements.

Operating outside a strong-swelling regime, reducing accumulated exposure or replacing components before their qualified limit are complementary measures. Each trades against other constraints such as [corrosion](../../engineering.md#corrosion), [creep](../../engineering.md#creep-deformation), [ductility](../../engineering.md#ductility) and heat removal. **“More [cold working](../../continuum-mechanics.md#cold-working)” or “more sinks” is not an unlimited prescription.** Measurements must separate [void swelling](../../engineering.md#void-swelling) from [creep](../../engineering.md#creep-deformation); reducing one does not establish that the other was reduced. The pressurised-tube study is a particularly useful control because, after separating stress-enhanced [void swelling](../../engineering.md#void-swelling), its derived [creep](../../engineering.md#creep-deformation) [strains](../../continuum-mechanics.md#strain) were similar for annealed and cold-worked specimens.[PNNL abstract, comparison after correction for stress-enhanced swelling](../../engineering.md#the-influence-of-cold-work-level-on-the-irradiation-creep-and-swelling-of-aisi-316-stainless-steel-by-e-r-gilbert-and-f-a-garner)

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Both terms concern **time-dependent [strain](../../continuum-mechanics.md#strain) under [stress](../../continuum-mechanics.md#stress)**. Here [radiation-enhanced creep](../../engineering.md#radiation-enhanced-creep) means irradiation accelerating a mechanism that also operates thermally, whereas [radiation-induced creep](../../engineering.md#radiation-induced-creep) emphasises deformation driven by irradiation-specific defect fluxes. The literature sometimes uses [irradiation creep](../../engineering.md#irradiation-creep) as an umbrella, so identifying the mechanism is more informative than treating the names as mutually exclusive experimental categories.

[radiation-enhanced diffusion](../../engineering.md#radiation-enhanced-diffusion) maintains mobile point-defect concentrations above their thermal equilibrium values. Under a load, this can accelerate diffusion-mediated deformation or [dislocation climb](../../physical-chemistry.md#dislocation-climb) and thereby enhance a [creep](../../engineering.md#creep-deformation) mechanism. The effect depends on [temperature](../../temperature.md), defect production, recombination and sinks; simply raising the specimen [temperature](../../temperature.md) by radiation heating is a different explanation and must be controlled.

[radiation-induced creep](../../engineering.md#radiation-induced-creep) can remain important where unirradiated [creep](../../engineering.md#creep-deformation) is small. [stress-induced preferential absorption](../../engineering.md#stress-induced-preferential-absorption) gives differently oriented [dislocations](../../physical-chemistry.md#dislocation) unequal capture of irradiation-produced defects, producing directional climb. Climb can also enable further glide by relieving obstacles. A schematic low-stress relation is

$$
\frac{d\varepsilon_{\rm irr}}{dD}\simeq B_{\rm irr}\sigma,
\qquad
\dot\varepsilon_{\rm irr}\simeq B_{\rm irr}\sigma\dot D,
$$

with a condition-dependent compliance $B_{\rm irr}$, not a universal constitutive law. Coupling to [void swelling](../../engineering.md#void-swelling) and evolving sinks can add further terms.

Compare stressed and unstressed specimens in and out of irradiation at matched actual [temperature](../../temperature.md), and resolve longitudinal, transverse and volumetric [strains](../../continuum-mechanics.md#strain). Unstressed [irradiation growth](../../engineering.md#irradiation-growth) or [void swelling](../../engineering.md#void-swelling) is not itself evidence of [creep](../../engineering.md#creep-deformation), and stress-enhanced [void swelling](../../engineering.md#void-swelling) must not be included automatically in a fitted [creep](../../engineering.md#creep-deformation) [strain](../../continuum-mechanics.md#strain). These controls distinguish a mechanical response to irradiation defects from ordinary [creep](../../engineering.md#creep-deformation) or a different dimensional-change mechanism.

## 3

↑ **Parent:** [Module NE4](paper-ne4.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

**A [reactor coolant](../../engineering.md#reactor-coolant) must remove heat reliably while remaining compatible with the core.** Desirable properties include adequate [heat capacity](../../heat.md#heat-capacity) and heat transfer, manageable viscosity and pumping demand, stability over the operating range, limited [corrosion](../../engineering.md#corrosion) of fuel and structures, acceptable [neutron](../../neutron.md) absorption and activation, and a tolerable leakage or chemical-reaction hazard. **[water](../../chemical-substance.md#water)** is a standard example in light-water reactors: it transfers heat well and also moderates, but pressure, boiling behaviour, [corrosion](../../engineering.md#corrosion) chemistry and loss of inventory must be managed. No single [reactor coolant](../../engineering.md#reactor-coolant) is best independently of reactor design.

**A control-rod material must absorb [neutrons](../../neutron.md) effectively and retain mechanical and chemical integrity.** It needs a suitable absorption cross section over the relevant spectrum, adequate absorber inventory over life, manageable capture heating and transmutation products, and compatibility with its sheath and [reactor coolant](../../engineering.md#reactor-coolant). **[boron carbide](../../chemical-substance.md#boron-carbide)** is an example. Depletion, gas generation, [radiation-induced swelling](../../engineering.md#radiation-induced-swelling) and cracking must be allowed for; a large initial cross section alone does not establish lifetime performance.

**A [neutron moderator](../../neutron.md#neutron-moderator) must slow [neutrons](../../neutron.md) efficiently while absorbing relatively few.** Light nuclei provide effective energy transfer per collision, but absorption, [density](../../fluid-mechanics.md#density), radiation stability, purity and temperature-dependent properties determine the usable moderation. **[heavy water](../../ionic-bonding.md#heavy-water)** is an example combining effective slowing with low parasitic absorption; [graphite](../../chemical-substance.md#graphite) is another possible material in different designs. Heat removal and compatibility remain necessary even though moderation is its principal neutronic role.

**[nuclear fuel cladding](../../engineering.md#nuclear-fuel-cladding) must retain fuel and [fission products](../../physics.md#fission-product) while transferring heat and carrying load.** Desirable properties include [corrosion](../../engineering.md#corrosion) resistance, low [neutron](../../neutron.md) absorption, adequate [thermal conductivity](../../heat.md#thermal-conductivity), strength and [ductility](../../engineering.md#ductility), resistance to [irradiation growth](../../engineering.md#irradiation-growth), [void swelling](../../engineering.md#void-swelling) and [creep](../../engineering.md#creep-deformation), and compatibility with fuel and [reactor coolant](../../engineering.md#reactor-coolant). **A [zirconium alloy](../../chemical-substance.md#zirconium-alloy) such as [Zircaloy](../../chemical-substance.md#zircaloy)** is a light-water-reactor example. Hydrogen uptake, [corrosion](../../engineering.md#corrosion) and irradiation response constrain service; the low absorption benefit does not eliminate these materials problems.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A useful fuel combines **neutronic suitability, heat removal, containment and dimensional stability**. A sufficient fissile inventory and acceptable [neutron](../../neutron.md) economy permit the intended power and exposure, while unnecessary parasitic absorption wastes [neutrons](../../neutron.md). These requirements are reactor-specific rather than a recommendation for one universal composition.

A high melting margin and stable phases help preserve geometry. Good [thermal conductivity](../../heat.md#thermal-conductivity) reduces the centre-to-surface [temperature](../../temperature.md) rise and associated thermal [stress](../../continuum-mechanics.md#stress); [heat capacity](../../heat.md#heat-capacity) helps moderate transient [temperature](../../temperature.md) changes. Chemical stability and compatibility with [reactor coolant](../../engineering.md#reactor-coolant) and [nuclear fuel cladding](../../engineering.md#nuclear-fuel-cladding) reduce [corrosion](../../engineering.md#corrosion) and reactions at the interface with [nuclear fuel cladding](../../engineering.md#nuclear-fuel-cladding). Oxygen chemistry and other composition variables can affect both transport and interface reactions.

Under irradiation the fuel should tolerate [displacement damage](../../engineering.md#displacement-damage), restructuring, [radiation-induced swelling](../../engineering.md#radiation-induced-swelling) and [fission gas](../../engineering.md#fission-gas) accumulation without unacceptable cracking, gap closure or pressure. Retention of radionuclides and controlled release of [fission gas](../../engineering.md#fission-gas) support the [nuclear fuel cladding](../../engineering.md#nuclear-fuel-cladding)'s containment function. Predictable [creep](../../engineering.md#creep-deformation) can relieve [stress](../../continuum-mechanics.md#stress), but excessive deformation may compromise geometry. Fabrication reproducibility, inspectable [microstructure](../../engineering.md#microstructure), resource availability and the practicability of subsequent waste management also matter.

**[uranium dioxide](../../engineering.md#uranium-dioxide) illustrates the compromises:** it is a chemically robust, high-melting ceramic fuel, but its relatively limited [thermal conductivity](../../heat.md#thermal-conductivity), irradiation-dependent [microstructure](../../engineering.md#microstructure) and gas behaviour require explicit thermal and mechanical design margins. A desirable individual property does not establish the performance of the coupled [nuclear fuel](../../engineering.md#nuclear-fuel) and [nuclear fuel cladding](../../engineering.md#nuclear-fuel-cladding) system.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

[plutonium](../../chemical-substance.md#plutonium) introduces **[decay heat](../../physics.md#decay-heat), self-irradiation and composition-sensitive thermochemical behaviour**, as well as demanding radiological handling and material accountancy. [isotopic composition](../../chemical-substance.md#isotopic-composition) affects heat and [neutron](../../neutron.md) production, so total [plutonium](../../chemical-substance.md#plutonium) mass alone does not specify the handling environment. The elemental metal also has inconvenient allotropic and thermal behaviour; using an appropriate stable ceramic fuel form avoids treating bare metal as a straightforward substitute for [uranium](../../chemical-substance.md#uranium) oxide.

In [mixed oxide fuel](../../engineering.md#mixed-oxide-fuel), [plutonium dioxide](../../engineering.md#plutonium-dioxide) and [uranium dioxide](../../engineering.md#uranium-dioxide) form the engineered ceramic system. Important challenges are composition uniformity, [thermal conductivity](../../heat.md#thermal-conductivity) and melting margin, oxygen chemistry, restructuring and [fission gas](../../engineering.md#fission-gas) behaviour, and compatibility with [nuclear fuel cladding](../../engineering.md#nuclear-fuel-cladding). A local composition variation can produce a local power or [temperature](../../temperature.md) variation. During service, [actinide](../../chemical-substance.md#actinide) redistribution can change the initial spatial distribution; its direction cannot be inferred from the [temperature](../../temperature.md) gradient alone. Autoradiographic examination of irradiated mixed-oxide pins directly investigated the competing transport effects.[Journal of Nuclear Materials 47, 187–197, abstract: irradiated-pin observations, thermal diffusion, evaporation–condensation and oxygen chemistry](../../engineering.md#plutonium-redistribution-in-fast-reactor-mixed-oxide-fuel-pins-by-m-bober-and-others)

Mitigation is to use a characterised fuel form and isotopic inventory, qualify composition and [microstructure](../../engineering.md#microstructure) uniformity, retain suitable thermal margins, and establish irradiation performance and interface compatibility. [radioactive material confinement](../../engineering.md#radioactive-material-confinement), remote or protected handling and waste management address the accompanying contamination and exposure problems. These are **materials requirements and verification objectives**; no [plutonium](../../chemical-substance.md#plutonium) preparation, separation or fuel-manufacturing procedure is needed to answer them.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The two historically dominant commercial processes are **[gaseous diffusion enrichment](../../engineering.md#gaseous-diffusion-enrichment) and [gas centrifuge enrichment](../../engineering.md#gas-centrifuge-enrichment)**. The first exploits differences in molecular transport through a barrier; the second exploits mass-dependent redistribution in a rotating gas. Both are isotope-separation principles rather than chemical separation of [uranium](../../chemical-substance.md#uranium) from another element.

**[gas centrifuge enrichment](../../engineering.md#gas-centrifuge-enrichment) had become predominant by the time of this examination.** Its much smaller electricity demand reduces a major operating cost of [diffusion](../../thermodynamics.md#diffusion) technology. Modular capacity and the replacement of ageing [diffusion](../../thermodynamics.md#diffusion) plants contributed to commercial adoption. This historical conclusion does not require machine dimensions, operating conditions or a cascade design. The United States' final operating [diffusion](../../thermodynamics.md#diffusion) plant closed in 2013, consistent with the earlier transition rather than a claim based on current plant counts.[Institutional historical sections on gas centrifuges, electricity demand and diffusion-plant closures](../../engineering.md#backgrounder-on-uranium-enrichment-by-the-united-states-nuclear-regulatory-commission)

## 4

↑ **Parent:** [Module NE4](paper-ne4.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

**[glass](../../chemical-substance.md#glass) accommodates a chemically diverse waste inventory without requiring every constituent to fit one specific crystal site.** A borosilicate network can incorporate many constituents while producing a dense monolithic waste form. An established melt-and-pour approach permits remote processing and a reproducible package geometry; suitable formulations combine useful waste loading with low aqueous release rates. The absence of crystalline [grain boundaries](../../physical-chemistry.md#grain-boundary) also removes one possible preferential path, although cracks or other heterogeneity can still occur.

The flexibility has limits. Some constituents have limited solubility or can separate into undesired phases, and increasing waste loading can impair processability or durability. Melting can release volatile constituents that require capture and generate secondary wastes. Cooling [stresses](../../continuum-mechanics.md#stress) may crack the product and enlarge its accessible surface; [devitrification](../../chemical-substance.md#devitrification) or phase separation can change chemical durability. Heat and radiation can change [density](../../fluid-mechanics.md#density), bonding or [microstructure](../../engineering.md#microstructure) even though the starting [glass](../../chemical-substance.md#glass) is already noncrystalline.

Most importantly, **[glass](../../chemical-substance.md#glass) is an immobilisation medium, not an assertion of zero reaction with [water](../../chemical-substance.md#water)**. Durability depends on composition, [temperature](../../temperature.md), solution chemistry and the evolution of alteration products. A low initial leach rate does not alone demonstrate long-term behaviour, and an amorphous structure does not make the material inert. Container and repository barriers complement rather than duplicate the [glass](../../chemical-substance.md#glass)'s role. A suitable choice therefore balances processing, composition tolerance, radiation response and aqueous durability instead of maximising only one property.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Write $SA=S$ for the exposed [glass](../../chemical-substance.md#glass) area. If $C_e$ is the blank-corrected dissolved mass concentration of element $e$, $x_e$ its initial [mass fraction](../../mixture.md#mass-fraction) in the [glass](../../chemical-substance.md#glass) and $V$ the leachate volume, then

$$
NL_e=\frac{C_e}{x_e(SA/V)}=\boxed{\frac{C_eV}{x_eSA}}.
$$

The numerator is the released element mass measured in solution. Dividing by $x_e$ converts this to an equivalent mass of the original [glass](../../chemical-substance.md#glass), while dividing by $SA$ expresses that mass per exposed area. With $C_e$ in $\mathrm{g\,L^{-1}}$ and $SA/V$ in $\mathrm{m^2\,L^{-1}}$, $NL_e$ has units **$\mathrm{g\,m^{-2}}$ of glass-equivalent release**. The fraction $x_e$ must be used as a fraction, not an unconverted percentage.

These corrections allow comparison of specimens of different size and composition without confusing a lower concentration with better durability. State how the area was measured; geometric area and a rough powder's accessible area need not coincide. For repeated sampling, include element mass removed in earlier aliquots and the volume remaining; for an initial blank in the leachant, subtract its corresponding inventory. Surface cracking and evolving [porosity](../../porous-media-flow.md#porosity) can make a rate based on initial area differ from a rate based on the true reactive area.

Under [congruent glass dissolution](../../engineering.md#congruent-glass-dissolution), constituents enter solution in their bulk proportions, so their correctly normalised releases coincide. Preferential [sodium](../../chemical-substance.md#sodium) release by [ion exchange](../../engineering.md#ion-exchange) can instead give $NL_{\rm Na}>NL_{\rm Si}$, while [silicon](../../chemical-substance.md#silicon) retention in a gel or secondary precipitate can depress its dissolved release. **Noncoincident curves show nonstoichiometric aqueous release, but do not uniquely identify the mechanism.** Conversely, solution coincidence does not by itself establish that no secondary reactions occurred. A complete inference compares solution inventories with altered solids.

Normalisation removes composition and first-order area/volume scaling; **it does not make different [pH](../../acid-base-chemistry.md#ph), [temperature](../../temperature.md), solution composition or contact histories equivalent**. In a batch test, even the same initial [water](../../chemical-substance.md#water) changes composition and [pH](../../acid-base-chemistry.md#ph) as reaction proceeds. Reporting those conditions and time is essential for a transferable comparison rather than treating $NL_e$ as a condition-independent material constant.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

[water](../../chemical-substance.md#water) first interacts with accessible surface sites and enters the near-surface region. Exchange of alkali ions with hydrogen-bearing species can release [sodium](../../chemical-substance.md#sodium) before the silicate network has dissolved in bulk. A schematic site exchange is

$$
\mathrm{\equiv SiO^-Na^+}+\mathrm{H^+}\longrightarrow\mathrm{\equiv SiOH}+\mathrm{Na^+}.
$$

[hydrolysis](../../chemical-reaction.md#hydrolysis) also breaks network linkages, illustrated by

$$
\mathrm{\equiv Si-O-Si\equiv}+\mathrm{H_2O}
\rightleftharpoons2\,\mathrm{\equiv SiOH}.
$$

Boron-containing linkages and the rest of the network react in a composition- and pH-dependent way. Alkali exchange changes the [water](../../chemical-substance.md#water) chemistry, and network [hydrolysis](../../chemical-reaction.md#hydrolysis) releases or rearranges constituents rather than simply removing an intact molecular [glass](../../chemical-substance.md#glass) unit.

In a finite batch of initially deionised [water](../../chemical-substance.md#water), dissolved products accumulate and [pH](../../acid-base-chemistry.md#ph) evolves. [silicon](../../chemical-substance.md#silicon) can be retained in a hydrated alteration gel, and condensation or restructuring changes that layer's connectivity and transport properties. Reduced chemical driving force and a less permeable interfacial layer can lower the rate; a [residual glass alteration rate](../../engineering.md#residual-glass-alteration-rate) can persist rather than all reaction stopping at an apparent plateau. Atomistic work published before the examination provides one account of how gel restructuring can hinder hydrated-species transport, without making that account universal for all [glasses](../../chemical-substance.md#glass).[npj Materials Degradation 3, 6, 7 February 2019; hydrated-gel restructuring and transport simulations](../../engineering.md#atomistic-origin-of-the-passivation-effect-in-hydrated-silicate-glasses-by-tao-du-and-others)

<a id="4/c/image-illustrative-normalised-sodium-boron-and-silicon-releases-in-one-batch-glass-alteration-scenario"></a>
![](../../past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge/2019/paper-ne4-glass-release.png)

**[Figure 1](#4/c/image-illustrative-normalised-sodium-boron-and-silicon-releases-in-one-batch-glass-alteration-scenario). Illustrative normalised sodium, boron and silicon releases in one batch-glass-alteration scenario**.

The original sketch shows **one plausible scenario, not measured data or a universal ordering**. [sodium](../../chemical-substance.md#sodium) initially rises rapidly through exchange. [boron](../../chemical-substance.md#boron) acts as a relatively mobile tracer of network alteration, while a smaller solution [silicon](../../chemical-substance.md#silicon) release reflects retention in an alteration layer. The slopes subsequently decrease as batch chemistry and the layer evolve; small continuing slopes represent residual release. Offsets can remain even if later release rates become similar. Initial deionised [water](../../chemical-substance.md#water) does not imply that the solution remains neutral or dilute throughout the test.

[boron](../../chemical-substance.md#boron) need not be an ideal fully released tracer: it can be retained in some gels, changing the relation between aqueous [boron](../../chemical-substance.md#boron) and the depth of alteration. A later study, published in **2020**, explicitly compared solution release with solid depth profiles and demonstrated that limitation; it is cited as a subsequent qualification, not evidence available to a student in May 2019.[npj Materials Degradation 4, 41, 11 December 2020; results comparing boron release with alteration-layer profiles](../../engineering.md#insights-into-the-mechanisms-controlling-the-residual-corrosion-rate-of-borosilicate-glasses-by-stephane-gin-and-others)

Secondary phases can further modify dissolved inventories and, by consuming solution components, sometimes accelerate alteration again. Neither a permanently flat terminal curve nor a later acceleration is compulsory. Without a specified [glass](../../chemical-substance.md#glass), [temperature](../../temperature.md), area/volume ratio and solution history, the defensible sketch communicates exchange, network reaction and evolving retention, with those assumptions stated.

## ↑ Ancestors (7)

1. [2019](../2019.md)
2. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
3. [MPhil in nuclear energy course of the University of Cambridge](../../university-of-cambridge.md#mphil-in-nuclear-energy-course-of-the-university-of-cambridge)
4. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
5. [University of Cambridge](../../university-of-cambridge.md)
6. [List of universities](../../README.md#list-of-universities)
7. [Codex Wiki](../../README.md)
