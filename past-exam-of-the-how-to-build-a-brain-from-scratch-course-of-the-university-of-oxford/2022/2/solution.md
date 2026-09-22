<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**[Complementary learning systems](../../../complementary-learning-systems.md) address the conflict between rapidly remembering a particular experience and gradually learning shared structure without destroying prior knowledge.** In the 1995 framework, the [hippocampal](../../../hippocampus.md) system rapidly stores relatively separated event representations, while the [neocortex](../../../neocortex.md) learns more slowly through overlapping representations. Separation reduces interference between episodes; overlap allows related experiences to influence common features and support [generalization](../../../generalization-in-statistical-learning.md). The [hippocampal](../../../hippocampus.md) system can reinstate experiences for interleaved cortical learning. Thus the distinction is not simply a short-lived store versus a long-lived store, nor two copies differing only in learning rate. Representation, learning dynamics and communication between systems are complementary.[Psychological Review 102, pp. 419–457; pp. 432–435 and Figures 9–11, interference and interleaved learning; later sections on consolidation](../../../why-there-are-complementary-learning-systems-in-the-hippocampus-and-neocortex-insights-from-the-successes-and-failures-of-connectionist-models-of-learning-and-memory-by-james-l-mcclelland-and-others.md)

The computational difficulty is [catastrophic interference](../../../catastrophic-interference.md). When many memories share parameters, updates that improve a new task can impair previous tasks. Completely isolating every experience would reduce this problem, but would also prevent useful transfer through shared features. The [intelligent agent](../../../intelligent-agent.md) therefore faces a [stability-plasticity dilemma](../../../stability-plasticity-dilemma.md): it needs to remain responsive to new evidence while retaining useful old structure.

An original linear example exposes the issue without assuming contradictory facts. Let $f_w(x)=w^{\mathsf T}x$. An old example is $x_A=(1,0)$ with target $1$, already fitted by $w=(1,0)$. A new example is $x_B=(1,1)$ with target $0$. One [gradient descent](../../../gradient-descent-split.md) step on its squared error, with learning rate $1/2$, gives

$$
w'=(1,0)-\frac12(1-0)(1,1)=(1/2,-1/2).
$$

The new prediction is now correct, but the old prediction falls from $1$ to $1/2$. Both examples could have been fitted exactly by $w_*=(1,-1)$, so the loss is due to the training history, not an impossible specification. Interleaving old and new examples instead estimates the [gradient](../../../gradient.md) of their joint [loss function](../../../loss-function.md),

$$
L(w)=\frac12\left[(w_1-1)^2+(w_1+w_2)^2\right],
$$

whose unique minimum is $w_*$. This small calculation illustrates interference and the benefit of retaining old constraints; it is not a reproduction of the published CLS simulations or measured forgetting.

A fast episodic store gives the [intelligent agent](../../../intelligent-agent.md) immediate access to the new observation even while its slower predictive system is still learning. Subsequent retrieval supplies examples to be mixed with new experience. Over many updates, the slower system can extract regularities while accommodating exceptions. The mathematical target is a suitably weighted mixture of previous and current experience, not necessarily an exact photographic copy of every past event. Biased or incomplete replay can still distort learning, and finite storage does not eliminate the stability problem indefinitely.

The anatomical proposal fits previously established computations: [dentate gyrus](../../../dentate-gyrus.md) sparsification and [pattern separation](../../../pattern-separation.md), recurrent [hippocampal CA3](../../../hippocampal-ca3.md) association, and [hippocampal CA1](../../../hippocampal-ca1.md) and cortical output pathways for reinstatement. These functions give a plausible route from a partial cue to a reactivated episode. They do not require every [neuron](../../../neuron-split.md) or every memory to obey one perfectly separated code. A complementary architecture also need not imply that cortex never learns rapidly.

A motivating recording experiment compared [hippocampal](../../../hippocampus.md) place-cell coactivity during spatial behaviour with sleep before and after it. Cell pairs coactive during behaviour were more likely to coactivate in subsequent sleep; inactive or spatially nonoverlapping pairs provided controls. This supports experience-related reactivation, rather than merely elevated firing during sleep. The 1994 result concerns ensemble coactivation: it should not be inflated into direct proof that a complete temporally ordered memory was transferred into cortex.[Abstract; Science 265, pp. 676–679, place-cell coactivation before and after spatial experience](../../../reactivation-of-hippocampal-ensemble-memories-during-sleep-by-matthew-a-wilson-and-others.md)

Intervention adds a different kind of evidence. Selectively suppressing [hippocampal](../../../hippocampus.md) [sharp-wave ripples](../../../sharp-wave-ripple.md) during post-training consolidation periods impaired a spatial memory task in rats. This supports a functional role for ripple-associated processing, but does not reveal which information was replayed or establish that cortical weight changes followed the exact interleaving algorithm.[Abstract; Nature Neuroscience 12, pp. 1222–1223, post-training ripple suppression](../../../selective-suppression-of-hippocampal-ripples-impairs-spatial-memory-by-gabrielle-girardeau-and-others.md)

An important qualification comes from flavour–place learning. After rats had acquired a structured set of associations, new information fitting that schema could be consolidated much more rapidly. This challenges an account in which cortical integration always requires the same long delay. It is compatible with the broader computational idea that information consistent with an established representation can be incorporated with less disruptive change.[Abstract; Science 316, pp. 76–82, flavour–place paired associates and schema-dependent rapid consolidation](../../../schemas-and-memory-consolidation-by-dorothy-tse-and-others.md)

For artificial [intelligent agents](../../../intelligent-agent.md), an [episodic memory](../../../episodic-memory.md) and [experience replay](../../../experience-replay.md) can similarly support rapid use of new observations and continued training of shared representations. This is a functional analogy, not proof that a replay buffer reproduces the [hippocampus](../../../hippocampus.md). It needs appropriate retrieval, protection against sampling bias and a representation that preserves relevant context. Exact episode details, semantic regularities and current goals may require different readouts.

**The central contribution of [complementary learning systems](../../../complementary-learning-systems.md) is a computational explanation of why rapid episodic storage and overlapping [generalization](../../../generalization-in-statistical-learning.md) should cooperate.** The theory predicts distinctive effects of learning history, replay disruption and prior knowledge, while its biological implementation and the eventual [hippocampal](../../../hippocampus.md) dependence of detailed memories remain matters for further testing.

## ↑ Ancestors (11)

1. [2](../2.md)
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
