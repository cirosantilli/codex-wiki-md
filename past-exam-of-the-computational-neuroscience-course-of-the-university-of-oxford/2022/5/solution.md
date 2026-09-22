<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

**[Error-correction learning](../../../error-correction-learning.md) adjusts a network using a discrepancy between a desired and an actual outcome. Different architectures differ in how they represent that discrepancy and assign it to earlier [synapses](../../../synapse.md).** This must be distinguished from simply strengthening every coactive pair through [Hebbian learning](../../../hebbian-learning.md), and from an autonomous error-correcting memory retrieving a stored attractor.

For a single-layer linear output $y=Wx$, let $t$ be the teaching target and $L=\|t-y\|^2/2$. The [delta rule](../../../delta-rule.md) is an exact [gradient descent](../../../gradient-descent-split.md) update,

$$
\Delta W=\eta(t-y)x^{\mathsf T}.
$$

For one example, $e'=t-(W+\eta ex^{\mathsf T})x=(1-\eta\|x\|^2)e$, so $0<\eta\|x\|^2<2$ decreases its squared error unless it is already zero. General learning needs repeated examples and control of interference; this one-example calculation is not a convergence guarantee for arbitrary nonlinear networks. The [perceptron algorithm](../../../perceptron.md) instead updates a threshold classifier on misclassified examples. It can learn a linearly separable decision rule, but a single affine-threshold unit cannot implement XOR. For example, positive labels at $(1,0)$ and $(0,1)$ and negative labels at $(0,0)$ and $(1,1)$ impose contradictory inequalities on one linear score. More layers are needed to learn a suitable feature representation.

A [multilayer perceptron](../../../multilayer-perceptron.md) uses nonlinear [hidden units](../../../hidden-unit.md) before the output. For squared error, write $h=\sigma(Ux)$ and $y=\sigma(Vh)$. Define output and hidden teaching signals by

$$
\delta^o=(t-y)\odot\sigma'(Vh),\qquad\delta^h=(V^{\mathsf T}\delta^o)\odot\sigma'(Ux).
$$

Then [backpropagation](../../../backpropagation.md) computes $\Delta V=\eta\delta^o h^{\mathsf T}$ and $\Delta U=\eta\delta^h x^{\mathsf T}$, using the same pre-update weights. The [chain rule](../../../chain-rule.md) makes these exact negative [gradients](../../../gradient.md). Unlike a fixed-feature [perceptron](../../../perceptron.md), hidden representations can change to make a difficult task separable. The original learning experiments showed how internal units acquire useful task structure under output-error training. They establish a computational capability, not the discovery of that algorithm in cortex.[Abstract; pp. 533–536, hidden representations and gradient-based error correction](../../../learning-representations-by-back-propagating-errors-by-david-e-rumelhart-and-others.md)

A [recurrent neural network](../../../recurrent-neural-network.md) can use state $h_{t+1}=\sigma(Ah_t+Bx_t)$ to integrate a sequence and produce an output after a delay. Error correction must now assign responsibility to earlier states as well as earlier layers. Applying the [chain rule](../../../chain-rule.md) through the unrolled recurrence solves the algorithmic problem, but storing the required history and transporting a late teaching signal to an earlier [synapse](../../../synapse.md) is biologically demanding. Repeated multiplication by the recurrent [Jacobian matrix](../../../jacobian-matrix.md) can also create the [vanishing gradient problem](../../../vanishing-gradient-problem.md) or the [exploding gradient problem](../../../exploding-gradient-problem.md). A local [eligibility trace](../../../eligibility-trace.md) can retain a record of recent synaptic participation for modulation by a later error signal, although that is not generally an exact replacement for the full recurrent [gradient](../../../gradient.md).

A biologically motivated comparison is the [cerebellum](../../../cerebellum.md). A broad input representation can be expanded by [granule cells](../../../granule-cell.md); [parallel fibers](../../../parallel-fiber.md) carry the resulting activity to [Purkinje cells](../../../purkinje-cell.md), while a [climbing fiber](../../../climbing-fiber.md) provides a separate instructive input. Such a circuit resembles a supervised adaptive filter: an active input is modified in a manner depending on a teaching signal, with Purkinje output affecting downstream motor control. The correspondence is a circuit hypothesis, not a claim that the climbing-fiber event equals the signed scalar $t-y$ in every task.

An instructive experiment recorded [Purkinje cells](../../../purkinje-cell.md) in monkeys tracking a moving visual target. A change in target direction supplied a learning instruction, and subsequent eye velocity and simple-spike activity measured trial-over-trial adaptation. Longer complex spikes were associated with larger subsequent simple-spike depression and stronger behavioural learning. Comparing trials matched for preceding simple-spike activity helped rule out that activity alone as the explanation. This connects a separable teaching-related event to later plasticity during behaviour, but extracellular recordings do not directly reveal the numerical update at every [parallel fiber](../../../parallel-fiber.md) [synapse](../../../synapse.md), and the finding does not demonstrate multilayer [backpropagation](../../../backpropagation.md).[Figures 1–4 and Methods; author manuscript at PMC4132823: smooth pursuit, trial-over-trial plasticity and controls for prior simple-spike activity](../../../purkinje-cell-plasticity-and-cerebellar-motor-learning-are-graded-by-complex-spike-duration-by-yan-yang-and-others.md)

For cortex, exact textbook [backpropagation](../../../backpropagation.md) faces a [weight transport problem](../../../weight-transport-problem.md): the hidden teaching signal uses the transpose of the actual forward matrix, while a real feedback pathway has its own independently adjustable [synapses](../../../synapse.md). It also needs a way to deliver a target or prediction error, keep learning signals distinct from ordinary activation, and convert them to local plasticity under spiking, delays and sign constraints. The mere presence of anatomical feedback does not establish this computation.

[Feedback alignment](../../../feedback-alignment.md) weakens one requirement: replace $V^{\mathsf T}\delta^o$ by $B\delta^o$ for a fixed random feedback matrix $B$. Simulations showed that changing forward weights can make these approximate teaching directions useful, even without exact reciprocal weights. This is evidence that the [weight transport problem](../../../weight-transport-problem.md) need not forbid useful deep error correction; it is not evidence that arbitrary feedback always converges, that the updates remain exact [gradient descent](../../../gradient-descent-split.md), or that this precise mechanism has been recorded in the [brain](../../../brain.md). The work explicitly leaves the physiological implementation and the interaction between feedback activation and learning unresolved.[Results, Figure 1 and Figure 2; Discussion: random feedback, learning performance and biological limitations](../../../random-synaptic-feedback-weights-support-error-backpropagation-for-deep-learning-by-timothy-p-lillicrap-and-others.md)

**Local supervised error correction has a plausible circuit substrate and direct behavioural-physiological support. Multilayer and recurrent error correction are powerful explanatory possibilities, but their teaching signals, temporal credit assignment and feedback pathways must be established experimentally.** Different architectures should be compared by held-out learning behaviour, representational changes and pathway-specific intervention, rather than by labelling all feedback as [backpropagation](../../../backpropagation.md).

## ↑ Ancestors (11)

1. [5](../5.md)
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
