<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

This is a [safety property](../../../../../safety-property.md): a bad shutdown or a later reactivation has a finite bad [CSP trace](../../../../../csp-trace.md). Use the [CSP traces model](../../../../../csp-traces-model.md). Let $V=\{0,\ldots,N-1\}$, let $A\subseteq V$ track active nodes, and let $D\subseteq V$ track nodes that have announced shutdown. Let $\mathrm{Ring}$ contain every message [CSP event](../../../../../csp-event.md). Define the following specification over the status-signal alphabet:

$$
\begin{aligned}
\mathrm{Safe}(A,D)
&=\mathop{\square}_{n\in A\setminus D}\mathit{idle}.n\to\mathrm{Safe}(A\setminus\{n\},D)\\
&\quad\mathbin\square\mathop{\square}_{\substack{n\in V\setminus(A\cup D)\\D=\varnothing}}\mathit{active}.n\to\mathrm{Safe}(A\cup\{n\},D)\\
&\quad\mathbin\square\mathop{\square}_{\substack{n\in V\setminus D\\A=\varnothing}}\mathit{shutdown}.n\to\mathrm{Safe}(A,D\cup\{n\}).
\end{aligned}
$$

Use the [CSP refinement](../../../../../csp-refinement.md) check

$$
\boxed{\mathrm{Safe}(V,\varnothing)\sqsubseteq_T\mathrm{System}\setminus\mathrm{Ring}.}
$$

The specification offers a shutdown only if the active set is empty, and offers no activation once $D$ is nonempty. A trace violating either requirement is therefore absent from the specification. Recording $D$ also prevents duplicate shutdowns and any status change by an already shut-down node. [CSP hiding](../../../../../csp-hiding.md) removes message details irrelevant to this finite bad-prefix check; a [CSP traces model](../../../../../csp-traces-model.md) check alone does not assert eventual progress.

The system satisfies the check. After the first message has passed nodes $1,\ldots,i$, its bit is the [Boolean conjunction](../../../../../logical-conjunction.md) of their being idle when sampled. Every sampled node is then frozen until it forwards the second-round decision. A true bit returning to node $0$ therefore means that every non-coordinator is idle and still frozen; the coordinator has itself remained idle. A true decision consequently reaches only idle nodes, each of which proceeds to shutdown rather than returning to $\mathrm{Free}$. No node can subsequently become active. A false decision permits no shutdown at all.

## ↑ Ancestors (11)

1. [D](../d.md)
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
