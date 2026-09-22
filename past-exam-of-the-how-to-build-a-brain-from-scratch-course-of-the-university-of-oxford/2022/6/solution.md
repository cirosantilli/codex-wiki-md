<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

**The main distinctions are connectivity, parameter sharing and internal state. A [convolutional neural network](../../../convolutional-neural-network.md) can itself be feedforward, and [convolution](../../../convolution.md) can also be used inside a [recurrent neural network](../../../recurrent-neural-network.md); these categories are not mutually exclusive.** Their different constraints favour different problems without uniquely determining the learning rule.

A [feedforward neural network](../../../feedforward-neural-network.md) passes activity through a directed acyclic sequence of layers,

$$
h^{(0)}=x,\qquad h^{(\ell+1)}=\phi_\ell(W_\ell h^{(\ell)}+b_\ell).
$$

An input produces an output without a persistent state feeding back into the computation. A dense [multilayer perceptron](../../../multilayer-perceptron.md) can learn classification, regression or a cue-to-associate mapping when the supplied input contains the needed information. Nonlinear [activation functions](../../../activation-function.md) matter: composing only affine layers gives another [affine map](../../../affine-map.md), so adding such layers would not create the same representational benefit. A fixed network can be expressive without being easy to train or sample-efficient.

Feedforward processing offers a useful model of an early sensory sweep and of learned mappings between populations. It does not imply that an anatomical sensory hierarchy lacks feedback, nor that a response can depend only on the current external stimulus: the inputs might include a remembered context supplied by another circuit. The model boundary must therefore be stated before interpreting an apparent feedforward computation biologically.

A [convolutional neural network](../../../convolutional-neural-network.md) introduces spatial locality and [weight sharing](../../../weight-sharing.md). For a stride-one layer on an appropriate grid,

$$
h_o(p)=\phi\!\left(b_o+\sum_{c,r}K_{o,c}(r)x_c(p-r)\right).
$$

The same filter $K$ is applied at many positions. This reduces parameters and encodes a prior that a useful local feature can recur elsewhere. As an exact count, an $8\times8$ single-channel input with four $3\times3$ filters and valid stride-one [convolution](../../../convolution.md) produces a $6\times6\times4$ output using **$4(9+1)=40$ parameters**. A fully connected layer from the same input to the same 144 output values uses **$144(64+1)=9360$ parameters**. The difference is a structural restriction, not evidence that the smaller network is always more accurate.

Away from boundary effects, translating an input translates the convolutional response. This is [translation equivariance](../../../translation-equivariance.md), not complete invariance. Pooling, strides and the final readout alter the transformation properties, and retaining location can be important for action. Hierarchical local features and expanding [receptive fields](../../../receptive-field.md) resemble aspects of the [ventral visual stream](../../../ventral-visual-stream.md); exact copying of one numerical filter across all positions is an idealization of biological connectivity. Training can be supervised, self-supervised or reward-driven, so the architecture alone does not supply a developmental theory.

A [recurrent neural network](../../../recurrent-neural-network.md) updates a state as new input arrives,

$$
h_t=\phi(Ux_t+Wh_{t-1}+b),\qquad y_t=\psi(Vh_t+c).
$$

The same current observation can then produce different outputs depending on history. This is useful for sequence prediction, [working memory](../../../working-memory.md), control under partial observation and sequential inference. For an original scalar example, let $h_t=h_{t-1}/2+x_t$ with $h_0=0$. Sequences $(1,0)$ and $(0,0)$ have the same final input but final states $1/2$ and $0$. A feedforward map of only that final input cannot distinguish them. A feedforward map supplied with the complete two-step history could do so; recurrence supplies an economical state-update mechanism rather than a magical representational capability.

The classic context-copying recurrent simulations learned tasks including temporal XOR and prediction in artificial word sequences. Hidden representations reflected both past state and current task demands. These computational experiments demonstrate how useful categories and temporal information can emerge, but do not show that a biological circuit uses the same weights, [training data](../../../training-data.md) or learning procedure.[Abstract; Cognitive Science 14, pp. 179–211, recurrent context, temporal XOR and sequence-learning simulations](../../../finding-structure-in-time-by-jeffrey-l-elman.md)

Recurrent learning is also harder to explain biologically. [Backpropagation through time](../../../backpropagation-through-time.md) differentiates through repeated state updates and can train all recurrent parameters, but [gradients](../../../gradient.md) can vanish or grow as they traverse many steps. Gating can help preserve useful information and regulate updates; it does not remove every credit-assignment problem. Activity and stability depend on the operating regime. Even a linear recurrence can fade when its gain is below one or grow without bound when its gain exceeds one, whereas nonlinear circuits can have more varied attractor dynamics.

Real [neural circuits](../../../neural-circuit.md) contain feedforward, lateral and feedback connections, delayed spikes, separate inhibitory and excitatory cells, and locally regulated plasticity. A feedforward model can approximate a computation over a chosen time interval; a recurrent model can account for refinement and state dependence over longer intervals. Neither is a complete cell-level description. Biological training signals must also be distinguished from an engineering method that produces useful responses.

**Feedforward networks favour direct mappings, convolutional constraints favour reusable spatial features, and recurrence favours state-dependent computation over time.** Their scientific value is assessed by predictions about representations, timing, behaviour and learning, with the architecture and its training assumptions tested separately.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2022](../../2022-split.md)
3. [Past exam of the how to build a brain from scratch course of the University of Oxford](../../split.md)
4. [How to build a brain from scratch course of the University of Oxford](../../../how-to-build-a-brain-from-scratch-course-of-the-university-of-oxford.md)
5. [Year 3 of the psychology (experimental) course of the University of Oxford](../../../year-3-of-the-psychology-experimental-course-of-the-university-of-oxford.md)
6. [Psychology (experimental) course of the University of Oxford](../../../psychology-experimental-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
