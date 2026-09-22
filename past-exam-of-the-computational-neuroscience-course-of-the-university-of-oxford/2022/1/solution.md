<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**A two-layer [heteroassociative memory](../../../heteroassociative-memory.md) can retrieve one activity pattern from a different associated cue through learned feedforward [synapses](../../../synapse.md).** Let $x^\mu\in\mathbb R^n$ represent a cue and $t^\mu\in\mathbb R^m$ its associate. An input population projects to an output population through $W$, with retrieval $y=\phi(Wx-\theta)$. The output [activation function](../../../activation-function.md) can be linear for an analysis or thresholded with [synaptic competition](../../../synaptic-competition.md) for a sparse categorical response. This is [pattern association](../../../heteroassociative-memory.md): the output need not reproduce the input, unlike an [autoassociative memory](../../../autoassociative-memory.md).

During storage, the cue and its desired associate must be coactive. A local [Hebbian learning](../../../hebbian-learning.md) rule, $\Delta W_{ij}=\eta t_i x_j$, strengthens the connection from an active cue [neuron](../../../neuron-split.md) to an active target [neuron](../../../neuron-split.md). With normalized inputs, the idealized batch weights are

$$
W=\sum_{\mu=1}^{P}t^\mu(x^\mu)^{\mathsf T}.
$$

Presenting cue $x^\nu$ gives

$$
Wx^\nu=t^\nu\|x^\nu\|^2+\sum_{\mu\ne\nu}t^\mu\bigl((x^\mu)^{\mathsf T}x^\nu\bigr).
$$

The first term is the desired association; the second is interference from overlapping cues. Thus retrieval follows exactly for orthonormal cue patterns, while [sparse coding](../../../sparse-coding.md), centring, [synaptic normalization](../../../synaptic-normalization.md) and a competitive output can reduce interference for realistic overlapping inputs. These devices have distinct roles: [synaptic normalization](../../../synaptic-normalization.md) prevents unlimited weight growth, and [synaptic competition](../../../synaptic-competition.md) separates competing associates. Signed, centred model weights should not be identified literally with negative excitatory [synapses](../../../synapse.md); biological inhibition and baseline subtraction need an explicit circuit implementation.

As an exact illustrative calculation, take $x^1=(1,0)^{\mathsf T}$, $x^2=(0,1)^{\mathsf T}$, $t^1=(1,1,0)^{\mathsf T}$ and $t^2=(0,0,1)^{\mathsf T}$. Then

$$
W=\begin{pmatrix}1&0\\1&0\\0&1\end{pmatrix},\qquad Wx^1=t^1,\qquad Wx^2=t^2.
$$

A cue $(0.8,0.1)^{\mathsf T}$ produces $(0.8,0.8,0.1)^{\mathsf T}$, so threshold $0.5$ retrieves the first associate. These are chosen model values, not recorded firing rates. If two genuinely different associates share an identical cue, a deterministic feedforward map cannot choose between them without additional context; adding capacity alone does not solve that ambiguity. A cue-to-associate map also need not provide the reverse association unless the reverse pathway is separately learned.

The [hippocampus](../../../hippocampus.md) provides a plausible anatomical setting. In a [hippocampal episodic memory model](../../../hippocampal-episodic-memory-model.md), a retrieved [hippocampal CA3](../../../hippocampal-ca3.md) event pattern can project through the [hippocampal CA1](../../../hippocampal-ca1.md) output pathway to reinstate associated cortical content. The feedforward CA3-to-CA1 and hippocampal-to-cortical links can provide [heteroassociation](../../../heteroassociative-memory.md), while recurrent [CA3](../../../hippocampal-ca3.md) connectivity provides [autoassociation](../../../autoassociative-memory.md). The [entorhinal cortex](../../../entorhinal-cortex.md) supplies converging information and routes cortical communication. This is a computational assignment to pathways; anatomical connectivity alone does not prove that their weights implement the displayed rule.

An especially direct physiological test comes from trained visual pairs. Monkeys learned arbitrary associations between computer-generated pictures and then selected the associated picture after a delay. [Extracellular single-unit recording](../../../extracellular-single-unit-recording.md) in anterior temporal cortex found both [neurons](../../../neuron-split.md) responding to the two members of a learned pair and [neurons](../../../neuron-split.md) whose delay activity anticipated the appropriate associate. The preparation therefore links an experimentally controlled cue–associate relation to neural responses, rather than merely showing visual selectivity. However, the recordings do not identify the individual modified [synapses](../../../synapse.md), establish one-way connectivity, or exclude recurrent retrieval. They support an associative representation in temporal cortex, not a unique proof of a two-layer implementation.[Abstract; pp. 152–155, pair-association task and cue/delay responses](../../../neural-organization-for-the-long-term-memory-of-paired-associates-by-kuniyoshi-sakai-and-others.md)

The rapid-learning requirement is relevant to the [hippocampal](../../../hippocampus.md) implementation: CA3-restricted [NMDA receptor](../../../nmda-receptor.md) deletion impaired learning of a newly located hidden platform in a delayed matching-to-place task while sparing performance with previously experienced locations. This supports rapid [hippocampal](../../../hippocampus.md) storage, but does not by itself identify a specific feedforward association matrix.[Abstract; pp. 305–315, delayed matching-to-place and novel versus familiar platform locations](../../../hippocampal-ca3-nmda-receptors-are-crucial-for-memory-acquisition-of-one-time-experience-by-kazu-nakazawa-and-others.md)

A decisive model test would measure cue and associate representations before learning, after learning, and during partial-cue retrieval, while selectively disrupting the proposed connecting pathway. Correct associate decoding with unrelated-cue and familiar-visual-response controls would be stronger evidence than activity during successful recall alone. **The architecture is a plausible component of temporal and [hippocampal](../../../hippocampus.md) memory circuits; its local learning rule, interference properties and pathway-specific causal predictions make it testable.**

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2022](../../2022-split.md)
3. [Past exam of the computational neuroscience course of the University of Oxford](../../split.md)
4. [Computational neuroscience course of the University of Oxford](../../../computational-neuroscience-course-of-the-university-of-oxford.md)
5. [Year 3 of the psychology (experimental) course of the University of Oxford](../../../year-3-of-the-psychology-experimental-course-of-the-university-of-oxford.md)
6. [Psychology (experimental) course of the University of Oxford](../../../psychology-experimental-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
