# Fine-grained Gibbs entropy

↑ **Parent:** [Gibbs entropy](gibbs-entropy.md)

For a normalized [probability density](probability-density.md) $\rho$ on classical [phase space](phase-space.md) with canonical volume element $d\Gamma$, the fine-grained [Gibbs entropy](gibbs-entropy.md) is $-k_B\int\rho\log(\rho/\rho_{\rm ref})\,d\Gamma$, whenever the integral exists. Here $\rho_{\rm ref}>0$ is a constant reference density fixing the units inside the [logarithm](logarithm.md), and $k_B$ is the [Boltzmann constant](boltzmann-constant.md). No averaging into finite cells is performed.

For a regular [Hamiltonian flow](hamiltonian-flow.md) $\Phi_t$, [Liouville theorem in Hamiltonian mechanics](liouville-s-theorem-hamiltonian.md) gives $d\Gamma(\Phi_tz)=d\Gamma(z)$ and $\rho_t(\Phi_tz)=\rho_0(z)$. Substitution directly proves

$$
S_{\rm fg}[\rho_t]=-k_B\int\rho_0(z)\log(\rho_0(z)/\rho_{\rm ref})\,d\Gamma(z)=S_{\rm fg}[\rho_0].
$$

An irreversible macroscopic entropy increase therefore requires a different description or additional assumptions; it is not a failure of this volume-preservation argument.

## ↑ Ancestors (5)

1. [Gibbs entropy](gibbs-entropy.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
