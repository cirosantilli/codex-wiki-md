<h1 id="clement-desormes-experiment">Clément-Desormes experiment</h1>

↑ **Parent:** [Heat capacity ratio](heat-capacity-ratio.md)

The Clément-Desormes experiment infers [heat capacity ratio](heat-capacity-ratio.md) from a rapid [pressure](pressure.md) reduction followed by reheating. Use a rigid bottle, pump or bellows, a quick release valve, and a U-tube [pressure](pressure.md) gauge connected to the bottle and atmosphere. First pump to a small excess [pressure](pressure.md), close the inlet, and wait for [thermal equilibrium](thermal-equilibrium.md) with the room at $T_0$. Measure $p_1>p_a$, where $p_a$ is local absolute atmospheric [pressure](pressure.md). Briefly open the release valve until the bottle reaches $p_a$, then close it promptly. The remaining [gas](gas.md) is cooler than the room. As it warms back to $T_0$ at fixed bottle [volume](volume-thermodynamics.md), its [pressure](pressure.md) rises to $p_3$, with $p_a<p_3<p_1$ in the ideal procedure. The rebound reveals cooling during release. [KIT Faculty of Physics, Clément-Desormes laboratory protocol: release and pressure rebound](https://labs.physik.kit.edu/prakt-nebenfach-manuals/Experiments/Adiabatenexponent_Luft/)

The bottle loses [molecules](molecule.md) while the valve is open: it is not a [closed system](closed-system.md) whose geometrical [volume](volume-thermodynamics.md) expands. In the well-mixed, negligible-[heat transfer](heat-transfer.md) discharge model with constant [heat capacity ratio](heat-capacity-ratio.md), the remaining [gas](gas.md) obeys $T_2/T_0=(p_a/p_1)^{(\gamma-1)/\gamma}$. Subsequent heating at fixed [amount of substance](amount-of-substance.md) and bottle [volume](volume-thermodynamics.md) gives $p_3/p_a=T_0/T_2$ by the [ideal gas law](ideal-gas-law.md). Eliminating the unmeasured $T_2$ yields

$$
\gamma=\frac{\ln(p_1/p_a)}{\ln(p_1/p_3)}
\simeq\frac{\Delta p_1}{\Delta p_1-\Delta p_3}
=\frac{h_1}{h_1-h_3},\qquad
\Delta p_i=p_i-p_a=\rho_{\rm liquid}gh_i.
$$

The [logarithms](logarithm.md) use absolute [pressure](pressure.md) ratios. The approximation requires small [gauge pressures](gauge-pressure.md) $\Delta p_i\ll p_a$; $h_i$ are signed height differences between the two liquid surfaces, and the final equality uses the same liquid in both readings with [hydrostatic equilibrium](hydrostatic-equilibrium.md). It is not an instruction to insert gauge readings into the logarithmic formula. For synthetic states generated with $p_a=100000\,\mathrm{Pa}$, $p_1=102000\,\mathrm{Pa}$ and $\gamma=1.4$, the model gives $p_3\simeq100567.39\,\mathrm{Pa}$. The logarithmic inference recovers $1.4$; the small-[pressure](pressure.md) approximation gives approximately $1.3961$.

Wait for a stable initial [pressure](pressure.md) after pumping and for a stable final [pressure](pressure.md) after closing. Vary the valve-open interval and initial excess [pressure](pressure.md) across repeated trials: closing too early leaves residual excess [pressure](pressure.md), while leaving the valve open during warming lets more [gas](gas.md) escape and suppresses the rebound. Test the seal for leaks, and read both liquid levels consistently. In a variant with incomplete release, measure the actual immediate post-release absolute [pressure](pressure.md) $p_2$ and replace the numerator by $\ln(p_1/p_2)$. The Zurich laboratory manual explains that liquid-column [oscillations](oscillation.md) can delay this reading until appreciable reheating has occurred; its proposed backward extrapolation assumes an exponential thermal relaxation and must be checked against the recorded readings. These controls separate a thermal signal from valve timing, instrumental lag and leakage. [University of Zurich, PHY112/122 laboratory manual, §1.3 and Appendix 1.4(a): pressure readings and reheating correction](https://www.physik.uzh.ch/~matthias/espace-assistant/manuals/en/anleitung-cd_e.pdf)

## ↑ Ancestors (7)

1. [Heat capacity ratio](heat-capacity-ratio.md)
2. [Ideal gas](ideal-gas.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Adiabatic process](adiabatic-process.md)
- [Heat capacity ratio](heat-capacity-ratio.md)
