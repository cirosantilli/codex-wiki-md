<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

This is a **finite, discrete, partially observable, single-agent, sequential [search problem](../../../../../search-problem.md) with an unknown initial state**. The cave is static while the agent deliberates. Given a complete world and an action, the described physical effects and ideal sensor readings are deterministic; ignorance of the world does not itself supply a [probability distribution](../../../../../probability-distribution-split.md). The fixed monster and gold are environmental objects, not competing decision makers. A known action/sensor law with unknown object locations is different from having to learn an unknown [search transition model](../../../../../search-transition-model.md).

Use [partially observable search](../../../../../partially-observable-search.md) over [belief states](../../../../../belief-state.md). A complete physical state can be written

$$
s=(p,m,P,g,\ell,r,k,e),
$$

where $p$ is the agent’s room, $m$ the fixed monster room, $P$ the pit [set](../../../../../set-split.md), $g$ the fixed gold room, $\ell$ records whether the monster lives, $r$ whether the arrow remains, $k$ whether gold has been collected and $e$ whether the agent has exited or failed. The known room dimensions and exit are fixed data. Include death or entrapment as failure states. Movement, shooting toward an adjacent room, collection and departure have their physical meanings. In particular, a shot consumes the arrow, and kills the monster exactly when it targets the live monster’s room.

Let $T(s,a)$ be this physical [search transition model](../../../../../search-transition-model.md). For a surviving agent, an ideal observation is the tuple of three [truth values](../../../../../truth-value.md)

$$
O(s)=\bigl(\mathbf1_{\{\ell\ \text{and}\ m\sim p\}},\ \mathbf1_{\{\exists q\in P:q\sim p\}},\ \mathbf1_{\{p=g\ \text{and}\ k=0\}}\bigr),
$$

recording sound, breeze and glitter. Here $\sim$ denotes geometric adjacency and $\mathbf1$ an [indicator function](../../../../../indicator-function.md). Initially $B_0$ contains all worlds compatible with the known facts and any initial observation. After action $a$ and observation $o$, update the [belief state](../../../../../belief-state.md) by

$$
\boxed{B'_{a,o}=\{T(s,a):s\in B,\ O(T(s,a))=o\}.}
$$

Known success or failure observations are included as needed. No prior [probabilities](../../../../../probability.md) are required. A guaranteed-success [goal test](../../../../../goal-test.md) accepts $B$ only when every $s\in B$ has exited carrying gold. A policy must use the same action in all worlds still indistinguishable to the agent.

An [AND-OR search](../../../../../and-or-search.md) has OR choices for the agent’s next action and AND branches for every possible resulting observation with nonempty $B'_{a,o}$. Its output is a [contingent plan](../../../../../contingent-planning.md), not merely a route. To demand safe success, reject any action whose possible outcomes include irreversible death or entrapment, and require a successful continuation on every observation branch. In an online execution the agent updates its [belief state](../../../../../belief-state.md), follows the observation branch and can plan again. A [strong plan](../../../../../strong-plan.md) need not exist: some admissible worlds have no safe route, and even solvable worlds can be observationally indistinguishable until a dangerous choice. Without an added prior and numerical rewards, expected-risk optimization is not determined by the description.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
