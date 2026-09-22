<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Computational models and biological experiments answer complementary questions. Experiments constrain what a nervous system actually does; a model makes a proposed explanation precise enough to test whether its mechanisms can produce those observations. **The useful comparison is between competing, experimentally constrained explanations, rather than between modelling and experimentation as alternatives.** A good model exposes assumptions, predicts new observations and identifies measurements that would distinguish it from rivals.

A [Hodgkin-Huxley model](../../../../../hodgkin-huxley-model.md) links [action potentials](../../../../../action-potential.md) to voltage-dependent conductances and channel kinetics. It is more informative than merely fitting a spike waveform because changes in its conductances predict changes in excitability. Yet a model calibrated for one cell or preparation does not automatically represent another: different channel combinations and spatial geometry can yield similar outputs. Detailed parameters must be constrained by experiments, and apparent agreement does not make them uniquely identifiable. A [leaky integrate-and-fire model](../../../../../leaky-integrate-and-fire-model.md) deliberately sacrifices channel detail to study the effects of connectivity, timing and [synapses](../../../../../synapse.md) in a large network. It is useful for such questions even though it cannot explain the microscopic origin of the action-potential waveform.

At a functional level, an [LNP model](../../../../../linear-nonlinear-poisson-cascade-model.md) tests which stimulus features predict a neuron's response and how those features map to firing rate. Independent testing, including response correlations rather than only mean rate, reveals what its assumptions miss. It can characterize a [receptive field](../../../../../receptive-field.md) without claiming that the brain explicitly performs its particular fitted calculation. A [Hopfield network](../../../../../hopfield-network.md) likewise demonstrates that recurrent interactions can implement content-addressable memory: corrupted cues relax toward stored patterns. Its usefulness is an existence proof and a quantitative account of interference, not evidence that biological memory literally uses symmetric binary connections and the same update schedule.

Developmental models connect observed input statistics with [synaptic plasticity](../../../../../synaptic-plasticity.md). [Hebbian learning](../../../../../hebbian-learning.md) with normalization or [synaptic competition](../../../../../synaptic-competition.md) can produce selective weights and segregation of competing inputs. Models of correlated ON and OFF inputs can explain the formation of oriented simple-cell subregions and predict how changing the correlations changes their organization. That makes altered visual experience or patterned stimulation informative tests. Such models still need anatomical, developmental and plasticity constraints; several learning rules may reproduce similar final receptive fields. [A primary model of activity-dependent ON/OFF competition](https://pmc.ncbi.nlm.nih.gov/articles/PMC6576834/) illustrates this approach.

Normative models instead ask what representation would perform a specified task efficiently. For example, [sparse coding](../../../../../sparse-coding.md) of natural images can produce localized oriented filters resembling [simple cell](../../../../../simple-cell.md) receptive fields. This links environmental statistics to a useful coding objective, but resemblance alone neither proves that the objective is the only explanation nor specifies the biological learning mechanism. Predictions about altered stimulus ensembles, population activity and synaptic changes provide stronger tests. [The original sparse-code receptive-field model](https://www.rctn.org/bruno/papers/sparse-coding.pdf) provides an example.

These distinctions also explain the dangers of models. Excessive flexibility can fit noise; unrealistic assumptions can generate a desired effect by construction; and multiple parameter sets can have nearly indistinguishable outputs. Simulation without analysis may obscure rather than explain a mechanism. [Cross-validation](../../../../../cross-validation.md), uncertainty analysis, comparisons with simpler models and controlled perturbations are therefore important. Conversely, collecting more measurements without a discriminating hypothesis can leave the same explanatory ambiguity unresolved.

The productive cycle is to propose a constrained model, determine which observations it predicts beyond the fitting data, perform the relevant experiment, and revise or reject the model. Models help select experiments and interpret results; experiments establish their scope and reveal omitted mechanisms. The appropriate level of detail depends on the question: spike-generation mechanisms, circuit computation and developmental organization need not be explained by the same model.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
