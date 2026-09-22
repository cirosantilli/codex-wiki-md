# Synapse

↑ **Parent:** [Neuron](neuron.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Synapse)

A [synapse](synapse.md) is a signaling junction between a [neuron](neuron.md) and another [biological cell](biological-cell-split.md). The sending side is presynaptic and the receiving side postsynaptic. At a [chemical synapse](chemical-synapse.md), released [neurotransmitter](neurotransmitter.md) acts on a [receptor](receptor-biochemistry.md) in the receiving [cell membrane](cell-membrane-split.md). At an [electrical synapse](electrical-synapse.md), [gap junctions](gap-junction.md) provide a direct path for [electric current](electric-current.md) between cells. See [1.1 Elements of Neuronal Systems](neuronal-dynamics-from-single-neurons-to-networks-and-models-of-cognition-by-wulfram-gerstner-and-others/1-1-elements-of-neuronal-systems.md).

In a common sequence at a [chemical synapse](chemical-synapse.md), an arriving [action potential](action-potential.md) opens [voltage-gated ion channels](voltage-gated-ion-channel.md) selective for [calcium](calcium.md). [Calcium](calcium.md) entry triggers fusion of [synaptic vesicles](synaptic-vesicle.md) with the presynaptic [cell membrane](cell-membrane-split.md), releasing [neurotransmitter](neurotransmitter.md) into the [synaptic cleft](synaptic-cleft.md). Binding to a [receptor](receptor-biochemistry.md) changes postsynaptic [electrical resistance and conductance](electrical-resistance-and-conductance.md), directly through an [ion channel](ion-channel.md) or through an intracellular signaling pathway. The resulting change in [membrane potential](membrane-potential-split.md) is a [synaptic potential](synaptic-potential.md). See [Ion Channels and the Electrical Properties of Membranes](molecular-biology-of-the-cell-4th-edition-by-bruce-alberts-and-others/ion-channels-and-the-electrical-properties-of-membranes.md).

A useful conductance approximation writes the inward-positive synaptic [electric current](electric-current.md) as

$$
I_{\mathrm{syn}}=g_{\mathrm{syn}}(t)(E_{\mathrm{syn}}-V),
$$

where $g_{\mathrm{syn}}\geq0$ describes the activated [electrical resistance and conductance](electrical-resistance-and-conductance.md), $V$ is the postsynaptic [membrane potential](membrane-potential-split.md), and $E_{\mathrm{syn}}$ is the [reversal potential](reversal-potential.md), the voltage at which this current vanishes. Opening these channels tends to pull $V$ toward $E_{\mathrm{syn}}$; it does not prescribe a current of fixed sign independently of $V$.

For a worked example, let $V=-65\,\mathrm{mV}$ and $g_{\mathrm{syn}}=1\,\mathrm{nS}$. A [reversal potential](reversal-potential.md) of $0\,\mathrm{mV}$ gives $I_{\mathrm{syn}}=65\,\mathrm{pA}$, an inward [electric current](electric-current.md) that raises [membrane potential](membrane-potential-split.md). A [reversal potential](reversal-potential.md) of $-75\,\mathrm{mV}$ instead gives $-10\,\mathrm{pA}$, which lowers [membrane potential](membrane-potential-split.md). These are illustrative calculations, not measurements. A [reversal potential](reversal-potential.md) of $-60\,\mathrm{mV}$ can raise $V$ from $-65\,\mathrm{mV}$ yet oppose reaching a threshold of $-50\,\mathrm{mV}$: a depolarizing input need not be excitatory.

An excitatory [synapse](synapse.md) favors a subsequent [action potential](action-potential.md), whereas an inhibitory [synapse](synapse.md) opposes it. The effect depends on the [receptor](receptor-biochemistry.md), the permeating [ions](ion.md), their gradients and the [reversal potential](reversal-potential.md); a [neurotransmitter](neurotransmitter.md) does not have one fixed excitatory or inhibitory sign in every context. Even with $E_{\mathrm{syn}}=V$, an added conductance can reduce responses to other inputs by lowering effective [electrical resistance](electrical-resistance.md), an effect called [shunting inhibition](shunting-inhibition.md). See [Purves and colleagues: excitatory and inhibitory postsynaptic potentials](https://www.ncbi.nlm.nih.gov/books/NBK11117/). This dependence matters when translating a biological [synapse](synapse.md) into a signed weight or an imposed [electric current](electric-current.md) in [computational neuroscience](computational-neuroscience.md).

**Table of contents**

- [Synaptic plasticity](synaptic-plasticity.md)
  - [Synaptic competition](synaptic-competition.md)
    - [Synaptic normalization](synaptic-normalization.md)
- [Neurotransmitter](neurotransmitter.md)
  - [Acetylcholine](acetylcholine.md)
- [Chemical synapse](chemical-synapse.md)
  - [Neurotransmitter clearance](neurotransmitter-clearance.md)
  - [Synaptic cleft](synaptic-cleft.md)
  - [Synaptic vesicle](synaptic-vesicle.md)
    - [Quantal neurotransmitter release](quantal-neurotransmitter-release.md)
      - [Synaptic release probability](synaptic-release-probability.md)
  - [Shunting inhibition](shunting-inhibition.md)
- [Electrical synapse](electrical-synapse.md)
- [Synaptic potential](synaptic-potential.md)
  - [Synaptic conductance](synaptic-conductance.md)
  - [Excitatory postsynaptic potential](excitatory-postsynaptic-potential.md)
  - [Inhibitory postsynaptic potential](inhibitory-postsynaptic-potential.md)

## ↑ Ancestors (4)

1. [Neuron](neuron.md)
2. [Neuroscience](neuroscience-split.md)
3. [Biology](biology-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (20)

- [Axon](axon.md)
- [Chemical synapse](chemical-synapse.md)
- [Extracellular single-unit recording](extracellular-single-unit-recording.md)
- [Leaky integrate-and-fire model](leaky-integrate-and-fire-model.md)
- [Neuron](neuron.md)
- [Neuronal paired-pulse recovery](neuronal-paired-pulse-recovery.md)
- [ON and OFF receptive-field subregions](on-and-off-receptive-field-subregions.md)
- [Solution](past-exam-of-the-biochemistry-course-of-the-university-of-cambridge/2025/paper-2/section-ii/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/2/solution.md)
- [Signed spatial filter model of a simple cell](signed-spatial-filter-model-of-a-simple-cell.md)
- [Simple cell](simple-cell.md)
- [Spatial summation](spatial-summation.md)
- [Synapse](synapse.md)
- [Synaptic conductance](synaptic-conductance.md)
- [Synaptic integration](synaptic-integration.md)
- [Synaptic potential](synaptic-potential.md)
- [Temporal summation](temporal-summation.md)
