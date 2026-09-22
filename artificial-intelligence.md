# Artificial intelligence

↑ **Parent:** [Computer science](computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Artificial_intelligence)

**Table of contents**

- [Planning](#planning)
- [World model](#world-model)
- [Neuro-symbolic artificial intelligence](#neuro-symbolic-artificial-intelligence)
- [Symbol grounding](#symbol-grounding)
- [Subsymbolic computation](#subsymbolic-computation)
- [Symbolic computation](#symbolic-computation)
  - [Physical symbol system hypothesis](#physical-symbol-system-hypothesis)
- [Intelligent agent](#intelligent-agent)
- [Planning fluent](#planning-fluent)
- [STRIPS](#strips)
  - [Precondition-free STRIPS planning](#precondition-free-strips-planning)
    - [Last-achiever algorithm for precondition-free planning](#last-achiever-algorithm-for-precondition-free-planning)
  - [Action schema](#action-schema)
    - [Ground action](#ground-action)
      - [Action grounding](#action-grounding)
  - [Static predicate](#static-predicate)
- [Automated planning](#automated-planning)
  - [Plan](#plan)
  - [Nondeterministic planning](#nondeterministic-planning)
    - [Strong plan](#strong-plan)
      - [Strong planning winning-set iteration](#strong-planning-winning-set-iteration)
  - [Contingent planning](#contingent-planning)
  - [Classical planning](#classical-planning)
    - [Goal interaction in planning](#goal-interaction-in-planning)
      - [Sussman anomaly](#sussman-anomaly)
      - [Goal-by-goal planning](#goal-by-goal-planning)
    - [Blocks world](#blocks-world)
    - [Goal regression](#goal-regression)
    - [Frame axiom](#frame-axiom)
    - [Successor-state axiom](#successor-state-axiom)
    - [SATPlan](#satplan)
      - [Sequential SATPlan correctness](#sequential-satplan-correctness)
      - [Action exclusion axiom](#action-exclusion-axiom)
      - [Action precondition axiom](#action-precondition-axiom)
      - [Planning horizon](#planning-horizon)
    - [Forward state-space planning](#forward-state-space-planning)
- [Machine learning](#machine-learning)
  - [Deep learning](#deep-learning)
  - [Statistical classification](#statistical-classification)
    - [Positive predictive value](#positive-predictive-value)

## Planning

↑ **Parent:** [Artificial intelligence](artificial-intelligence.md)

Computing or comparing sequences of actions using representations of their expected consequences and relevant constraints. A plan can be revised after a goal, transition or inferred state changes. [Planning](#planning) is distinct from merely evaluating one fixed control policy or repeating a cached response.

## World model

↑ **Parent:** [Artificial intelligence](artificial-intelligence.md)

An internal model of relationships among states, actions, observations and outcomes, used to predict consequences or support inference. It can be incomplete and task-specific. [Planning](#planning) through a mistaken model can produce confident errors, so model accuracy and the choice of abstraction are part of intelligent control.

## Neuro-symbolic artificial intelligence

↑ **Parent:** [Artificial intelligence](artificial-intelligence.md)

Approaches combining learned [neural representations](neuroscience.md#neural-representation) or computations with explicit structured representations and reasoning. A useful account specifies the interface, uncertainty and learning responsibilities of the components rather than assuming their combination automatically supplies general intelligence.

## Symbol grounding

↑ **Parent:** [Artificial intelligence](artificial-intelligence.md)

The problem of connecting internal symbols to what they designate in perception, action or other meaningful relations. Supplying an [intelligent agent](#intelligent-agent) with perfectly identified objects and relations can conceal this problem rather than solve it.

## Subsymbolic computation

↑ **Parent:** [Artificial intelligence](artificial-intelligence.md)

Computation over quantities such as distributed activation patterns and learned weights, without requiring every meaningful entity to occupy a separate explicit token. [Neural networks](statistical-learning.md#neural-network) are common examples. A distributed implementation can nevertheless learn or implement structured operations.

## Symbolic computation

↑ **Parent:** [Artificial intelligence](artificial-intelligence.md)

Computation using explicitly structured representations whose elements have identifiable roles, with rules or procedures acting on those structures. Logical [planning](#planning) is an example. This sense concerns symbolic cognitive architectures rather than only computer algebra; it can be implemented by different physical substrates.

### Physical symbol system hypothesis

↑ **Parent:** [Symbolic computation](#symbolic-computation)

A proposal that structured symbolic representation and manipulation provide a basis for general intelligent action. It is a claim about computation to be evaluated empirically, rather than a mathematical theorem equating every particular symbolic program with intelligence.[Communications of the ACM 19, pp. 113–126, physical symbol systems and search](computer-science-bibliography.md#computer-science-as-empirical-inquiry-symbols-and-search-by-allen-newell-and-others)

## Intelligent agent

↑ **Parent:** [Artificial intelligence](artificial-intelligence.md)

A system that uses observations and internal information to choose actions in an environment in pursuit of specified or learned objectives. Assessing intelligence requires stating the tasks, available experience, uncertainty and resource constraints; a useful internal representation is part of the problem, not automatically supplied by the environment.

## Planning fluent

↑ **Parent:** [Artificial intelligence](artificial-intelligence.md)

A fact whose truth can change as actions execute in [automated planning](#automated-planning). Ground location facts and an empty-container marker are examples. In [STRIPS](#strips), static facts such as an object's fixed type are never added or deleted, while [planning fluents](#planning-fluent) can appear in action effects.

## STRIPS

↑ **Parent:** [Artificial intelligence](artificial-intelligence.md)

A representation for [automated planning](#automated-planning) in which a state $S$ is a [set](set.md) of true ground facts and an action has a positive [precondition](algorithm.md#precondition) set $P$, add set $A$ and delete set $D$. Under the [closed-world assumption](mathematical-logic.md#closed-world-assumption), facts absent from $S$ are false. The action applies when $P\subseteq S$ and produces

$$
S'=(S\setminus D)\cup A.
$$

Negative effects are delete-list entries; they do not require negative [preconditions](algorithm.md#precondition). A movement action must delete an object's old location as well as add its destination. Capacity and safety restrictions require explicit action conditions or auxiliary [planning fluents](#planning-fluent); they do not follow automatically from an intended physical interpretation.

### Precondition-free STRIPS planning

↑ **Parent:** [STRIPS](#strips)

[Automated planning](#automated-planning) with [ground actions](#ground-action) that are always applicable because their [precondition](algorithm.md#precondition) sets are empty. Delete effects are still permitted, so taking the union of all add effects does not decide reachability. With a positive conjunctive goal, the [last-achiever algorithm for precondition-free planning](#last-achiever-algorithm-for-precondition-free-planning) gives a [polynomial-time algorithm](theoretical-computer-science.md#polynomial-time-algorithm).

#### Last-achiever algorithm for precondition-free planning

↑ **Parent:** [Precondition-free STRIPS planning](#precondition-free-strips-planning)

Start with required facts $R=G$. If $R\subseteq I$, the empty prefix suffices. Otherwise choose an action adding a member of $R$ and deleting none of $R$, record it as a final action, and remove its add effects from $R$. Repeat and reverse the recorded actions when the residual requirements hold initially. Reject if no permitted action exists.

Soundness follows because each recorded last action supplies its removed requirements without deleting the remaining ones. If a [plan](#plan) satisfies a residual $R$ not contained in $I$, its last action affecting $R$ cannot delete an $R$-fact and must add one; therefore a candidate exists. Any selected candidate leaves a smaller required set, which is no harder to achieve than $R$. This proves completeness by [mathematical induction](foundations-of-mathematics.md#mathematical-induction). Every selection removes a required fact, so there are at most $|G|$ selections and a scan of all effect lists at each step gives [polynomial time](theoretical-computer-science.md#polynomial-time).

### Action schema

↑ **Parent:** [STRIPS](#strips)

A parameterized action definition with typed parameters, [preconditions](algorithm.md#precondition), add effects and delete effects. Replacing its parameters by type-correct objects yields a [ground action](#ground-action). Type restrictions and static inequalities can remove invalid instantiations before the action is considered by a [search algorithm](algorithm.md#search-algorithm) or [SATPlan](#satplan).

#### Ground action

↑ **Parent:** [Action schema](#action-schema)

An action with no unbound object [variables](mathematics.md#variable-mathematics). Its [precondition](algorithm.md#precondition) and effect sets consist of fixed ground facts. [Action grounding](#action-grounding) an [action schema](#action-schema) over a finite object universe creates one candidate action for each type-correct parameter tuple, after any static filtering; a time-indexed encoding then creates copies or [variables](mathematics.md#variable-mathematics) for individual action occurrences.

##### Action grounding

↑ **Parent:** [Ground action](#ground-action)

Substituting object names for all parameters in an [action schema](#action-schema), retaining the type-correct tuples and any required static restrictions. The result is a collection of [ground actions](#ground-action).

### Static predicate

↑ **Parent:** [STRIPS](#strips)

A predicate whose ground facts are unchanged by every action in a [planning](#planning) model. Object types and a fixed adjacency relation are common examples. Static conditions can filter [ground actions](#ground-action) before search; they need not acquire a separate truth [variable](mathematics.md#variable-mathematics) at every time layer. A [planning fluent](#planning-fluent) can instead be added or deleted by actions.

## Automated planning

↑ **Parent:** [Artificial intelligence](artificial-intelligence.md)

Constructing a sequence of actions whose successive applications transform a specified initial state into one satisfying a goal. The formal model must specify action [preconditions](algorithm.md#precondition), state changes and the meaning of facts absent from a state. [STRIPS](#strips) represents changes by add and delete lists; [planning state invariants](algorithm.md#planning-state-invariant) explain which physical properties the action definitions preserve.

### Plan

↑ **Parent:** [Automated planning](#automated-planning)

In deterministic [classical planning](#classical-planning), a finite sequence of actions applicable successively from the initial state and ending in a state satisfying the goal. A [STRIPS](#strips) [plan](#plan) must respect every action's [precondition](algorithm.md#precondition) set and both add and delete effects. A numerical bound on a possible [plan](#plan)'s cost does not itself specify the action sequence.

### Nondeterministic planning

↑ **Parent:** [Automated planning](#automated-planning)

[Automated planning](#automated-planning) with several possible successors for an action and no specified [probabilities](probability-theory.md#probability) for choosing between them. A plan must say how to act after observed outcomes. A [strong plan](#strong-plan) guarantees eventual success for every possible outcome history; a favorable outcome on just one branch does not establish that guarantee.

#### Strong plan

↑ **Parent:** [Nondeterministic planning](#nondeterministic-planning)

A plan or policy that reaches a goal after finitely many steps under every permitted outcome sequence. In a finite [state space](dynamical-systems.md#state-space) with finite outcome [sets](set.md), a terminating finitely branching plan tree has bounded depth. [Strong planning winning-set iteration](#strong-planning-winning-set-iteration) constructs exactly the states from which such finite guaranteed-success plans exist. A repeated state cannot be accepted merely because repeated attempts might eventually succeed: without a fairness or [probability](probability-theory.md#probability) assumption, an unfavorable outcome can recur forever.

##### Strong planning winning-set iteration

↑ **Parent:** [Strong plan](#strong-plan)

For a finite [nondeterministic planning](#nondeterministic-planning) problem with goal [set](set.md) $G$, initialize $W_0=G$ and put

$$
W_{t+1}=W_t\cup\{s:\exists a,\ \varnothing\ne\operatorname{Results}(s,a)\subseteq W_t\}.
$$

A state in $W_t$ has a [strong plan](#strong-plan) reaching $G$ within $t$ steps. The proof is [mathematical induction](foundations-of-mathematics.md#mathematical-induction): an action witnessing admission to $W_{t+1}$ has only successors with plans of depth at most $t$. Conversely, the first action of any guaranteed plan of depth $t+1$ has every successor in $W_t$, again by [mathematical induction](foundations-of-mathematics.md#mathematical-induction). Since $W_t$ only grows inside a finite [state space](dynamical-systems.md#state-space), the iteration stabilizes after at most the number of states many strict expansions. Recording a witnessing action at first admission gives a policy whose rank decreases at every nonterminal step.

### Contingent planning

↑ **Parent:** [Automated planning](#automated-planning)

[Automated planning](#automated-planning) whose result may branch on information revealed during execution. In [partially observable search](theoretical-computer-science.md#partially-observable-search), an [AND-OR search](algorithm.md#and-or-search) chooses an action at each OR node and requires a continuation for each possible observation at its AND branches. A contingent plan can therefore be a conditional tree or a policy on [belief states](theoretical-computer-science.md#belief-state), rather than one fixed action sequence.

### Classical planning

↑ **Parent:** [Automated planning](#automated-planning)

[Automated planning](#automated-planning) with a completely specified initial state, deterministic actions and a goal condition. A finite [STRIPS](#strips) model is a common representation. A plan is an action sequence applicable from the initial state, ending in a goal state. Unknown facts about the initial world require an epistemic representation such as a [belief state](theoretical-computer-science.md#belief-state), rather than silently interpreting every unlisted fact as false.

#### Goal interaction in planning

↑ **Parent:** [Classical planning](#classical-planning)

Two subgoals interact when actions needed for one can establish, obstruct or delete facts needed for the other. A [plan](#plan) for each subgoal separately need not combine into a [plan](#plan) for their [conjunction](planetary-science.md#conjunction-astronomy). Preparing the world before committing to a subgoal, revising an earlier subplan or temporarily undoing an achieved fact can all be necessary. [Goal-by-goal planning](#goal-by-goal-planning) may therefore be incomplete.

##### Sussman anomaly

↑ **Parent:** [Goal interaction in planning](#goal-interaction-in-planning)

The [Sussman anomaly](#sussman-anomaly) is a [blocks world](#blocks-world) example in which independently constructing the obvious subplans for two stacking goals gives destructive [goal interaction in planning](#goal-interaction-in-planning). Clearing a block in advance allows a short joint [plan](#plan), while prematurely achieving either isolated goal can block the other. It demonstrates the inadequacy of restricted [goal-by-goal planning](#goal-by-goal-planning), rather than a prohibition on every possible ordering of final goal achievements. Preparatory actions can make such an ordering succeed. For a concrete instance, start with $C$ on $A$ and $A,B$ on the table, and require $A$ on $B$ and $B$ on $C$. Moving $C$ to the table, then $B$ onto $C$, then $A$ onto $B$ succeeds. The first move is preparation that an isolated shortest subplan for the second stacking goal would omit.

##### Goal-by-goal planning

↑ **Parent:** [Goal interaction in planning](#goal-interaction-in-planning)

A restricted [goal-by-goal planning](#goal-by-goal-planning) procedure chooses one subgoal, constructs a subplan for it without preparation motivated by other pending subgoals, then moves on while treating the earlier goal as protected. Destructive [goal interaction in planning](#goal-interaction-in-planning) can defeat either ordering. Merely requiring the final [plan](#plan) to be a concatenation of subplans is a weaker condition: a subplan may already contain preparatory work useful to a later goal. A claimed impossibility must specify the stronger restriction rather than infer it from concatenation alone.

#### Blocks world

↑ **Parent:** [Classical planning](#classical-planning)

The [blocks world](#blocks-world) is a [classical planning](#classical-planning) model of movable blocks arranged in stacks on an unlimited table. Each block has one support, each block supports at most one other block, and the support relation has no [directed cycle](graph-theory.md#directed-cycle). A clear block can move onto another clear block or onto the table. In a direct-transfer [STRIPS](#strips) representation, an action includes the entire pickup-and-placement operation; a separate holding or empty-hand [planning fluent](#planning-fluent) is unnecessary unless the action model explicitly splits those operations.

The table has unlimited capacity, so its availability must not be deleted when a block is placed there. [Planning state invariants](algorithm.md#planning-state-invariant) connect the [predicate](analysis-of-boolean-functions.md#predicate) describing a clear block to the absence of any block directly above it. [Goal interaction in planning](#goal-interaction-in-planning) makes this small model useful for testing [automated planning](#automated-planning) methods.

#### Goal regression

↑ **Parent:** [Classical planning](#classical-planning)

For a positive conjunctive goal $G$, an action with $\operatorname{Del}(a)\cap G=\varnothing$ can serve as the final step. Before it executes, the remaining goals and its [preconditions](algorithm.md#precondition) must hold, giving the displayed regressed set. For [precondition-free STRIPS planning](#precondition-free-strips-planning), only deletion of already supplied requirements remains.

#### Frame axiom

↑ **Parent:** [Classical planning](#classical-planning)

A condition specifying when a fact remains unchanged by an action. In [STRIPS](#strips), facts outside the add and delete lists persist. A [successor-state axiom](#successor-state-axiom) combines these persistence conditions with all action effects that can change the fact.

#### Successor-state axiom

↑ **Parent:** [Classical planning](#classical-planning)

A logical equivalence characterizing exactly when a [planning fluent](#planning-fluent) is true after one step. Here $\operatorname{Add}_F$ and $\operatorname{Delete}_F$ are disjunctions of selected actions with the respective effects, under a suitable action-conflict policy. The persistence term excludes spontaneous changes and captures the relevant [frame axiom](#frame-axiom). An implication from add effects alone would not constrain all other state changes.

#### SATPlan

↑ **Parent:** [Classical planning](#classical-planning)

An approach to [automated planning](#automated-planning) that constructs a [Boolean satisfiability problem](theoretical-computer-science.md#boolean-satisfiability-problem) for a bounded [planning horizon](#planning-horizon), solves it and decodes a satisfying assignment into a [plan](#plan). A typical encoding has time-indexed action occurrences and [planning fluents](#planning-fluent), initial and goal clauses, [action precondition axioms](#action-precondition-axiom), state-transition constraints and [action exclusion axioms](#action-exclusion-axiom). Sequential and parallel encodings have different notions of a step.

[Henry Kautz](computer-science.md#henry-kautz) and [Bart Selman](computer-science.md#bart-selman) introduced [planning](#planning) as satisfiability in their 1992 paper.[ECAI 1992, pp. 359–363; publication listed in the author's Cornell bibliography](computer-science-bibliography.md#planning-as-satisfiability-by-henry-kautz-and-bart-selman)

##### Sequential SATPlan correctness

↑ **Parent:** [SATPlan](#satplan)

A sequential [SATPlan](#satplan) encoding has a complete initial assignment of [planning fluents](#planning-fluent), final goal constraints, [action precondition axioms](#action-precondition-axiom), [successor-state axioms](#successor-state-axiom) and [action exclusion axioms](#action-exclusion-axiom) allowing at most one action per layer. Zero selected actions is an idle step: the [successor-state axioms](#successor-state-axiom) preserve all facts. This encodes an upper bound on [plan](#plan) length rather than forcing exactly $T$ physical actions.

For soundness, read selected [ground actions](#ground-action) in layer order. The initial assignment is the real initial state. By [mathematical induction](foundations-of-mathematics.md#mathematical-induction), each selected action has its [preconditions](algorithm.md#precondition) in the current state and the [successor-state axioms](#successor-state-axiom) give precisely its add/delete update; an empty layer leaves that state unchanged. The final goal constraint therefore proves that the decoded [plan](#plan) succeeds. Conversely, take any [plan](#plan) of length at most $T$, assign its actual state trajectory to the fluent [variables](mathematics.md#variable-mathematics), select its actions in successive layers and pad with idle layers. All encoding components hold. Complete initial negations and persistence conditions are essential: omitting either can introduce unsupported facts and spurious [plans](#plan).

##### Action exclusion axiom

↑ **Parent:** [SATPlan](#satplan)

A condition forbidding a conflicting pair of action occurrences in one layer. A serial [SATPlan](#satplan) encoding excludes every distinct pair; parallel encodings exclude the pairs disallowed by their concurrency semantics. Excluding two simultaneous pickups can enforce a one-hand resource restriction even if both individual [precondition](algorithm.md#precondition) sets hold.

##### Action precondition axiom

↑ **Parent:** [SATPlan](#satplan)

A clause or formula ensuring a selected action occurrence has all of its [preconditions](algorithm.md#precondition) satisfied at the current time. It is one part of a [plan](#plan) encoding; action effects, persistence, initial conditions and goals require additional constraints.

##### Planning horizon

↑ **Parent:** [SATPlan](#satplan)

The number of action layers allowed in a bounded [automated planning](#automated-planning) encoding. Sequential layers permit at most one physical action, while a parallel semantics may permit several compatible actions. A sufficiently large horizon guarantees finding a solution only for a solvable input; shorter [plans](#plan) require idle layers or testing the successive smaller horizons.

#### Forward state-space planning

↑ **Parent:** [Classical planning](#classical-planning)

Expand a concrete state by applying every action whose [preconditions](algorithm.md#precondition) hold, and search the resulting state [graph](graph.md) for a goal. For [STRIPS](#strips), the successor is $(S\setminus\operatorname{Del}(a))\cup\operatorname{Add}(a)$. A valid expansion checks the complete [precondition](algorithm.md#precondition) set, including resource markers such as an empty hand, rather than only an action's geometric destination.

## Machine learning

↑ **Parent:** [Artificial intelligence](artificial-intelligence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Machine_learning)

[Machine learning](#machine-learning) develops computational methods whose behaviour is learned from data. [Statistical learning](statistical-learning.md) supplies methods for reasoning about prediction, uncertainty and generalization.

### Deep learning

↑ **Parent:** [Machine learning](#machine-learning)

Learning with multiple stages of representation, typically implemented by a [neural network](statistical-learning.md#neural-network). Depth, connectivity, objective, training experience and parameter sharing are distinct design choices; a deep architecture need not be convolutional or supervised.

### Statistical classification

↑ **Parent:** [Machine learning](#machine-learning)

Assignment of observations to categories using measured features and a statistical rule. In geological [remote sensing](radiometry.md#remote-sensing), features can be multispectral pixel values or derived [spectral reflectance](radiometry.md#spectral-reflectance) ratios; known field samples provide training labels and independent observations assess errors. Classification boundaries need not coincide with [lithological contacts](planetary-science.md#lithological-contact) when illumination or cover dominates the signal.

#### Positive predictive value

↑ **Parent:** [Statistical classification](#statistical-classification)

For a binary [classifier](foundations-of-mathematics.md#classifier), the [conditional probability](probability-theory.md#conditional-probability) of the target condition given a positive classification. If its [base rate](bayesian-statistics.md#base-rate) is $p$, its true-positive [probability](probability-theory.md#probability) is $s$, and its false-positive [probability](probability-theory.md#probability) is $f$, [Bayes' theorem](probability-theory.md#bayes-theorem) gives $P(E\mid +)=sp/(sp+f(1-p))$. The denominator is positive whenever a positive classification can occur.

## ↑ Ancestors (2)

1. [Computer science](computer-science.md)
2. [Codex Wiki](README.md)

## ← Incoming links (2)

- [Peter Norvig](computer-science.md#peter-norvig)
- [Stuart J. Russell](computer-science.md#stuart-j-russell)
