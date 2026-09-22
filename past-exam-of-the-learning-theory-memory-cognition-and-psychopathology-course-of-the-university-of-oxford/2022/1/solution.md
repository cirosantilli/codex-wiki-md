<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**[Learning](../../../learning.md) theory explains pathological behaviour through representations, action selection, [controllability](../../../controllability.md) and retrieval as well as through [prediction errors](../../../prediction-error.md); mathematical description becomes explanatory only when those quantities are connected to people, environments and interventions.** A useful [computational psychiatry](../../../computational-psychiatry.md) account identifies the problem a person faces, the information available, the internal representation and the rule selecting an action. A fitted [learning](../../../learning.md) rate alone does not establish the cause of a [mental disorder](../../../mental-disorder.md).

First, distinguish [goal-directed action](../../../goal-directed-action.md) from [habit](../../../habit.md). A goal-directed controller evaluates outcomes using their current value, whereas a [habit](../../../habit.md) can repeat a previously acquired stimulus–response policy despite a changed outcome. An illustrative mixture is

$$
Q(a)=wQ_{\mathrm{goal}}(a)+(1-w)Q_{\mathrm{habit}}(a),\qquad 0\leq w\leq1.
$$

If washing formerly relieved distress, lowering the presently expected benefit need not immediately eliminate washing when the habitual component remains influential. This formulation distinguishes an erroneous [threat appraisal](../../../threat-appraisal.md) from failure to use an accurately represented outcome. Either can produce repetitive behaviour, so persistence alone does not distinguish the mechanisms.

An [outcome devaluation](../../../outcome-devaluation.md) experiment makes the distinction testable. In [Claire M. Gillan](../../../claire-m-gillan.md)'s study, people learned button responses to pictured stimuli for outcomes; instructions then made selected outcomes worthless, and a speeded [slips-of-action test](../../../slips-of-action-test.md) required withholding their associated responses. Participants with [OCD](../../../obsessive-compulsive-disorder.md) showed poorer outcome knowledge and greater devaluation-insensitive responding despite acquiring the trained responses. This supports deficient [goal-directed control](../../../goal-directed-action.md) rather than demonstrating exceptionally strong [habit](../../../habit.md) acquisition. Medication, task understanding and the difference between laboratory responses and actual compulsions limit the inference.[American Journal of Psychiatry 168, 718–726; Method, instructed outcome devaluation and slips-of-action test](../../../disruption-in-the-balance-between-goal-directed-behavior-and-habit-learning-in-obsessive-compulsive-disorder-by-claire-m-gillan-and-others.md)

Second, [action-outcome contingency](../../../action-outcome-contingency.md) separates frequent adversity from absent control. Define $\Delta P=P(O\mid A)-P(O\mid\neg A)$ for an aversive outcome $O$. With experimental action assignment, values $0.2-0.8=-0.6$ indicate that acting protects against the outcome, whereas $0.8-0.8=0$ supplies no such control. A learner who generalises zero control to a new situation may stop trying even when a useful action has become available. This is a route to helpless behaviour without merely asserting a large negative [prediction error](../../../prediction-error.md). Observational [conditional probabilities](../../../conditional-probability.md) require caution because an action may be chosen precisely when danger is greatest.

The motivating yoked-control logic holds exposure constant while changing whether a response terminates it. In rodent experiments, [Jose Amat](../../../jose-amat.md) and colleagues linked the protective effect of control to [medial prefrontal cortex](../../../medial-prefrontal-cortex.md) regulation of the [dorsal raphe nucleus](../../../dorsal-raphe-nucleus.md): prefrontal inactivation removed that protection. The circuit findings constrain a purely abstract account of [learned helplessness](../../../learned-helplessness.md), but neither the rodent procedure nor reduced escape defines human [depression](../../../depression.md).[Nature Neuroscience 8, 365–371; yoked escapable/inescapable stress and prefrontal inactivation](../../../medial-prefrontal-cortex-determines-how-stressor-controllability-affects-behavior-and-dorsal-raphe-nucleus-by-jose-amat-and-others.md)

Third, [negative reinforcement](../../../negative-reinforcement.md) can make avoidance locally successful and globally disabling. Leaving a feared situation removes distress, strengthening escape, while preventing experience that the situation would have been safe. The crucial informational question becomes whether safety is attributed to the environment or to the escape response. In a human [conditioning](../../../associative-learning.md) experiment, retaining an avoidance button during otherwise unreinforced cue presentations preserved threat expectancy and [skin conductance responses](../../../skin-conductance-response.md) when the button was subsequently unavailable. This supports a mechanism by which [safety behavior](../../../safety-behavior.md) can obstruct corrective [learning](../../../learning.md).[Behaviour Research and Therapy 47, 716–720; avoidance available during extinction and response-unavailable test](../../../safety-behaviours-preserve-threat-beliefs-by-peter-f-lovibond-and-others.md)

Fourth, retrieval is context dependent. An old [fear](../../../fear.md) association and subsequent [extinction learning](../../../extinction-learning.md) can coexist; the action observed depends on which learned association guides responding. In rat conditioned-suppression experiments, extinguishing a cue outside its acquisition context allowed [fear renewal](../../../fear-renewal.md) on return. Thus relapse can reflect a retrieval change rather than a failure to acquire anything during [treatment](../../../treatment.md). The account motivates practising safety across settings and testing retention outside the [treatment](../../../treatment.md) room.[Journal of Experimental Psychology: Animal Behavior Processes 9, 248–265; Experiments 1–4](../../../contextual-control-of-the-extinction-of-conditioned-fear-tests-for-the-associative-value-of-the-context-by-mark-e-bouton-and-others.md)

Mathematics also exposes ambiguity. For softmax action choice,

$$
P(a)=\frac{\exp(\beta Q(a))}{\sum_b\exp(\beta Q(b))},
$$

The [choice-value scale non-identifiability](../../../choice-value-scale-non-identifiability.md) follows because rescaling every value by $c>0$ and replacing $\beta$ by $\beta/c$ leaves all choice probabilities unchanged. Choice data alone cannot identify both scales. What appears to be low [reward](../../../reward.md) valuation may instead be noisy choice, a representation difference or a poorly specified task. [Parameter recovery](../../../parameter-recovery.md), independent measurements, alternative-model comparison and predictions for new conditions are therefore necessary.

Finally, [psychopathology](../../../psychopathology.md) involves suffering, impairment, bodily state, development and social circumstances. The same observed withdrawal can be adaptive in a dangerous environment and disabling elsewhere. A mathematical objective does not decide whose goals matter or whether a preference warrants clinical concern. Accounts must incorporate the person's history and meaning, ascertain distress and functional impact, and test feasible interventions. **The strongest explanation combines formal constraints with biological and behavioural evidence and a contextual [clinical formulation](../../../clinical-formulation.md); a compact equation is a tool, not a diagnosis.**

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2022](../../2022-split.md)
3. [Past exam of the learning theory: memory, cognition and psychopathology course of the University of Oxford](../../split.md)
4. [Learning theory: memory, cognition and psychopathology course of the University of Oxford](../../../learning-theory-memory-cognition-and-psychopathology-course-of-the-university-of-oxford.md)
5. [Year 3 of the psychology (experimental) course of the University of Oxford](../../../year-3-of-the-psychology-experimental-course-of-the-university-of-oxford.md)
6. [Psychology (experimental) course of the University of Oxford](../../../psychology-experimental-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
