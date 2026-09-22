# Deferred charge in CCD readout

↑ **Parent:** [Charge-coupled device](charge-coupled-device.md)

[Deferred charge in CCD readout](deferred-charge-in-ccd-readout.md) reaches later output samples than its originating packet. [George Elwood Smith](george-elwood-smith.md) describes [surface states](surface-state.md) at the [silicon](silicon.md)–[silicon dioxide](silicon-dioxide.md) interface capturing [electrons](electron.md) and releasing them later, smearing the image. A buried channel keeps the stored packet away from that interface.[pp. 2310–2311, Figs. 10–11, trapping](nobel-lecture-the-invention-and-early-history-of-the-ccd-by-george-elwood-smith.md)

An original comparison separates two interpretations of the same main-packet deficit. If a single transfer defers fraction $\epsilon$ by exactly one sample and loses nothing, an isolated input packet $N$ produces samples $\eta_{\rm tr}N$ followed by $\epsilon N$: summing both recovers $N$. A truly lossy transfer yields only $\eta_{\rm tr}N$, with no later recovery. For $N=10000$ and $\epsilon=0.01$, both give $9900$ in the intended sample, but only the deferred case gives a $100$-[electron](electron.md) trail. Such a trail redistributes position information even when total [electric charge](electric-charge-split.md) is conserved. Repeated delays require a time-response model; $N_{\rm in}\eta_{\rm tr}^n$ alone cannot predict trail shape. [Electron-hole recombination](electron-hole-recombination.md), escape to another contact, or release beyond the recorded window can instead remove signal from the measured sum.

## ↑ Ancestors (7)

1. [Charge-coupled device](charge-coupled-device.md)
2. [Photodetector](photodetector.md)
3. [Optical instrument](optical-instrument-split.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Deferred charge in CCD readout](deferred-charge-in-ccd-readout.md)
- [Early CCD charge-transfer experiment](early-ccd-charge-transfer-experiment.md)
