# Knudsen number

↑ **Parent:** [Kinetic theory](kinetic-theory.md)

The [Knudsen number](knudsen-number.md) is the [dimensionless](dimensionless-quantity.md) ratio of an intermolecular [mean free path](mean-free-path.md) $\ell_{\mathrm{mfp}}$ to a specified characteristic length $L$ of the apparatus or flow. The [mean free path](mean-free-path.md) measures the distance travelled between gas–gas [collisions](collision.md); $L$ measures the distance over which boundaries or macroscopic conditions matter. Wall encounters must not be counted as gas–gas [collisions](collision.md) in this comparison: doing so would hide the very wall-dominated behavior we want to detect. The same gas can therefore have a small [Knudsen number](knudsen-number.md) in a large vessel and a large [Knudsen number](knudsen-number.md) in a tiny opening.

For a dilute [hard-sphere gas](hard-sphere-gas.md) of identical molecular diameter $d$ in [thermal equilibrium](thermal-equilibrium.md), use the convention

$$
\ell_{\mathrm{mfp}}=\frac{1}{\sqrt2\,n\pi d^2}=\frac{k_BT}{\sqrt2\,\pi d^2p},\qquad \mathrm{Kn}=\frac{k_BT}{\sqrt2\,\pi d^2pL}.
$$

Here $n$ is the [number density](number-density.md), $p$ the [pressure](pressure.md), $T$ the absolute [temperature](temperature.md), and $k_B$ the [Boltzmann constant](boltzmann-constant.md); the second equality uses the [ideal gas law](ideal-gas-law.md). The [collision cross-section](collision-cross-section.md) is $\pi d^2$, and the $\sqrt2$ accounts for both partners moving with independent equilibrium [velocities](velocity.md). Mixtures and velocity-dependent [collision cross-sections](collision-cross-section.md) require a stated molecular model and [mean free path](mean-free-path.md) convention; the displayed expression is not an exact formula for every real gas. [Fitzpatrick, Mean Free Path, equations 5.209–5.219](https://farside.ph.utexas.edu/teaching/355/Surveyhtml/node219.html) [Steve T. Paik, Is the mean free path the mean of a distribution?, dilute hard-sphere equilibrium convention](https://arxiv.org/abs/1309.1197)

As a numerical toy example, choose $T=300\,\mathrm K$ and $d=0.37\,\mathrm{nm}$, without claiming that this is a measured molecular diameter for a particular gas. The formula gives $\ell_{\mathrm{mfp}}\simeq68.1\,\mathrm{nm}$ at $p=10^5\,\mathrm{Pa}$. It yields $\mathrm{Kn}\simeq6.81\times10^{-6}$ for a $1\,\mathrm{cm}$ vessel but $\mathrm{Kn}\simeq0.681$ for a $100\,\mathrm{nm}$ gap. At $p=1\,\mathrm{Pa}$ the same toy gas has $\ell_{\mathrm{mfp}}\simeq6.81\,\mathrm{mm}$, comparable to the centimetre vessel. Reducing either [pressure](pressure.md) or apparatus size can thus expose molecular transport.

Choose $L$ for the question being asked: a tube diameter compares the [mean free path](mean-free-path.md) with wall separation, while tube length describes a different geometric scale. For a positive macroscopic field $q$, a local gradient scale can instead be $L_q=|q|/|\nabla q|$, where its [gradient](gradient.md) is nonzero. A large vessel can contain a thin region with a large local [Knudsen number](knudsen-number.md). Small geometric [Knudsen number](knudsen-number.md) alone does not guarantee a slowly varying near-equilibrium flow. The time, [velocity](velocity.md) and space scalings must also be stated when the [Knudsen number](knudsen-number.md) appears as a coefficient in a [Boltzmann equation](boltzmann-equation.md). [NASA, Comparison Between DSMC and CFD for Hypersonic Planetary Entry Simulations (2023), local gradient-length breakdown analysis](https://ntrs.nasa.gov/citations/20230013741)

<a id="image-mean-free-path-versus-apparatus-scale-with-a-fixed-rate-single-flight-toy-model"></a>
![](knudsen-scale-and-flight-survival.png)

**[Figure 7](#image-mean-free-path-versus-apparatus-scale-with-a-fixed-rate-single-flight-toy-model). Mean free path versus apparatus scale, with a fixed-rate single-flight toy model**. The three chosen ratios are examples, not regime boundaries. The curve assumes a constant collision hazard per distance and plots $\exp(-L/\ell_{\mathrm{mfp}})$; it is neither measured gas data nor the full free-path distribution of an equilibrium hard-sphere gas.

**Table of contents**

- [Rarefied gas flow approximations](rarefied-gas-flow-approximations.md)
  - [Knudsen layer](knudsen-layer.md)
  - [Free molecular flow](free-molecular-flow.md)

## ↑ Ancestors (5)

1. [Kinetic theory](kinetic-theory.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Hydrodynamic limit of the Boltzmann equation](hydrodynamic-limit-of-the-boltzmann-equation.md)
- [Kinetic theory](kinetic-theory.md)
- [Knudsen number](knudsen-number.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7/4/solution.md)
- [Rarefied gas flow approximations](rarefied-gas-flow-approximations.md)
- [Thermal transpiration](thermal-transpiration.md)
- [Thermal transpiration experiment with a glass microtube](thermal-transpiration-experiment-with-a-glass-microtube.md)
