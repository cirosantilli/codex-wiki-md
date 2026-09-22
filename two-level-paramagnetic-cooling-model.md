# Two-level paramagnetic cooling model

↑ **Parent:** [Magnetic entropy](magnetic-entropy.md)

Use the [independent spin-one-half two-level system](independent-spin-one-half-two-level-system.md) with fixed $N$ distinguishable sites and [Hamiltonian](hamiltonian.md) levels $E_\pm=\pm\mu B$, where $\mu>0$ is the magnitude of the field-axis [magnetic moment](magnetic-dipole-moment.md) and $B>0$ is a uniform externally controlled [magnetic field](magnetic-field-split.md). Assume positive [temperature](temperature-split.md), no interactions between sites, and no appreciable lattice or load [entropy](entropy-split.md). The two levels differ by $2\mu B$. With [inverse temperature](inverse-temperature.md) $\beta$, the [canonical ensemble](canonical-ensemble-split.md) gives the one-site and total [partition functions](canonical-partition-function.md)

$$
\beta=\frac1{k_BT},\qquad x=\beta\mu B,\qquad
z=e^x+e^{-x}=2\cosh x,\qquad Z=z^N,
\qquad p_-=\frac{e^x}{2\cosh x},\quad p_+=\frac{e^{-x}}{2\cosh x}.
$$

Here the minus subscript denotes the lower [energy](energy-split.md) $-\mu B$. Factorization of the [partition function](canonical-partition-function.md) requires additive [energy](energy-split.md) and independent sites; there is no particle-exchange factor $N!$ for these fixed distinguishable sites.

Differentiate the [partition function](canonical-partition-function.md), holding $B$ fixed when differentiating with respect to $\beta$. The [internal energy](internal-energy-split.md), [Helmholtz free energy](helmholtz-free-energy.md), total field-axis [magnetic moment](magnetic-dipole-moment.md) $m$, and [magnetic entropy](magnetic-entropy.md) are

$$
U_{\rm mag}=-\partial_\beta\ln Z=-N\mu B\tanh x,\qquad
F=-Nk_BT\ln(2\cosh x),
$$



$$
m=-\left(\frac{\partial F}{\partial B}\right)_T=N\mu\tanh x,\qquad
\frac{S_{\rm mag}}{Nk_B}=\frac{\ln Z+\beta U_{\rm mag}}N
=\ln(2\cosh x)-x\tanh x=:s(x).
$$

The extensive moment $m$ is distinct from [magnetization](magnetization.md), the moment per unit [volume](volume-thermodynamics.md). Direct substitution of $p_\pm$ into the [Gibbs entropy](gibbs-entropy.md) gives the same $s(x)$ independently of the free-energy [derivative](derivative.md).

At fixed $B$, the magnetic [heat capacity](heat-capacity.md) is

$$
C_{B,{\rm mag}}=\left(\frac{\partial U_{\rm mag}}{\partial T}\right)_B
=Nk_Bx^2\operatorname{sech}^2x\geq0,\qquad
\frac{ds}{dx}=-x\operatorname{sech}^2x<0\quad(x>0).
$$

Strict decrease makes $s$ invertible on $x>0$. Constant [magnetic entropy](magnetic-entropy.md) therefore fixes $x$, not $B$ or $T$ separately:

$$
\frac{B}{T}=\text{constant},\qquad
\frac{T_f}{T_i}=\frac{B_f}{B_i}\quad(B_i,B_f,T_i,T_f>0).
$$

The [partition function](canonical-partition-function.md) may be used to label these equilibrium states even though the isolated cooling leg has no external [heat bath](heat-bath.md). Actual thermalization of the lattice and load additionally requires a sufficiently fast [spin-lattice relaxation](spin-lattice-relaxation.md); perfectly uncoupled spins by themselves cannot refrigerate an attached object.

The limiting cases are instructive. For $x\ll1$, $s(x)=\ln2-x^2/2+O(x^4)$, $m\simeq N\mu^2B/(k_BT)$, and $C_{B,{\rm mag}}\simeq Nk_Bx^2$. The moment response reproduces [Curie's law](curie-s-law.md). For $x\gg1$, $s(x)\simeq(1+2x)e^{-2x}$ and the upper-state occupation is exponentially small. Taking $B\to0$ at fixed $T>0$ gives $s\to\ln2$; taking $T\to0$ at fixed $B>0$ gives $s\to0$. The origin has a path-dependent limit. Extrapolating a line of constant $x$ to $B=T=0$ does not construct a usable zero-[temperature](temperature-split.md) state or prove that a real material retains independent degenerate spins there.

**Table of contents**

- [Constant-entropy magnetic cooling example](constant-entropy-magnetic-cooling-example.md)

## ↑ Ancestors (8)

1. [Magnetic entropy](magnetic-entropy.md)
2. [Adiabatic demagnetization](adiabatic-demagnetization.md)
3. [Temperature](temperature-split.md)
4. [Thermodynamics](thermodynamics-split.md)
5. [Statistical physics](statistical-physics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Giauque-MacDougall magnetic cooling experiment](giauque-macdougall-magnetic-cooling-experiment.md)
