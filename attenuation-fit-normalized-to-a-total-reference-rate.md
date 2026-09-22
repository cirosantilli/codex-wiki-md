# Attenuation fit normalized to a total reference rate

↑ **Parent:** [Attenuation count model with an additive background](attenuation-count-model-with-an-additive-background.md)

If a measured unattenuated reference rate includes the same additive background as subsequent measurements, then $N_{\mathrm{ref}}=S_0+B$, where $S_0$ is signal alone. Substituting $S_0=N_{\mathrm{ref}}-B$ into an [attenuation count model with an additive background](attenuation-count-model-with-an-additive-background.md) gives $N(n)=(N_{\mathrm{ref}}-B)e^{-bn}+B$. This automatically returns the measured reference at $n=0$ and tends to $B$ at strong attenuation. Adding $B$ directly to $N_{\mathrm{ref}}e^{-bn}$ would count background twice at zero attenuation. A joint count likelihood can fit the reference and attenuated data with their separate exposure times, avoiding the need to regard the reference estimate as exact.

## ↑ Ancestors (6)

1. [Attenuation count model with an additive background](attenuation-count-model-with-an-additive-background.md)
2. [Exponential decay](exponential-decay.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-d/d12/e/solution.md)
