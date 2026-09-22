<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

**A [world model](../../../world-model.md) supports intelligent behaviour by predicting the consequences of actions that need not be executed first. The [prefrontal cortex](../../../prefrontal-cortex.md) can contribute task-state and goal control, while the [hippocampus](../../../hippocampus.md) can supply relational and episodic content for constructing possible situations and trajectories.** This is a division of computational requirements, not a rigid one-region-per-function scheme.

In a [Markov decision process](../../../markov-decision-process.md), a model can represent transitions $\widehat P(s'\mid s,a)$ and expected rewards $\widehat r(s,a)$. [Planning](../../../planning.md) uses them to evaluate an action through a backup such as

$$
\widehat Q(s,a)=\widehat r(s,a)+\gamma\sum_{s'}\widehat P(s'\mid s,a)\widehat V(s').
$$

Longer searches apply the same principle across alternative trajectories. A [world model](../../../world-model.md) can be symbolic, distributed, probabilistic or a combination; it need only preserve information relevant to the decision. In a partially observed situation, the [intelligent agent](../../../intelligent-agent.md) must infer a state or maintain uncertainty over states rather than treating the latest image as a complete description of the world.

For a simple constructed example, suppose one action leads to food and another to water, with current outcome values $2$ and $1$. After the food is devalued to $0$, an [intelligent agent](../../../intelligent-agent.md) that knows the action–outcome relations can immediately prefer water without experiencing the food-producing action again. A purely cached action value does not necessarily change at that moment. This demonstrates the usefulness of an internal model; it does not imply that every devaluation effect uniquely identifies one algorithm, because inferred state changes or offline value updates can also alter cached decisions.

[Mental simulation](../../../mental-simulation.md) can recombine remembered components into a possible future, evaluate an untried route and compare goals. It differs from simply replaying a previous trajectory verbatim. It also differs from [episodic memory](../../../episodic-memory.md) retrieval: simulated content may describe something that never happened. Both operations can use shared representations, so a new imagined situation need not be generated independently of memory.

The [prefrontal cortex](../../../prefrontal-cortex.md) is well placed to contribute the control side of this process: maintaining the current task, selecting relevant information, representing goals and using prospective outcomes to guide action. It is heterogeneous, and activity in one subregion is not evidence that all of [prefrontal cortex](../../../prefrontal-cortex.md) carries a complete internal simulator. A particularly relevant hypothesis concerns the [orbitofrontal cortex](../../../orbitofrontal-cortex.md): a useful decision state may depend on previous events and task rules even when current sensory input is unchanged.

A human fMRI study used superimposed face and house images with a rule determining which category to judge from the preceding task history. Different hidden task states could therefore accompany similar current inputs. Cross-validated multivariate decoding recovered task-state information from [orbitofrontal cortex](../../../orbitofrontal-cortex.md), and decoding fidelity related to behavioural accuracy. This supports a role in representing the situation in which values and actions are evaluated. It does not demonstrate that the decoded patterns themselves contain a complete future trajectory, and noninvasive imaging cannot identify the synaptic algorithm.[Abstract, Figures 1–5 and Experimental Procedures: hidden task states, face/house judgements and cross-validated fMRI decoding](../../../human-orbitofrontal-cortex-represents-a-cognitive-map-of-state-space-by-nicolas-w-schuck-and-others.md)

The [hippocampus](../../../hippocampus.md) provides a complementary source of spatial and relational content. A [cognitive map](../../../cognitive-map.md) describes relationships among locations or task states rather than only a sequence of rewarded responses. Such a representation can support a novel route when goals change, and event representations can contribute objects, locations and contextual relations to a simulated scene. Whether an internally generated sequence represents a possible future, a remembered past or a training signal must be tested rather than inferred from sequence-like firing alone.

In freely moving rats choosing journeys between food locations, [hippocampal](../../../hippocampus.md) place-cell ensembles sometimes produced internally generated sequences before travel. Decoded sequences described trajectories related to remembered goals and predicted upcoming behaviour. The ordering and timing make the result relevant to prospective computation, but the recording is correlational: a sequence could reflect a prepared choice or goal-related retrieval rather than perform the decisive search itself.[Abstract and Results; Nature 497, pp. 74–79: awake ensemble sequences before goal-directed journeys](../../../hippocampal-place-cell-sequences-depict-future-paths-to-remembered-goals-by-brad-e-pfeiffer-and-others.md)

A separate intervention interrupted awake [sharp-wave ripples](../../../sharp-wave-ripple.md) during a spatial alternation task and impaired learning and performance. Place fields and post-experience reactivation were relatively preserved, helping distinguish the effect from wholesale destruction of spatial coding or later replay. This supports a causal contribution of awake ripple-associated processing to memory-guided decisions, without identifying every disrupted sequence as a [planning](../../../planning.md) calculation.[Abstract; Science 336, pp. 1454–1458: awake ripple interruption during spatial alternation](../../../awake-hippocampal-sharp-wave-ripples-support-spatial-memory-by-shantanu-p-jadhav-and-others.md)

Human lesion evidence extends the discussion beyond navigation. Patients with predominantly bilateral [hippocampal](../../../hippocampus.md) damage were asked to construct new experiences from short scenario cues. Their descriptions were generally less spatially coherent than those of matched controls, despite preserved semantic retrieval; one patient performed well. The task therefore supports a [hippocampal](../../../hippocampus.md) contribution to binding imagined scene elements, while the spared case, lesion selectivity and the difference between scene construction and action [planning](../../../planning.md) limit a universal necessity claim.[Results, Discussion and Methods: scenario construction, spatial coherence, preserved semantic retrieval and the spared patient](../../../patients-with-hippocampal-amnesia-cannot-imagine-new-experiences-by-demis-hassabis-and-others.md)

A plausible integrated model lets prefrontal representations specify the task and current goal, [hippocampal](../../../hippocampus.md) and cortical representations generate or retrieve candidate situations, and valuation and action-selection circuits compare their consequences. Communication can be iterative: candidate outcomes change what information is sought, and new observations update the inferred state. This is more specific than assigning “imagination” to the [hippocampus](../../../hippocampus.md) and “intelligence” to [prefrontal cortex](../../../prefrontal-cortex.md), but remains a hypothesis about their interaction.

[Planning](../../../planning.md) also has costs. Long simulations can amplify model errors, and unlimited search is computationally expensive. An [intelligent agent](../../../intelligent-agent.md) should select a useful abstraction, prioritize relevant branches and decide when a cached policy is adequate. Tests should distinguish sensitivity to reward changes from sensitivity to transition changes, and compare neural predictions before a decision rather than only after a successful action. **[World models](../../../world-model.md) enable flexible prospective control; the evidence implicates interacting state, memory and valuation processes, rather than a single anatomical seat of [mental simulation](../../../mental-simulation.md).**

## ↑ Ancestors (11)

1. [5](../5.md)
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
