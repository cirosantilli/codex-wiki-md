# Optimum capture window in a background-dominated model

↑ **Parent:** [Delayed neutron-capture coincidence window](delayed-neutron-capture-coincidence-window.md)

If genuine pairs arrive at rate $S_0$ before the timing cut, an exposure $T$ gives $S=S_0T(1-e^{-W/\tau})$ and expected accidental pairs $B=R_pR_dWT$. In a background-dominated large-count approximation, maximizing $S/\sqrt B$ reduces to maximizing $f(x)=(1-e^{-x})/\sqrt x$ for $x=W/\tau>0$. Differentiation gives the positive stationary solution $e^x=1+2x$, or $x\simeq1.25643$. The endpoint $x=0$ solves the rearranged equation but is outside the domain of this derivative calculation; $f(x)$ tends to zero at both positive-domain extremes.

Thus the chosen $\tau=20\,\mu\mathrm s$ gives $W\simeq25.13\,\mu\mathrm s$ for this particular criterion, accepting about $0.715$ of genuine delayed signals. This differs from maximizing signal counts alone, which would favor longer windows. Small samples, appreciable signal fluctuations, unknown background, dead time and multiple-candidate vetoes require a fuller [likelihood](likelihood-function.md) model. The calculation isolates a tradeoff rather than prescribing an experimental cut.

## ↑ Ancestors (8)

1. [Delayed neutron-capture coincidence window](delayed-neutron-capture-coincidence-window.md)
2. [Cowan-Reines reactor antineutrino experiment](cowan-reines-reactor-antineutrino-experiment.md)
3. [Inverse beta decay](inverse-beta-decay.md)
4. [Beta decay](beta-decay.md)
5. [Radioactive decay](radioactive-decay.md)
6. [Nuclear physics](nuclear-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
