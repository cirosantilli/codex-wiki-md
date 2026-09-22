<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**[Temporal-difference learning](../../../temporal-difference-learning.md) uses sampled reward-plus-continuation predictions to approach a [Bellman expectation equation](../../../bellman-expectation-equation.md). Policy evaluation must be distinguished from finding an optimal policy.** Consider a finite [Markov decision process](../../../markov-decision-process.md), a fixed policy $\pi$, bounded rewards and discount $0\le\gamma<1$. Define

$$
V^\pi(s)=\mathbb E_\pi\!\left[\sum_{k=0}^{\infty}\gamma^kR_{t+k+1}\,\middle|\,S_t=s\right].
$$

Separating the first reward from the remaining return gives

$$
\boxed{V^\pi(s)=r^\pi(s)+\gamma\sum_{s'}P^\pi(s,s')V^\pi(s').}
$$

Here $r^\pi$ is expected immediate reward and $P^\pi$ is the transition [matrix](../../../matrix.md) under the fixed policy. In [matrix](../../../matrix.md) form, $V^\pi=(I-\gamma P^\pi)^{-1}r^\pi$. The inverse exists because the geometric series $\sum_{k\ge0}(\gamma P^\pi)^k$ converges in the [supremum norm](../../../supremum-norm.md).

Define the [Bellman expectation operator](../../../bellman-expectation-operator.md) $T^\pi V=r^\pi+\gamma P^\pi V$. A [stochastic matrix](../../../stochastic-matrix.md) averages component differences, so

$$
\|T^\pi V-T^\pi U\|_\infty\le\gamma\|V-U\|_\infty.
$$

The [Banach fixed-point theorem](../../../contraction-mapping-theorem.md) gives a unique [fixed point](../../../fixed-point.md) and convergence of exact repeated backups. This establishes why the equation has a well-defined solution in the stated discounted setting; it does not require the [intelligent agent](../../../intelligent-agent.md) to know its transition [matrix](../../../matrix.md).

The model-free alternative observes $(S_t,R_{t+1},S_{t+1})$ and forms

$$
\delta_t=R_{t+1}+\gamma V_t(S_{t+1})-V_t(S_t),\qquad V_{t+1}(S_t)=V_t(S_t)+\alpha_t\delta_t.
$$

Other tabular entries remain unchanged. Under the same policy and Markov assumptions, conditioning on the current value estimates gives

$$
\mathbb E[\delta_t\mid S_t=s,V_t]=(T^\pi V_t)(s)-V_t(s).
$$

Thus the sample error has the correct mean direction for correcting the current Bellman mismatch. The defining idea is bootstrapping: a later prediction supplies part of the earlier prediction's target, so learning need not wait for a final outcome.[Abstract and sections 2–3; successive predictions and temporal credit assignment](../../../learning-to-predict-by-the-methods-of-temporal-differences-by-richard-s-sutton.md)

In [tabular temporal-difference policy evaluation](../../../tabular-temporal-difference-policy-evaluation.md), convergence requires appropriate sampling and step sizes, not merely writing the update. Standard sufficient conditions include bounded rewards, infinitely many visits to each relevant state and, along visits to each state, $\sum_t\alpha_t(s)=\infty$ with $\sum_t\alpha_t(s)^2<\infty$. Diminishing steps allow continuing correction while limiting accumulated sampling noise. Constant steps generally track a noisy estimate instead of converging exactly. The target's dependence on the present values also means that this is not ordinary [gradient descent](../../../gradient-descent-split.md) on an independent, fixed supervised label. These tabular guarantees should not be transferred automatically to nonlinear function approximation or off-policy training.

For an exact illustrative problem, alternate deterministically between states $A$ and $B$, receive reward $1$ on leaving $A$ and $0$ on leaving $B$, and take $\gamma=1/2$. Then

$$
V_A=1+\frac12V_B,\qquad V_B=\frac12V_A,\qquad\boxed{V_A=\frac43,\quad V_B=\frac23.}
$$

Starting from zero with step size $1/2$, the first transition updates $V_A$ to $1/2$; the next updates $V_B$ to $1/8$. At the exact solution, both transition errors are zero. These values are a model calculation, not neural measurements.

This solves evaluation of the specified policy. The optimal [Bellman equation](../../../bellman-equation.md) instead maximizes over possible actions. An [intelligent agent](../../../intelligent-agent.md) can combine policy evaluation with [policy iteration](../../../policy-iteration.md) or an [actor-critic](../../../actor-critic-architecture.md) improvement mechanism. Estimating the value of a poor fixed policy does not by itself make that policy optimal. Episodic tasks use terminal-state value zero; undiscounted continuing tasks require additional conditions or a different formulation.

A proposed neural implementation uses a representation of the situation to drive a value-predicting population, with a [reward prediction error](../../../reward-prediction-error.md) modulating recently active [synapses](../../../synapse.md). An [eligibility trace](../../../eligibility-trace.md) can preserve a record of prior activity so delayed errors influence earlier states. Temporal representation is indispensable: if the population does not distinguish when a reward is expected, it cannot generate the appropriate omission signal at that time.

Primate recordings during acquisition of successive delayed-response tasks found that dopamine-neuron reward responses were more prominent during learning than after performance was established, while significant cues elicited phasic responses. This supports prediction-sensitive signalling but also allows attentional and motivational contributions.[Abstract; Journal of Neuroscience 13, pp. 900–913, learning versus established task performance](../../../responses-of-monkey-dopamine-neurons-to-reward-and-conditioned-stimuli-during-successive-steps-of-learning-a-delayed-response-task-by-wolfram-schultz-and-others.md) The temporal-difference interpretation explains how a reward response can diminish as reward becomes predicted and a response can develop at an informative cue; a worse-than-expected omission gives a negative error. The physiological interpretation is a quantitative hypothesis, not an identification of every [dopamine](../../../dopamine.md) signal with a single critic variable.[Science 275, pp. 1593–1599, temporal-difference interpretation of reward and cue responses](../../../a-neural-substrate-of-prediction-and-reward-by-wolfram-schultz-and-others.md)

Causal evidence comes from reward-timed stimulation of [dopamine](../../../dopamine.md) [neurons](../../../neuron-split.md) in rat blocking and extinction tasks. Artificial activation, intended to supply a positive prediction-error-like event, increased subsequent cue-driven reward seeking. This strengthens the teaching-signal interpretation beyond response correlation. It does not show that all components of the Bellman computation reside in [dopamine](../../../dopamine.md) [neurons](../../../neuron-split.md) or that the entire algorithm is unique.[Abstract and Figures 1–4, reward-timed [dopamine](../../../dopamine.md) stimulation in blocking and extinction](../../../a-causal-link-between-prediction-errors-dopamine-neurons-and-learning-by-elizabeth-e-steinberg-and-others.md)

**The mathematical bridge is precise: the mean TD error is the sampled Bellman mismatch, and appropriate repeated updates solve tabular policy evaluation. Neural evidence supports prediction-sensitive plasticity signals, while state representation, timing, function approximation and action improvement remain distinct parts of the implementation.**

## ↑ Ancestors (11)

1. [4](../4.md)
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
