<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First define the ordinary unbounded [FIFO buffer](../../../../../fifo-buffer.md):

$$
\begin{aligned}
\mathrm{BUF}(q)&=\bigl(\mathit{left}?x:T\to\mathrm{BUF}(q\mathbin{\frown}\langle x\rangle)\bigr)\\
&\quad\mathbin\square\begin{cases}\mathrm{STOP},&q=\langle\rangle,\\\mathit{right}.\operatorname{head}(q)\to\mathrm{BUF}(\operatorname{tail}(q)),&q\ne\langle\rangle.\end{cases}
\end{aligned}
$$

Now use [CSP internal choice](../../../../../csp-internal-choice.md) to permit an immediate stop:

$$
\boxed{P=\mathrm{BUF}(\langle\rangle)\sqcap\mathrm{STOP}.}
$$

An execution choosing the first branch can perform every legal [CSP trace](../../../../../csp-trace.md) satisfying the [prefix of a list](../../../../../prefix-of-a-list.md) condition in part (a). Conversely that condition excludes all other [CSP traces](../../../../../csp-trace.md), so no process satisfying it can have more [CSP traces](../../../../../csp-trace.md). The second branch adds no new [CSP trace](../../../../../csp-trace.md), since the empty [CSP trace](../../../../../csp-trace.md) is already present.

The second branch does add the [CSP stable failure](../../../../../csp-stable-failure.md) $(\langle\rangle,\{\mathit{left}.x\})$ for any $x\in T$. This violates mandatory input readiness. Therefore the process has the maximum possible [CSP trace](../../../../../csp-trace.md) set and fails the [CSP stable failure](../../../../../csp-stable-failure.md) specification. The qualification is $T\ne\varnothing$, as is implicit for a useful [FIFO buffer](../../../../../fifo-buffer.md); with an empty value type there is no input-readiness event to violate. Maximizing the number of [CSP traces](../../../../../csp-trace.md) does not pick a unique process in the finer models: other processes with the same complete legal [CSP trace](../../../../../csp-trace.md) set and extra refusals also qualify.

## ↑ Ancestors (11)

1. [B](../b.md)
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
