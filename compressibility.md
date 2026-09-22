# Compressibility

↑ **Parent:** [Thermodynamics](thermodynamics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compressibility)

Compressibility measures how readily a sample's [volume](volume-thermodynamics.md) decreases when its [pressure](pressure.md) increases. For a [simple compressible system](simple-compressible-system.md) with fixed particle number $N$ and composition, specify the constraint $X$:

$$
\kappa_X=-\frac1V\left(\frac{\partial V}{\partial P}\right)_{X,N},\qquad
\frac{dV}{V}=-\kappa_X\,dP\quad(X,N\text{ fixed}).
$$

Here $P$ denotes [pressure](pressure.md), also written $p$ elsewhere. The minus sign makes [compressibility](compressibility.md) positive on a mechanically stable equilibrium branch. Its units are inverse [pressure](pressure.md), $\mathrm{Pa^{-1}}$; its reciprocal $K_X=1/\kappa_X$ is the constrained [bulk modulus](bulk-modulus.md), measured in [pascal](pascal-unit.md) units. Holding [temperature](temperature.md) fixed gives [isothermal compressibility](isothermal-compressibility.md); holding [entropy](entropy.md) fixed gives [isentropic compressibility](isentropic-compressibility.md) $\kappa_S$ along an [isentropic process](isentropic-process.md). The latter describes a reversible [adiabatic compression](adiabatic-compression.md), since an irreversible [adiabatic process](adiabatic-process.md) can increase [entropy](entropy.md). [G. Ceder, MIT thermodynamics notes, section 1.14: compressibility](https://ocw.mit.edu/courses/3-20-materials-at-equilibrium-sma-5111-fall-2003/e402e3f0f555e15ff3af29b5b44b4e57_notes1.pdf)

For an [ideal gas](ideal-gas.md), the [ideal gas law](ideal-gas-law.md) $PV=Nk_BT$ and the [reversible ideal-gas adiabat](reversible-ideal-gas-adiabat.md) give, at the same equilibrium state,

$$
\kappa_T=\frac1P,\qquad
\kappa_S=\frac1{\gamma P},\qquad
\gamma=\frac{C_P}{C_V}>1.
$$

Here $C_P$ and $C_V$ are the whole sample's [heat capacity at constant pressure](heat-capacity-at-constant-pressure.md) and [heat capacity at constant volume](heat-capacity-at-constant-volume.md), and $\gamma$ is the [heat capacity ratio](heat-capacity-ratio.md). Constant $\gamma$ is required for the finite-path formula $PV^\gamma=\mathrm{constant}$. Reversible [adiabatic compression](adiabatic-compression.md) raises the [temperature](temperature.md), making the [pressure](pressure.md) rise more steeply than in an [isothermal compression](isothermal-compression.md). Thus keeping [entropy](entropy.md) fixed makes the [gas](gas.md) harder to compress locally. For a classical [monatomic gas](monatomic-gas.md) at $100\,\mathrm{kPa}$, $\gamma=5/3$, so $\kappa_T=10^{-5}\,\mathrm{Pa^{-1}}$ and $\kappa_S=6\times10^{-6}\,\mathrm{Pa^{-1}}$; the corresponding values of the [bulk modulus](bulk-modulus.md) are $100\,\mathrm{kPa}$ and $166.67\,\mathrm{kPa}$.

For a smooth, stable single [thermodynamic phase](thermodynamic-phase.md) at positive [temperature](temperature.md), [Maxwell relations](maxwell-relations.md) also imply

$$
\frac{\kappa_T}{\kappa_S}=\frac{C_P}{C_V},\qquad
\kappa_T-\kappa_S=\frac{TV\alpha^2}{C_P},
$$

where $\alpha$ is the [coefficient of thermal expansion](coefficient-of-thermal-expansion.md). The [ideal gas](ideal-gas.md) result is one example of this broader link between mechanical and thermal responses. The equality $\kappa_T=\kappa_S$ is possible when $\alpha=0$ and the other responses remain finite. These formulas compare equilibrium [partial derivatives](partial-derivative.md), rather than arbitrary fast or dissipative compression histories. [G. P. Beretta, MIT 2.43, Lecture 7: response-function identities](https://ocw.mit.edu/courses/2-43-advanced-thermodynamics-spring-2024/1Q7kBt43LW4oPrh3pxYjs2xxe7HWsC1oR_transcript.pdf)

**Table of contents**

- [Isothermal compressibility](isothermal-compressibility.md)
- [Isentropic compressibility](isentropic-compressibility.md)

## ↑ Ancestors (5)

1. [Thermodynamics](thermodynamics-split.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Compressibility](compressibility.md)
- [Dynamic pressure](dynamic-pressure.md)
- [Isentropic compressibility](isentropic-compressibility.md)
- [Isothermal compressibility](isothermal-compressibility.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-83/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-84/1/iii/solution.md)
