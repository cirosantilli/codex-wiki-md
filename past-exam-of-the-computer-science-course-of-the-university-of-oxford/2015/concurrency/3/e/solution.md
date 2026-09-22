<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The trigger is specifically the first-round reception $\mathit{ring}.0.\mathrm{true}$. A [CSP trace](../../../../../csp-trace.md) restriction cannot by itself guarantee progress after this event, because a finite prefix is compatible with both completion and an indefinitely delayed completion. We need to exclude both a stable refusal to continue and [CSP divergence](../../../../../csp-divergence.md), so use the [CSP failures-divergences model](../../../../../csp-failures-divergences-model.md).

Here is an explicit conditional check that imposes no progress requirement before the trigger. Build the reachable [labelled transition system](../../../../../labelled-transition-system.md) of $\mathrm{System}$ and observe coordinator rounds with a two-phase monitor: it starts in the first-return phase and toggles on each $\mathit{ring}.0.b$. Collect the set $\mathcal H$ of system derivatives immediately after a true return in the first-return phase. This distinguishes the survey's return from the decision's return, without changing any system transitions. For fixed finite $N$, the set is finite. Define

$$
\begin{aligned}
\mathrm{Shut}&=\{\mathit{shutdown}.n:n\in V\},\\
\mathrm{Post}&=\mathop{\sqcap}_{H\in\mathcal H}\left(H\setminus(\Sigma\setminus\mathrm{Shut})\right),\\
\mathrm{Finish}(D)&=\begin{cases}\mathrm{STOP},&D=V,\\\displaystyle\mathop{\sqcap}_{n\in V\setminus D}\mathit{shutdown}.n\to\mathrm{Finish}(D\cup\{n\}),&D\ne V.
\end{cases}
\end{aligned}
$$

Here $\sqcap$ denotes [CSP internal choice](../../../../../csp-internal-choice.md). Perform the single [CSP refinement](../../../../../csp-refinement.md) check

$$
\boxed{\mathrm{Finish}(\varnothing)\sqsubseteq_{FD}\mathrm{Post}.}
$$

Equivalently, check each post-trigger derivative $H$ individually against $\mathrm{Finish}(\varnothing)$ after the displayed [CSP hiding](../../../../../csp-hiding.md). If the trigger is unreachable, the conditional property is vacuously true and there is no post-trigger check to perform.

The [CSP internal choice](../../../../../csp-internal-choice.md) in $\mathrm{Finish}$ deliberately permits any next shutdown, including an implementation that offers only one of the remaining shutdowns. It forbids a stable refusal of all remaining shutdowns, has no [CSP divergence](../../../../../csp-divergence.md), and permits at most $N$ distinct shutdowns before $\mathrm{STOP}$. A [CSP external choice](../../../../../csp-external-choice.md) over all remaining nodes would instead demand simultaneous readiness for every remaining shutdown and would unnecessarily reject the protocol's sequential delivery.

After hiding all other actions, endless internal work becomes a [CSP divergence](../../../../../csp-divergence.md) and a blocked unfinished state becomes a forbidden [CSP stable failure](../../../../../csp-stable-failure.md). Since there are only $N$ possible shutdown actions and duplicates are excluded by [CSP traces](../../../../../csp-trace.md), every maximal progressing execution must complete all $N$. As usual for untimed CSP, this progress claim assumes the environment allows shutdown signals to occur; it supplies no wall-clock deadline. No fairness assumption requiring the coordinator eventually to initiate a survey has been smuggled into this conditional check.

For the defined system the check succeeds. Immediately after the trigger all statuses are idle and frozen. The only message work left is the second round: node $0$ sends the decision to node $1$, nodes $1$ through $N-1$ forward it, and node $0$ receives it. These are exactly $N$ more message transfers. Each node then has its one shutdown action, and the message can advance even while an earlier node's shutdown is pending. Thus there are no remaining status changes, no message cycle, and no unfinished global state in which every action is blocked. The measure

$$
\boxed{\text{remaining second-round transfers}+\text{remaining shutdown signals}}
$$

starts at $2N$, is nonnegative, and decreases on every subsequent transition. This excludes any hidden infinite run; before all shutdowns finish there is either an enabled message transfer or an enabled shutdown signal. The operational argument proves the conditional claim for every $N\geq2$; finite state enumeration is only a supporting check.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Concurrency](../../../concurrency-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
