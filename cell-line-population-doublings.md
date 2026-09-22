# Cell line population doublings

↑ **Parent:** [Cell line](cell-line.md)

For positive recoverable counts $N_0,N_1$ bracketing one growth interval, define its net [cell line population doublings](cell-line-population-doublings.md) by

$$
d=\log_2\!\left(\frac{N_1}{N_0}\right)=\frac{\ln(N_1/N_0)}{\ln2}.
$$

The formula counts how many factors of two produce the observed net factor. For exactly two divisions per original [biological cell](biological-cell-split.md), with all daughters recovered, $N_1=2^2N_0$, giving $d=2$. Death or loss of [biological cells](biological-cell-split.md) makes this a net estimate of division.[Passage number and population doubling level, PDL equation and loss caveat](animal-cell-culture-guide-by-atcc.md)

Under constant-rate [exponential growth](exponential-growth.md), $N(t)=N_0e^{rt}$, a growth interval of duration $\Delta t$ gives

$$
r=\frac{\ln(N_1/N_0)}{\Delta t},\qquad t_2=\frac{\ln2}{r}=\frac{\Delta t}{d}.
$$

For the constructed fourfold increase over $48\,\mathrm{h}$, $d=2$ and the model [doubling time](doubling-time.md) is $24\,\mathrm{h}$. The proof follows by taking the [natural logarithm](natural-logarithm.md) and solving $e^{rt_2}=2$. This is a fitted property of that interval and model: it is not a universal [HeLa](hela.md) [doubling time](doubling-time.md), nor the interval between two divisions of each individual [biological cell](biological-cell-split.md). Across successive growth intervals, add their $d$ values; keep transfer losses separate as in [cell culture passage accounting](cell-culture-passage-accounting.md).

## ↑ Ancestors (4)

1. [Cell line](cell-line.md)
2. [Biological cell](biological-cell-split.md)
3. [Biology](biology-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Cell culture passage accounting](cell-culture-passage-accounting.md)
- [Cell line population doublings](cell-line-population-doublings.md)
- [Immortalised cell line](immortalised-cell-line.md)
