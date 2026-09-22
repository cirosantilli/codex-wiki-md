# Atomic clock frequency lock

↑ **Parent:** [Atomic clock](atomic-clock.md)

A peak has zero slope at its center, so a single peak-height reading does not tell [feedback control](closed-loop-control.md) which way to tune. Instead sample the two sides at ordinary [frequencies](frequency.md) $\nu_c\pm d$, where $d>0$ is a chosen modulation offset, and subtract:

$$
E(\nu_c)=S(\nu_c+d)-S(\nu_c-d).
$$

For an even signal around the true center $\nu_0$, write $\epsilon=\nu_c-\nu_0$. A [Taylor expansion](taylor-expansion.md) gives $E(\nu_0+\epsilon)=2S'(\nu_0+d)\epsilon+O(\epsilon^3)$. On the descending side of a positive central peak $S'(\nu_0+d)<0$, so the update $\nu_c\mapsto\nu_c+gE$ has restoring sign for $g>0$ and is locally stable in this ideal discrete update when $0<-2gS'(\nu_0+d)<2$. A detector dip requires the opposite sign. These conditions follow from linearizing the update, not from assuming any particular electronics.

For the ideal signal $S=A\cos^2[\pi(\nu-\nu_0)T]+S_{\mathrm{bg}}$, choose $d=1/(4T)$. Then $E\simeq-2\pi AT\epsilon$. With $T=5\,\mathrm{ms}$ and $A=1$, a center error of $+1\,\mathrm{Hz}$ gives exact $E=-\sin(0.01\pi)\simeq-0.03141$. The sign directs the update toward lower [frequency](frequency.md). Constant background cancels, but background drift between samples or asymmetric neighboring [spectral lines](spectral-line.md) can bias the zero. An initial scan matters because other fringes can also supply zeros.

## ↑ Ancestors (9)

1. [Atomic clock](atomic-clock.md)
2. [Twin paradox clock experiments](twin-paradox-clock-experiments.md)
3. [Twin paradox](twin-paradox.md)
4. [Time dilation](time-dilation.md)
5. [Lorentz factor](lorentz-factor.md)
6. [Special relativity](special-relativity-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Atomic clock frequency shifts](atomic-clock-frequency-shifts.md)
- [Ramsey spectroscopy](ramsey-spectroscopy.md)
