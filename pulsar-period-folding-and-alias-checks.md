# Pulsar period folding and alias checks

↑ **Parent:** [Pulsar](pulsar.md)

[Phase folding of a light curve](phase-folding-of-a-light-curve.md) collects samples at equal trial [phase](phase-waves.md). Consider a noiseless illustrative [pulsar](pulsar.md) with one pulse every $P=1.4\,\mathrm{s}$ and arrival times $t_n=nP$, after [pulsar dedispersion](pulsar-dedispersion.md). At $P_{\rm trial}=P$, all arrivals fold to one [phase](phase-waves.md). But $P/2$ also puts all arrivals at one [phase](phase-waves.md): folding discarded the fact that alternate proposed cycles contain no pulse. At $2P$, the arrivals instead occupy two [phases](phase-waves.md), $0$ and $1/2$. Thus a sharp folded profile alone need not identify the fundamental [period](period-of-a-function.md).

Check the original time sequence, adjacent arrival intervals and pulse occupancy as well as the folded profile. With $N$ arrivals and a slightly wrong trial [period](period-of-a-function.md), the unwrapped drift is

$$
\delta\phi_{N-1}=(N-1)\left(\frac{P}{P_{\rm trial}}-1\right).
$$

For $N=100$ and $P_{\rm trial}=1.401\,\mathrm{s}$, this is about $-0.07066$ cycle. Splitting the observation into early and late pieces reveals the drift that one full folded average can blur. Separately, regular discrete sampling can create [aliasing](aliasing.md): observing at a spacing comparable with the pulse width can miss narrow pulses even when the recurrence [period](period-of-a-function.md) is much longer. Neither this toy exercise nor one sharp profile replaces time-standard calibration and propagation corrections.

## ↑ Ancestors (8)

1. [Pulsar](pulsar.md)
2. [Neutron star](neutron-star.md)
3. [Stellar evolution](stellar-evolution.md)
4. [Stellar astrophysics](stellar-astrophysics-split.md)
5. [Astrophysics](astrophysics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
