<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use fresh event tags to tell apart an action by $P$ and an interrupting action by $Q$. Put $B=\Sigma\setminus A$ and introduce a disjoint copy $B'=\{a':a\in B\}$. Let $f$ fix $A$ and map each $a\in B$ to $a'$, and put $S=A\cup B'$. Define a process that always accepts an event from $S$ by

$$
\mathrm{RUN}(S)=\mathop{\square}_{x\in S}x\to\mathrm{RUN}(S),
$$

and an ordinary [CSP interrupt](../../../../../csp-interrupt.md) handler by

$$
I=\mathop{\square}_{a\in B}a'\to\mathrm{RUN}(S).
$$

Finally let $g$ fix every original event and send $a'$ back to $a$. A simulation containing no occurrence of the new operator is

$$
\boxed{R=g\left((P\mathbin\triangle I)\underset S\Vert f(Q)\right).}
$$

Here $\triangle$ is the ordinary [CSP interrupt](../../../../../csp-interrupt.md), and the [CSP event renaming](../../../../../csp-event-renaming.md) $g$ is applied after the [CSP parallel composition](../../../../../csp-parallel-composition.md). It is non-injective, so part (c) explains why moving it inside would be unsafe.

Before the interrupt, $P$'s events in $A$ synchronize with $f(Q)$ on the same events. Its events outside $A$ are unprimed and do not synchronize with $f(Q)$. Meanwhile $Q$'s events outside $A$ are primed; they synchronize with $I$ and thereby interrupt and discard $P$. After the first such event, the left operand is $\mathrm{RUN}(S)$, so it imposes no further restriction on $f(Q)$; final [CSP event renaming](../../../../../csp-event-renaming.md) then yields exactly the remaining behaviour of $Q$.

For a formal [strong bisimulation](../../../../../strong-bisimulation.md), relate a pre-interrupt state $J_A(P_0,Q_0)$ to

$$
g\left((P_0\mathbin\triangle I)\underset S\Vert f(Q_0)\right),
$$

and an already-interrupted state $Q_0$ to

$$
g\left(\mathrm{RUN}(S)\underset S\Vert f(Q_0)\right).
$$

The three visible cases match the rules in part (d), including both transitions when both operands offer the same event outside $A$. A [CSP internal action](../../../../../csp-internal-action.md) of $Q_0$ never activates $I$, while a [CSP internal action](../../../../../csp-internal-action.md) of $P_0$ remains possible exactly until the interrupt. The controller adds no [CSP internal actions](../../../../../csp-internal-action.md). Thus transitions match in both directions and related derivatives remain related.

Consequently this simulation is stronger than merely [CSP trace](../../../../../csp-trace.md) equivalent:

$$
\boxed{R=_T J_A(P,Q),\qquad R=_F J_A(P,Q),\qquad R=_{FD}J_A(P,Q).}
$$

It preserves [CSP stable states](../../../../../csp-stable-state.md), their enabled-event sets and their [CSP stable failures](../../../../../csp-stable-failure.md), and matches every possible infinite run of [CSP internal actions](../../../../../csp-internal-action.md). In particular, it introduces neither a premature commitment nor a new [CSP divergence](../../../../../csp-divergence.md). A different simulation that guesses an interrupt with a hidden handshake would need a separate refusal analysis; the visible tagging construction above needs no hidden handshake.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Concurrency](../../../concurrency-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
