# Strong planning winning-set iteration

↑ **Parent:** [Strong plan](strong-plan.md)

For a finite [nondeterministic planning](nondeterministic-planning.md) problem with goal [set](set-split.md) $G$, initialize $W_0=G$ and put

$$
W_{t+1}=W_t\cup\{s:\exists a,\ \varnothing\ne\operatorname{Results}(s,a)\subseteq W_t\}.
$$

A state in $W_t$ has a [strong plan](strong-plan.md) reaching $G$ within $t$ steps. The proof is [mathematical induction](mathematical-induction.md): an action witnessing admission to $W_{t+1}$ has only successors with plans of depth at most $t$. Conversely, the first action of any guaranteed plan of depth $t+1$ has every successor in $W_t$, again by [mathematical induction](mathematical-induction.md). Since $W_t$ only grows inside a finite [state space](state-space.md), the iteration stabilizes after at most the number of states many strict expansions. Recording a witnessing action at first admission gives a policy whose rank decreases at every nonterminal step.

## ↑ Ancestors (6)

1. [Strong plan](strong-plan.md)
2. [Nondeterministic planning](nondeterministic-planning.md)
3. [Automated planning](automated-planning.md)
4. [Artificial intelligence](artificial-intelligence-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/2/g/solution.md)
- [Strong plan](strong-plan.md)
