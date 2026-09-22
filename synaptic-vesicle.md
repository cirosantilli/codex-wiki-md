# Synaptic vesicle

↑ **Parent:** [Chemical synapse](chemical-synapse.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Synaptic_vesicle)

A [synaptic vesicle](synaptic-vesicle.md) is a small membrane-bounded compartment in a presynaptic terminal that stores [neurotransmitter](neurotransmitter.md) for release. Fusion with the [cell membrane](cell-membrane-split.md) exposes its contents to the [synaptic cleft](synaptic-cleft.md); the packet supplied by one [synaptic vesicle](synaptic-vesicle.md) is a quantum of release. [Quantal neurotransmitter release](quantal-neurotransmitter-release.md) refers to these discrete packets, rather than the release of one [molecule](molecule-split.md) at a time. The postsynaptic response to a packet can vary with its contents, [receptors](receptor-biochemistry.md) and recording conditions. See [Purves and colleagues: vesicles as the source of transmitter quanta](https://www.ncbi.nlm.nih.gov/books/NBK10866/).

The useful cycle is filling, preparation for fusion, [calcium](calcium.md)-triggered [exocytosis](exocytosis.md), and recovery of membrane and [proteins](protein-split.md) through [endocytosis](endocytosis.md) for reuse. Different recovery routes occur; recycling need not preserve a particular [synaptic vesicle](synaptic-vesicle.md) as an identifiable container throughout. Limited availability of prepared [synaptic vesicles](synaptic-vesicle.md) can reduce release during repeated stimulation, while changes in [synaptic release probability](synaptic-release-probability.md) can also change successive responses. See [Basic Neurochemistry: secretion machinery and vesicle reuse](https://www.ncbi.nlm.nih.gov/books/NBK27911/) and [3.1 Synapses](neuronal-dynamics-from-single-neurons-to-networks-and-models-of-cognition-by-wulfram-gerstner-and-others/3-1-synapses.md).

For an illustrative calculation, assume four release sites, each with one prepared [synaptic vesicle](synaptic-vesicle.md), each releasing with [synaptic release probability](synaptic-release-probability.md) $p=0.25$ during one presynaptic [action potential](action-potential.md). Assume [independent](independent-random-variables.md) [Bernoulli trials](bernoulli-trial.md) and at most one release per site. The released packet count $K$ has a [binomial distribution](binomial-distribution.md):

$$
K\sim\operatorname{Bin}(4,0.25),\qquad \mathbb E[K]=4(0.25)=1,\qquad \operatorname{Var}(K)=4(0.25)(0.75)=0.75.
$$

The [probability](probability.md) of no release is $\mathbb P(K=0)=0.75^4=0.31640625$; at least one release has [probability](probability.md) $0.68359375$. An [expected value](expected-value-split.md) of one packet does not mean that every [action potential](action-potential.md) releases one packet. If each packet contributes a stipulated $0.5\,\mathrm{nS}$ conductance increment and increments add, the [expected value](expected-value-split.md) of that increment is $0.5\,\mathrm{nS}$, with zero increment on about $31.6\%$ of trials. These assumptions are a teaching model: shared [calcium](calcium.md) fluctuations, unequal sites, depletion and nonlinear [receptor](receptor-biochemistry.md) responses can invalidate them.

**Table of contents**

- [Quantal neurotransmitter release](quantal-neurotransmitter-release.md)
  - [Synaptic release probability](synaptic-release-probability.md)

## ↑ Ancestors (6)

1. [Chemical synapse](chemical-synapse.md)
2. [Synapse](synapse.md)
3. [Neuron](neuron.md)
4. [Neuroscience](neuroscience-split.md)
5. [Biology](biology-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Chemical synapse](chemical-synapse.md)
- [Electrical synapse](electrical-synapse.md)
- [Endocytosis](endocytosis.md)
- [Exocytosis](exocytosis.md)
- [Neuron](neuron.md)
- [Quantal neurotransmitter release](quantal-neurotransmitter-release.md)
- [Synapse](synapse.md)
- [Synaptic release probability](synaptic-release-probability.md)
- [Synaptic vesicle](synaptic-vesicle.md)
