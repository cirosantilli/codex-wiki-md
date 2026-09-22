<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A common computational target is plausible: [retrospective confidence](../../../retrospective-confidence.md) evaluates whether an already selected answer is correct. In a [Bayesian inference](../../../bayesian-statistics-split.md) model this can be written $P(\text{selected answer correct}\mid\text{available evidence, action})$. The evidence might be a sensory signal in [perception](../../../perception.md) or retrieved information in [memory retrieval](../../../memory-retrieval.md). A shared target does not require the same evidence representation, parameters or neural implementation in both domains.

A basic [signal detection theory](../../../signal-detection-theory.md) account illustrates the common structure. Two alternatives generate different distributions of internal evidence, the decision selects an alternative, and confidence reflects evidence relative to the decision boundary. With equal prior probabilities and two alternatives, let $L$ be the [log-likelihood ratio](../../../log-likelihood-ratio.md) for the observed evidence. For the alternative with the larger posterior probability, [confidence as posterior correctness probability](../../../confidence-as-posterior-correctness-probability.md) gives

$$
P(\text{correct}\mid L)=\frac{1}{1+e^{-|L|}}.
$$

This is a normative consequence of the assumed model, rather than a universal empirical law. The same algebra can describe old/new recognition or a perceptual discrimination only when their assumed likelihoods, priors and decision rule justify it. An old/new discrimination also has a different response structure from comparing two simultaneously presented objects.

A different common account is [self-consistency theory of confidence](../../../self-consistency-theory-of-confidence.md): confidence tracks how consistently a choice is supported across sampled representations. [Asher Koriat](../../../asher-koriat.md) found predictions of this account, previously applied to knowledge judgments, also held in perceptual judgments.[2011, abstract: consistency, response latency and confidence–correctness dissociations](../../../subjective-confidence-in-perceptual-judgments-by-asher-koriat.md) Its distinctive implication is that confidently repeated errors are possible when misleading evidence consistently favours the wrong choice. Reliable internal agreement need not entail external correctness. This differs from simply identifying subjective confidence with an objectively calibrated posterior.

Important limitations remain. Recognition can be supported by [familiarity](../../../familiarity.md) and [recollection](../../../recollection.md), while a perceptual choice may depend on a currently visible stimulus. The content and timing of evidence differ. Confidence can incorporate an additional retrieval attempt, response fluency, or evidence acquired after the initial decision. A common computation can therefore give different levels of metacognitive efficiency across tasks without requiring a wholly different function for confidence. Conversely, similar average rating curves do not prove a single mechanism: quite different latent processes can produce them.

[Second-order inference about decisions](../../../second-order-inference-about-decisions.md) makes the relation explicit by distinguishing the information supporting the decision from the partially correlated information supporting its evaluation.[2017, distinction between first-order, postdecisional and second-order architectures](../../../self-evaluation-of-decision-making-a-general-bayesian-framework-for-metacognitive-computation-by-stephen-m-fleming-and-nathaniel-d-daw.md) A model in which confidence has exactly the same evidence as the choice is a stronger hypothesis than a model with a shared inferential goal and separate noisy samples. Error detection and later changes of mind are useful tests because they constrain what further information confidence can use.

Strong evidence for a common mechanism would include quantitative predictions across domains, transfer to a new domain after controlled training, and common effects of selective interventions after matching first-order performance. A shared brain region or a cross-task correlation alone is insufficient: task demands and measurement reliability can produce either apparent commonality or apparent dissociation. **The most defensible common basis is a family of evidence-based evaluations of correctness, while the claim of one identical process for memory and perception remains substantially stronger.**

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2022](../../2022-split.md)
3. [Past exam of the metacognition course of the University of Oxford](../../split.md)
4. [Metacognition course of the University of Oxford](../../../metacognition-course-of-the-university-of-oxford.md)
5. [Year 3 of the psychology (experimental) course of the University of Oxford](../../../year-3-of-the-psychology-experimental-course-of-the-university-of-oxford.md)
6. [Psychology (experimental) course of the University of Oxford](../../../psychology-experimental-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
