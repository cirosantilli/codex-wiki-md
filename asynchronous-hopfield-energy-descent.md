# Asynchronous Hopfield energy descent

↑ **Parent:** [Hopfield network](hopfield-network.md)

For symmetric zero-diagonal weights and zero thresholds, update one binary unit to the sign of its current field, retaining it at a zero field. The displayed energy change is negative on every actual flip. There are finitely many states, so a fair asynchronous update schedule eventually reaches a fixed point that is a minimum against single-unit flips. Synchronous updates can instead cycle, and local minima need not be global minima.

To obtain the displayed identity, subtract the two [energies](energy-split.md). Terms not involving $x_k$ cancel, and symmetry combines the two copies of each pair. With thresholds included the result is $\Delta E=-(x_k'-x_k)h_k$. The zero-threshold expression above is its specialization. At $h_k=0$, keeping the old state rules out motion along equal-[energy](energy-split.md) states. Finiteness then excludes infinitely many strict decreases, while fairness ensures that an unstable unit cannot be ignored forever. A [local minimum](local-minimum.md) here means no single flip lowers [energy](energy-split.md); equality directions can remain.

The asynchronous condition matters even for two units: with $w_{12}=w_{21}=1$ and zero thresholds, simultaneous updates alternate $(1,-1)$ and $(-1,1)$ forever. Either single-unit update instead reaches an aligned stable state.

## ↑ Ancestors (9)

1. [Hopfield network](hopfield-network.md)
2. [Neural network](neural-network.md)
3. [Statistical learning](statistical-learning-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Boltzmann machine](boltzmann-machine.md)
- [Hebbian memory weights for a Hopfield network](hebbian-memory-weights-for-a-hopfield-network.md)
- [Hopfield recall from a corrupted cue](hopfield-recall-from-a-corrupted-cue.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/3/e/solution.md)
