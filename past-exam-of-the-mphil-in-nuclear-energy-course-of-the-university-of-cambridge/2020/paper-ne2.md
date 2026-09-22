# Module NE2

↑ **Parent:** [2020](../2020.md)

Original paper: [Released original PDF, physical pages 28–30; questions on pages 29–30](https://www.whatdotheyknow.com/request/past_exam_papers_16/response/2088673/attach/3/FOI%202022%20471%20Smith%20materials.pdf?cookie_passthrough=1#page=28).

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

## 1

↑ **Parent:** [Module NE2](paper-ne2.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Take one-dimensional [steady state](../../dynamical-systems.md#steady-state) [thermal conduction](../../heat.md#thermal-conduction), constant [thermal conductivity](../../heat.md#thermal-conductivity) $k>0$, and positive [volumetric heat generation rate](../../heat.md#volumetric-heat-generation-rate). Write $q_0=q'''_0$ for brevity, and let $x$ increase away from the illuminated face. [Conservation of energy](../../mathematical-physics.md#conservation-of-energy) and [Fourier's law](../../heat.md#fourier-s-law) give

$$
\frac{d}{dx}\left(-k\frac{dT}{dx}\right)=q_0e^{-\mu x},
\qquad T(0)=T(a)=T_0.
$$

Thus $T''=-(q_0/k)e^{-\mu x}<0$: the profile is strictly concave and any stationary point is its unique maximum. Two [integrations](../../integral.md) and the equal-surface [boundary conditions](../../differential-equation.md#boundary-condition) yield the [exponential slab heating](../../heat.md#slab-conduction-with-exponentially-decaying-heat-generation) solution

$$
\boxed{T(x)-T_0=\frac{q_0}{k\mu^2}
\left[1-e^{-\mu x}-(1-e^{-\mu a})\frac{x}{a}\right].}
$$

Its derivative is

$$
T'(x)=\frac{q_0}{k\mu}
\left[e^{-\mu x}-\frac{1-e^{-\mu a}}{\mu a}\right].
$$

Define $\beta=\mu a$ and $C=(1-e^{-\beta})/\beta$. Setting $T'(x_m)=0$ gives **the distance from the illuminated surface**:

$$
\boxed{x_m=\frac1\mu\ln\frac{\mu a}{1-e^{-\mu a}}=-\frac{\ln C}{\mu}.}
$$

For $\beta>0$, $e^{-\beta}<C<1$, so $0<x_m<a$. More specifically $C=e^{-\beta/2}\sinh(\beta/2)/(\beta/2)>e^{-\beta/2}$, hence $x_m<a/2$: the peak is nearer the more strongly heated face.

The apparent singularity at $\mu=0$ is removable. Expansion gives

$$
\frac{x_m}{a}=\frac12-\frac{\beta}{24}+O(\beta^3),
\qquad
T(x)-T_0\longrightarrow\frac{q_0}{2k}x(a-x).
$$

The uniform-heating limit therefore has its maximum at $a/2$, as symmetry requires.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

At the maximum found in part(a), $e^{-\mu x_m}=C$ and $(1-e^{-\beta})x_m/a=C\mu x_m=-C\ln C$. Substitution into the [exponential slab heating](../../heat.md#slab-conduction-with-exponentially-decaying-heat-generation) solution gives

$$
\boxed{T_{\max}-T_0=\frac{q_0}{k\mu^2}\left(1-C+C\ln C\right),
\qquad C=\frac{1-e^{-\mu a}}{\mu a}.}
$$

For $0<C<1$, the function $1-C+C\ln C$ is positive: it vanishes at $C=1$ and has derivative $\ln C<0$. Thus the interior [temperature](../../temperature.md) exceeds the common surface [temperature](../../temperature.md), consistently with positive internal heating.

A convenient dimensionless form uses $\xi=x/a$:

$$
\theta(\xi)=\frac{k(T-T_0)}{q_0a^2}
=\frac{1-e^{-\beta\xi}-(1-e^{-\beta})\xi}{\beta^2}.
$$

As $\beta\to0$, $\theta\to\xi(1-\xi)/2$, giving the check

$$
\boxed{T_{\max}-T_0\longrightarrow\frac{q_0a^2}{8k}.}
$$

<a id="1/b/image-original-normalized-slab-temperature-profiles-calculated-from-the-exponential-slab-heating-solution-markers-indicate-the-maxima"></a>


![](../../past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge/2020/paper-ne2-slab-temperature.png)

**[Figure 1](#1/b/image-original-normalized-slab-temperature-profiles-calculated-from-the-exponential-slab-heating-solution-markers-indicate-the-maxima). Original normalized slab temperature profiles calculated from the exponential slab heating solution; markers indicate the maxima**.

The graph holds the normalization $q_0a^2/k$ fixed. Its decreasing peaks with increasing $\beta$ reflect a decreasing source away from the illuminated face under that comparison; they do not assert the same trend at fixed total absorbed power.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The two outward surface normals point in opposite directions. With positive [heat flux](../../heat.md#heat-flux-density) defined as heat leaving each face, [Fourier's law](../../heat.md#fourier-s-law) gives

$$
q''_{\rm left}=kT'(0),\qquad q''_{\rm right}=-kT'(a).
$$

Using the derivative from part(a), **the removed fluxes per unit face area** are

$$
\boxed{q''_{\rm left}=\frac{q_0}{\mu}\left[1-\frac{1-e^{-\mu a}}{\mu a}\right]
=\frac{q_0}{\mu}(1-C),}
$$



$$
\boxed{q''_{\rm right}=\frac{q_0}{\mu}\left[\frac{1-e^{-\mu a}}{\mu a}-e^{-\mu a}\right]
=\frac{q_0}{\mu}(C-e^{-\beta}).}
$$

Both are positive because $e^{-\beta}<C<1$. Their sum satisfies the independent [conservation of energy](../../mathematical-physics.md#conservation-of-energy) check

$$
q''_{\rm left}+q''_{\rm right}
=\frac{q_0}{\mu}(1-e^{-\mu a})
=\int_0^a q_0e^{-\mu x}\,dx.
$$

The illuminated face removes more [heat](../../heat.md) because heating is concentrated nearer it. Equivalently, weighting each source slice by the fraction of its heat conducted to either equal-temperature boundary gives

$$
q''_{\rm left}=\int_0^a q'''(x)\frac{a-x}{a}\,dx,
\qquad
q''_{\rm right}=\int_0^a q'''(x)\frac{x}{a}\,dx.
$$

A decreasing source weights the left face more strongly. In the uniform-heating limit, **each face removes $q_0a/2$**. If a heat removal rate rather than a flux is wanted, multiply the relevant expression by the face area.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [exponential slab heating](../../heat.md#slab-conduction-with-exponentially-decaying-heat-generation) solution separates three useful controls: the heat source, the conductive path and the boundary [temperature](../../temperature.md). **Reduce deposited power, improve [thermal conduction](../../heat.md#thermal-conduction), shorten paths to a cooled surface, or lower the actual surface [temperature](../../temperature.md).** Each proposal has to preserve the shield's radiation-protection function.

Reduce incident photon intensity, intercept part of the beam in a separately cooled upstream shield, or distribute the deposited power over a larger cooled region. These reduce the relevant [volumetric heat generation rate](../../heat.md#volumetric-heat-generation-rate) or local heat load. Intermittent exposure can reduce average heating, but the peak then requires a transient [heat equation](../../diffusion-equation.md#heat-equation) calculation; a smaller average alone does not establish a safe pulse maximum.

Increase the effective [thermal conductivity](../../heat.md#thermal-conductivity), for example through a suitable material or a well-bonded conductive path to a heat sink. Reduce contact [thermal resistance](../../heat.md#thermal-resistance) in any added path. Material substitution must also satisfy shielding, mechanical and environmental constraints.

Shorten the maximum conduction distance by introducing cooled internal surfaces or dividing the shield into thinner, separately cooled layers. Reducing the thickness of a single slab lowers its temperature rise at fixed $q_0$ and $\mu$, but also reduces attenuation; it is not automatically an acceptable shield modification. A layered arrangement can preserve the required total shielding while changing the thermal boundary-value problem.

Lower the cooling-air [temperature](../../temperature.md), improve [forced convection](../../convection.md#forced-convection) by appropriate flow and surface design, enlarge the heat-exchange area, or use a more effective [coolant](../../engineering.md#coolant) where compatible. These can lower the actual boundary [temperature](../../temperature.md) when the external cooling is modeled. **In the stipulated model $T_0$ is already prescribed**: increasing the external [heat transfer coefficient](../../linear-ordinary-differential-equation.md#heat-transfer-coefficient) while holding $T_0$ fixed leaves the calculated interior profile unchanged. It helps physically by reducing the surface-to-coolant temperature difference under a heat load.

Do not change the attenuation coefficient independently of the heat-source normalization without explaining the comparison. At fixed incident photon energy flux, the entrance deposition $q_0$ generally changes with absorption properties. A larger $\mu$ with artificially fixed $q_0$ is a different experiment. Similarly, increasing total slab heat capacity delays heating but does not lower the [steady state](../../dynamical-systems.md#steady-state) maximum for an unchanged source and unchanged thermal boundary conditions.

## 2

↑ **Parent:** [Module NE2](paper-ne2.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use a common comparison for all of question2: retain the same number and height of fuel rods and approximately the same normalized rod-power shape; reduce [fuel lattice pitch](../../engineering.md#fuel-lattice-pitch) by making the active core cross-section smaller. Compare otherwise similar operating states of an initially [under-moderated reactor](../../physics.md#under-moderated-reactor), typical of a [pressurized water reactor](../../physics.md#pressurized-water-reactor). Rod number, core height, reflector and control settings are not all fixed explicitly by the question, so these are stated assumptions. Keeping the external core envelope fixed while inserting more rods would be a different comparison.

**[Reactor reactivity](../../physics.md#reactivity-nuclear-engineering) normally decreases at unchanged controls and reference temperatures.** Less water per fuel atom reduces [neutron moderation](../../neutron.md#neutron-moderation) and increases resonance absorption during slowing down. Reduced absorption in the water partly compensates, but on the under-moderated side the net lattice tendency is lower multiplication. This is the usual under-moderation argument, rather than a universal rule for arbitrary fuel lattices.[Module NP-03, pp.24–25, Moderator Effects: competing resonance escape and thermal utilization](../../engineering.md#nuclear-physics-and-reactor-theory-volume-2-by-the-united-states-department-of-energy)

**[Neutron leakage](../../physics.md#neutron-leakage) would usually tend to increase.** The smaller transverse core extent increases the geometric tendency to leak, and reduced moderation generally increases the slowing-down distance. There are competing changes in fuel absorption, transport lengths and reflection. Thus a definite leakage fraction needs the actual core and reflector arrangement; the usual increase is a qualitative tendency, not a geometric theorem for every redesign.

**The [Doppler coefficient of reactivity](../../physics.md#doppler-coefficient-of-reactivity) remains negative under the ordinary uranium-fuel assumptions.** Increasing fuel [temperature](../../temperature.md) broadens absorption resonances, increasing effective [uranium-238](../../chemical-substance.md#uranium-238) resonance capture and reducing [reactor reactivity](../../physics.md#reactivity-nuclear-engineering). This stabilizing fuel-temperature effect is distinct from moderator-density feedback.[Doppler coefficient entry: increased uranium-238 absorption as fuel temperature increases](../../engineering.md#reactor-glossary-by-the-united-states-nuclear-regulatory-commission) Greater importance of resonance absorption can make this feedback more important in a tighter lattice, but **its change in magnitude is not fixed by pitch alone**: spectrum, resonance self-shielding, fuel composition, burnup and the reference fuel [temperature](../../temperature.md) all enter the derivative.

**The fraction of fissions in [uranium-238](../../chemical-substance.md#uranium-238) tends to increase.** The harder neutron spectrum gives more opportunity for [fast fission](../../physics.md#fast-fission) before [neutrons](../../neutron.md) slow below the uranium-238 fission threshold. This concerns the fraction of the total [nuclear fission](../../physics.md#nuclear-fission) rate, not an assertion that the total thermal power increases; that power is held fixed.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Continue the same-rod-number and same-height comparison from part(a), and assume unchanged pump speed, similar inlet conditions and single-phase forced flow for the normal-operation hydraulic argument.

**[Core power density](../../engineering.md#core-power-density) increases.** The active core volume decreases while total thermal power stays fixed. The fuel's own average volumetric power and the mean [fuel linear heat rate](../../engineering.md#fuel-linear-heat-rate) do not increase merely from bringing the same rods closer together: fuel volume and rod count are unchanged.

**[Coolant](../../engineering.md#coolant) [mass flow rate](../../fluid-mechanics.md#mass-flow-rate) normally decreases.** Tighter passages reduce flow area and [hydraulic diameter](../../fluid-mechanics.md#hydraulic-diameter), increasing the core's hydraulic resistance. The unchanged [centrifugal pumps](../../fluid-mechanics.md#centrifugal-pump) do not enforce constant flow. The [pump operating point](../../fluid-mechanics.md#pump-operating-point) moves to the intersection of the same pump curve with the steeper system-resistance curve, normally giving smaller flow at greater pump head.[Module HT-03, pp.51–53, System Characteristic Curve and System Operating Point, Figure10](../../engineering.md#thermodynamics-heat-transfer-and-fluid-flow-volume-3-by-the-united-states-department-of-energy)

**The core [pressure](../../pressure.md) drop normally increases for the usual pump curve.** Its resistance at any given flow is higher. At the new, smaller flow, unchanged external piping and component losses are smaller, whereas a conventional falling pump head-versus-flow curve gives greater available head. The core takes the difference. This conclusion uses the stated pump-curve assumptions; holding flow fixed or holding pump head fixed would be different models. The exact new flow and pressure drop need both system and pump characteristics.

**Fuel [temperature](../../temperature.md) would normally tend to rise, especially downstream, if the loss of flow increases coolant heating without a compensating improvement in film heat transfer.** At fixed inlet state,

$$
P\simeq\dot m c_p(T_{\rm out}-T_{\rm in})
$$

shows that smaller total [mass flow rate](../../fluid-mechanics.md#mass-flow-rate) raises the bulk coolant temperature rise. At unchanged local [fuel linear heat rate](../../engineering.md#fuel-linear-heat-rate), the fuel-to-surface conductive contribution is approximately unchanged if material properties and gap conditions are held fixed. Its boundary [temperature](../../temperature.md) and the coolant film drop can nevertheless change.

The local [coolant mass flux](../../fluid-mechanics.md#coolant-mass-flux) is $G=\dot m/A_f$. Both total flow and flow area decrease, so the sign of the change in $G$, the [heat transfer coefficient](../../linear-ordinary-differential-equation.md#heat-transfer-coefficient) and the fuel [temperature](../../temperature.md) cannot be deduced from total flow alone. Changes in power peaking and inlet conditions add further qualifications to the usual hotter-fuel tendency.

**The [minimum departure from nucleate boiling ratio](../../critical-phenomenon.md#minimum-departure-from-nucleate-boiling-ratio) would commonly decrease, implying reduced boiling margin, but its sign is conditional.** The defining local ratio is

$$
\mathrm{DNBR}=\frac{q''_{\rm crit}}{q''_{\rm actual}},\qquad
\mathrm{MDNBR}=\min_{\rm core}\mathrm{DNBR}.
$$

The numerator is the [critical heat flux](../../critical-phenomenon.md#critical-heat-flux) for the local conditions, and the denominator is actual rod-surface [heat flux](../../heat.md#heat-flux-density).[Departure from nucleate boiling ratio entry](../../engineering.md#reactor-glossary-by-the-united-states-nuclear-regulatory-commission) The mean surface heat loading remains approximately unchanged for the same rods and total power. Greater coolant enthalpy rise tends to reduce margin, while changes in $G$, geometry, pressure and local power determine the actual critical heat flux. A geometry-appropriate correlation or experiment is needed for a definite MDNBR change; unchanged hardware does not supply it.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

**A tighter core is likely to have a more demanding cooling response, but the specification does not determine a unique peak cladding [temperature](../../temperature.md) or reflood time in a [loss-of-coolant accident](../../engineering.md#loss-of-coolant-accident).** Several effects compete.

At the same pre-accident power and comparable irradiation history, the total [decay heat](../../physics.md#decay-heat) source remains of broadly comparable scale; increasing [core power density](../../engineering.md#core-power-density) does not multiply the total decay power by the inverse change in core volume. The core nevertheless has less water within its tighter rod lattice. Its local thermal buffer is smaller, and the same heat must be removed through narrower passages. If the normal-operation fuel [temperature](../../temperature.md) is higher, more stored fuel thermal energy must also be removed after shutdown.

Reduced passage size and increased hydraulic resistance can impede emergency-coolant penetration and steam discharge during reflood. Local two-phase flow, entrainment and boiling heat transfer can change, so single-phase pump-curve reasoning is insufficient during blowdown and reflood. Less local water can favor earlier uncovering, but blowdown flow and the much larger inventory elsewhere in the unchanged primary circuit also matter. It would be unjustified to infer a proportionate reduction in the entire primary-circuit inventory.

Loss of water also removes [neutron moderation](../../neutron.md#neutron-moderation). In the assumed [under-moderated reactor](../../physics.md#under-moderated-reactor), this normally contributes negative [reactor reactivity](../../physics.md#reactivity-nuclear-engineering), helping suppress fission power. It does not eliminate [decay heat](../../physics.md#decay-heat) after shutdown. The thermal challenge must therefore be assessed separately from the sign of this feedback.

A quantitative comparison needs break characteristics, initial states, emergency injection performance, bypass paths and a transient two-phase calculation. The defensible conclusion is **potentially reduced thermal margin and more difficult reflood, requiring reassessment of the [emergency core cooling system](../../engineering.md#emergency-core-cooling-system)**, rather than an unconditional prediction that every large-break transient becomes worse in every metric.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

**The [conversion ratio](../../physics.md#conversion-ratio) usually tends to increase as moderation is reduced.** A harder spectrum gives greater importance to capture in fertile fuel, while less water can reduce some parasitic neutron absorption. These tendencies can increase replacement of fissile material during irradiation. Competing leakage, fast-fission and spectral effects mean the exact change is not fixed by the hydrogen-to-heavy-metal ratio alone.

**Higher conversion can support greater [discharge burnup](../../engineering.md#discharge-burnup) and a longer [nuclear fuel cycle length](../../engineering.md#nuclear-fuel-cycle-length), but neither follows automatically.** The improvement tends to slow the loss of useful fissile inventory during irradiation. The same change of lattice, however, lowers beginning-of-cycle [reactor reactivity](../../physics.md#reactivity-nuclear-engineering) under the usual under-moderated assumptions. With enrichment unchanged, the available initial reactivity margin may become inadequate before any later benefit from improved conversion can be realized.

Under the same-rod-number and same-height assumptions, the initial [heavy-metal mass of nuclear fuel](../../engineering.md#heavy-metal-mass-of-nuclear-fuel) $M_{\rm HM}$ and thermal power $P$ are unchanged. Thus the rate of accumulating energy-per-mass [burnup](../../engineering.md#nuclear-fuel-burnup) is unchanged:

$$
\frac{dB}{dt}=\frac{P}{M_{\rm HM}}.
$$

For a constant-power irradiation interval $t$, $B=Pt/M_{\rm HM}$. A longer achievable interval would consequently increase the burnup accumulated in that interval. This relation alone says nothing about whether that interval remains possible.

If sufficient initial [reactor reactivity](../../physics.md#reactivity-nuclear-engineering), shutdown capability and thermal margins are retained, slower depletion can allow increased discharge burnup and a longer cycle. If initial reactivity is too low, or the reduced boiling margin or fuel limits become controlling, either can instead decrease. [Discharge burnup](../../engineering.md#discharge-burnup) also depends on batch residence and refuelling strategy, so it is not generally identical to burnup accumulated in one operating cycle.

The appropriate qualitative answer is therefore **conversion tends upward; achievable discharge burnup and cycle length are conditional on the full reactivity history and operating limits**. An increased conversion ratio by itself does not determine a longer cycle.

## ↑ Ancestors (7)

1. [2020](../2020.md)
2. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
3. [MPhil in nuclear energy course of the University of Cambridge](../../university-of-cambridge.md#mphil-in-nuclear-energy-course-of-the-university-of-cambridge)
4. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
5. [University of Cambridge](../../university-of-cambridge.md)
6. [List of universities](../../README.md#list-of-universities)
7. [Codex Wiki](../../README.md)
