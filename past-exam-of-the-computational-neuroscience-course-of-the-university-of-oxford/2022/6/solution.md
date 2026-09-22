<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

**An [actor-critic architecture](../../../actor-critic-architecture.md) learns a situation-to-action policy from rewards while a separate value network evaluates its consequences.** It is a concrete [reinforcement learning](../../../reinforcement-learning.md) architecture: no supervisor supplies the correct action on each trial. In a finite [Markov decision process](../../../markov-decision-process.md), let $x(s)$ encode the current situation, $r_{t+1}$ be the reward after action $a_t$, and $0\le\gamma<1$ discount future rewards. The objective is expected return, $\mathbb E_\pi\sum_{t\ge0}\gamma^t r_{t+1}$. For an episodic undiscounted task, termination can instead make the return finite. State representation matters: if the sensory input does not identify the relevant situation, a memory of previous observations must be added.

The actor has preferences $u_a^{\mathsf T}x(s)$ and selects actions using a [softmax function](../../../softmax-function.md),

$$
\pi_u(a\mid s)=\frac{\exp(u_a^{\mathsf T}x(s))}{\sum_b\exp(u_b^{\mathsf T}x(s))}.
$$

Sampling from this policy supplies exploration. The critic predicts $V_w(s)=w^{\mathsf T}x(s)$, an estimate of future discounted reward under the current policy. Its [temporal-difference learning](../../../temporal-difference-learning.md) signal is

$$
\delta_t=r_{t+1}+\gamma V_w(s_{t+1})-V_w(s_t),
$$

with $V_w=0$ at a terminal state. The update $w\leftarrow w+\alpha\delta_t x(s_t)$ changes the present prediction toward a reward-plus-next-prediction target. It is a semi-gradient update: it does not differentiate through the bootstrapped target. The temporal-difference principle assigns credit using successive predictions rather than waiting for a complete episode to end.[Abstract and sections 2–3; Machine Learning 3, pp. 9–44: successive predictions and temporal credit assignment](../../../learning-to-predict-by-the-methods-of-temporal-differences-by-richard-s-sutton.md)

A corresponding actor update is

$$
u_a\leftarrow u_a+\beta\delta_t\bigl(\mathbf1_{\{a=a_t\}}-\pi_u(a\mid s_t)\bigr)x(s_t).
$$

The bracketed term is the [gradient](../../../gradient.md) of the log policy with respect to the preference for action $a$. A positive [reward prediction error](../../../reward-prediction-error.md) increases the probability of the selected action; a negative one decreases it. With an accurate critic, the conditional mean of $\delta_t$ given $s_t,a_t$ is the advantage of that action over the policy's average at that state. This motivates the update, while approximate values, changing policies and limited exploration can compromise learning. It is not a guarantee of the globally best behaviour for every choice of features and learning rates.

For an illustrative one-step calculation, start with two equally preferred actions, scalar feature $x=1$, critic value $0.5$, and a chosen first action followed by reward $1$. Then $\delta=0.5$. With actor learning rate $\beta=0.1$, its two preference changes are $+0.025$ and $-0.025$, so the next probability of the rewarded action is $1/(1+e^{-0.05})\approx0.5125$. These are chosen model values. A delayed reward can also modify recently active connections through an [eligibility trace](../../../eligibility-trace.md), for example $e_t=\gamma\lambda e_{t-1}+x(s_t)$ for the critic, followed by $\Delta w=\alpha\delta_t e_t$. The actor needs its own policy-gradient eligibility. Traces must be reset or otherwise handled at episode boundaries.

The key biological hypothesis is a three-factor plasticity rule: presynaptic activity, postsynaptic or action-selection activity, and a modulatory [reward prediction error](../../../reward-prediction-error.md). Cortical inputs to the [striatum](../../../striatum.md) can provide situation features, action-related populations can supply the actor, and [dopamine](../../../dopamine.md) can modulate plasticity. This is a functional correspondence, not a one-to-one identification of all actor units with one anatomical compartment. The critic itself must be learned; delivering reward directly to every active connection would not explain prediction-dependent changes.

Recordings in monkeys trained through successive delayed-response tasks provide relevant primary evidence. Phasic responses of putative [dopamine](../../../dopamine.md) [neurons](../../../neuron-split.md) to liquid reward were more common during learning than after task performance had become established, while significant stimuli continued to elicit responses. This is compatible with a learning signal sensitive to predictability rather than a permanent readout of reward consumption, but the study also emphasizes attentional and motivational interpretations.[Abstract; Journal of Neuroscience 13, pp. 900–913: learning versus established performance](../../../responses-of-monkey-dopamine-neurons-to-reward-and-conditioned-stimuli-during-successive-steps-of-learning-a-delayed-response-task-by-wolfram-schultz-and-others.md) The canonical [temporal-difference learning](../../../temporal-difference-learning.md) interpretation predicts increased signalling for an unexpectedly good outcome and decreased signalling when an expected reward fails to occur; it explains why cue and reward responses can change as predictions are learned. This is a quantitative interpretation of physiological evidence, not an assertion that all [dopamine](../../../dopamine.md) activity equals one scalar critic error.[Abstract and reward-prediction-error interpretation; Science 275, pp. 1593–1599](../../../a-neural-substrate-of-prediction-and-reward-by-wolfram-schultz-and-others.md)

The model also explains [classical conditioning](../../../classical-conditioning.md) phenomena such as blocking. If an established cue already predicts the reward, adding another cue leaves little positive prediction error, so the new cue acquires little value. More causally informative experiments in rats stimulated [dopamine](../../../dopamine.md) [neurons](../../../neuron-split.md) at reward delivery in blocking and extinction procedures. The stimulation, timed to mimic a positive prediction error, produced lasting increases in cue-elicited reward seeking. This supports a teaching role for phasic [dopamine](../../../dopamine.md), rather than merely a correlation with successful behaviour. It does not identify every [synapse](../../../synapse.md) or prove that a complete [actor-critic](../../../actor-critic-architecture.md) algorithm is the only explanation.[Abstract and Figures 1–4: associative blocking, extinction and reward-timed dopamine-neuron stimulation](../../../a-causal-link-between-prediction-errors-dopamine-neurons-and-learning-by-elizabeth-e-steinberg-and-others.md)

**The simplest model-free [actor-critic](../../../actor-critic-architecture.md) is consistent with important aspects of learning, but it does not exhaust animal behaviour.** It gradually caches action preferences. It cannot immediately change an unvisited action's value after an outcome is devalued unless the state or reward representation supplies an additional route to that change. In an [instrumental conditioning](../../../instrumental-conditioning.md) experiment in rats, lever pressing trained on interval schedules became insensitive to sucrose devaluation in sham controls, whereas dorsolateral-striatal lesions preserved sensitivity to devaluation. Consumption controls showed that devaluation itself was effective, and testing in extinction limited new reward learning. This dissociation supports a distinction between habitual and goal-directed control, rather than one universal cached policy.[Abstract, experiments 1–2; pp. 181–189: interval training, devaluation, extinction test and lesion controls](../../../lesions-of-dorsolateral-striatum-preserve-outcome-expectancy-but-disrupt-habit-formation-in-instrumental-learning-by-henry-h-yin-and-others.md)

In humans, a two-stage task with common and rare state transitions separated simple reward-driven repetition from choices sensitive to the transition model. Behaviour and striatal prediction-error-related imaging signals showed both [model-free reinforcement learning](../../../model-free-reinforcement-learning.md) and [model-based reinforcement learning](../../../model-based-reinforcement-learning.md) influences. The imaging signal is not a direct measurement of individual [dopamine](../../../dopamine.md) spikes, and task performance alone does not uniquely identify a circuit, but it argues against treating every striatal value signal as purely model-free.[Abstract; Results, two-stage choice task; Discussion: model-based and model-free influences](../../../model-based-influences-on-humans-choices-and-striatal-prediction-errors-by-nathaniel-d-daw-and-others.md)

A stronger architecture can combine the learned [actor-critic](../../../actor-critic-architecture.md) with a model of action–outcome transitions and current outcome value, and arbitrate between cached action selection and planning. **The model's strength is its explicit account of exploration, delayed credit and prediction-dependent plasticity; its limits become visible in devaluation, latent learning and rapid replanning.**

## ↑ Ancestors (11)

1. [6](../6.md)
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
