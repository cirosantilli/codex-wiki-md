<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $A$ be a finite set of alternatives with $|A|\geq3$, and let each agent report a [strict total order](../../../../../strict-total-order.md) on $A$. A profile is the tuple of these orders. The domain is unrestricted: every tuple of orders is allowed. A deterministic [social choice function](../../../../../social-choice-function.md) $f$ selects one alternative from each profile. It is onto if every alternative is selected at some profile. It is [strategyproof](../../../../../strategyproofness.md) if no agent, holding all other reports fixed, can obtain an outcome strictly preferred according to its true order by reporting another order. A [dictatorship in social choice](../../../../../dictatorship-in-social-choice.md) means that one fixed agent's highest-ranked alternative is always selected, regardless of all other reports.

The **[Gibbard-Satterthwaite theorem](../../../../../gibbard-satterthwaite-theorem.md)** says that every onto, deterministic [strategyproof](../../../../../strategyproofness.md) [social choice function](../../../../../social-choice-function.md) on this unrestricted domain is a [dictatorship in social choice](../../../../../dictatorship-in-social-choice.md). Equivalently, with at least three possible alternatives an onto nondictatorial rule must permit manipulation. Both the number of alternatives and the unrestricted preference domain are essential hypotheses.

For the requested **[top-bottom decisiveness lemma](../../../../../top-bottom-decisiveness-lemma.md)**, suppose $f(R,S)=a$, with $a$ top in $R$ and bottom in $S$. Fix any $R'$ with $a$ top. If $f(R',S)\ne a$, agent $1$ with true order $R'$ could report $R$ and obtain its best outcome $a$, contrary to [strategyproofness](../../../../../strategyproofness.md). Hence $f(R',S)=a$. Now fix any $S'$. If $f(R',S')=b\ne a$, agent $2$ with true order $S$ could report $S'$ and obtain $b$, which is better than its bottom alternative $a$. Therefore

$$
\boxed{f(R',S')=a\quad\text{whenever }a\text{ is top in }R'.}
$$

Call this agent $1$ being decisive for $a$. The same argument with agents interchanged applies to agent $2$.

Here is a complete proof of the two-agent theorem. First, onto plus [strategyproofness](../../../../../strategyproofness.md) gives unanimity. If $a$ occurs at some profile, change agent $1$ to any order with $a$ top: a different outcome would allow that agent to obtain $a$ by returning to its old report. Then change agent $2$ to any order with $a$ top in the same way. Thus every profile with both agents ranking $a$ top selects $a$.

We also need [Pareto efficiency](../../../../../pareto-efficiency.md). A useful [rank-raising monotonicity lemma](../../../../../rank-raising-monotonicity-lemma.md) follows from [strategyproofness](../../../../../strategyproofness.md): if the current outcome is $b$, and one agent changes its order without placing above $b$ any alternative previously below $b$, the outcome remains $b$. Otherwise an outcome $c\ne b$ would satisfy $b\succ c$ in the old order, since a profitable deviation is forbidden there, but $c\succ' b$ in the new order, since reporting the old order is forbidden there. Those comparisons contradict the allowed change. If both agents prefer $a$ to a selected $b$, change their orders one at a time to put $a$ first and $b$ second. These changes only raise $b$ relative to other alternatives, so the outcome remains $b$, contradicting unanimity for $a$. Therefore an alternative unanimously dominated by another cannot be selected.

Choose distinct $a,b$. Give agent $1$ order $b\succ a\succ\text{the rest}$ and agent $2$ order $a\succ b\succ\text{the rest}$. [Pareto efficiency](../../../../../pareto-efficiency.md) forces the outcome to be $a$ or $b$. If it is $b$, move $b$ to the bottom of agent $2$'s order while keeping $a$ top. A switch to $a$ would be a profitable deviation for its old true order. Every other alternative is unanimously dominated by $a$. Hence the outcome stays $b$, and the [top-bottom decisiveness lemma](../../../../../top-bottom-decisiveness-lemma.md) makes agent $1$ decisive for $b$. If the outcome is $a$, the symmetric argument makes agent $2$ decisive for $a$. Consequently some agent is decisive for some alternative. Rename that agent $1$ and that alternative $a$.

Both agents cannot be decisive for this same $a$. To see this, choose $b,c\ne a$ distinct, with every remaining alternative below these three, and consider

$$
R:b\succ a\succ c,\quad R':b\succ c\succ a,\qquad S:c\succ a\succ b,\quad S':c\succ b\succ a.
$$

At $(R,S')$, agent $1$ can obtain $a$ by placing it top, so [strategyproofness](../../../../../strategyproofness.md) restricts the outcome to $a$ or $b$. Both agents prefer $b$ to $a$, so [Pareto efficiency](../../../../../pareto-efficiency.md) forces $b$. At $(R',S')$, agent $1$ still ranks $b$ top and can obtain it by reporting $R$, so the outcome must again be $b$. On the other hand, at $(R',S)$, decisiveness of agent $2$ for $a$ restricts the outcome to $a$ or $c$. Both agents prefer $c$ to $a$, so it must be $c$. Since $c$ is top in $S'$, agent $2$ can obtain it at $(R',S')$ by reporting $S$, forcing outcome $c$ there. This contradiction proves that agent $2$ is not decisive for $a$.

Now fix $b\ne a$ and any agent-$1$ order $R$ with $b$ first and $a$ second. At every $(R,S)$, agent $1$ can force $a$ by placing it top, so the outcome must lie in $\{a,b\}$. If $a$ occurs for even one report $S$, changing agent $2$ to an order with $a$ first and $b$ second preserves $a$, because it can return to $S$ to obtain its top choice. Lower $a$ to the bottom of agent $1$'s order, keeping $b$ top. A switch to $b$ would be a profitable deviation under its old order, and any other outcome is unanimously dominated by $b$. Thus $a$ remains selected at a profile where agent $2$ ranks it top and agent $1$ ranks it bottom. The [top-bottom decisiveness lemma](../../../../../top-bottom-decisiveness-lemma.md) would make agent $2$ decisive for $a$, a contradiction.

Therefore every $(R,S)$ with agent $1$ ranking $b$ first and $a$ second selects $b$. Choose $S$ with $b$ bottom and apply the [top-bottom decisiveness lemma](../../../../../top-bottom-decisiveness-lemma.md) once more: agent $1$ is decisive for $b$ in every order placing $b$ top. This holds for each $b\ne a$, and it already holds for $a$. **Agent $1$ is a [dictator in social choice](../../../../../dictator-in-social-choice.md), proving the two-agent theorem.**

With three agents and only two alternatives, **the [two-alternative majority rule](../../../../../two-alternative-majority-rule.md) is onto and [strategyproof](../../../../../strategyproofness.md) and has no [dictator in social choice](../../../../../dictator-in-social-choice.md)**. An agent whose vote is not pivotal cannot change the outcome. A pivotal agent obtains its preferred alternative by voting truthfully and its less preferred alternative by reversing its vote. No one is a [dictator in social choice](../../../../../dictator-in-social-choice.md), since the other two agents can both oppose its preference. There is no tie with three agents. This does not contradict the theorem because its hypothesis $|A|\geq3$ fails.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 212](../../paper-212-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
