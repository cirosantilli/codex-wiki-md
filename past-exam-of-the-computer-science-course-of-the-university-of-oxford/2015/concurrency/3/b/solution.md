<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The coordinator has the following states:

$$
\begin{aligned}
C_{\mathrm{active}}&=\mathit{idle}.0\to C_{\mathrm{idle}},\\
C_{\mathrm{idle}}&=\mathit{active}.0\to C_{\mathrm{active}}\mathbin\square\mathit{ring}.1.\mathrm{true}\to C_{\mathrm{first}},\\
C_{\mathrm{first}}&=\mathit{ring}.0?b:\mathrm{Bool}\to\mathit{ring}.1.b\to C_{\mathrm{return}}(b),\\
C_{\mathrm{return}}(b)&=\mathit{ring}.0.b\to\begin{cases}\mathit{shutdown}.0\to\mathrm{STOP},&b=\mathrm{true},\\C_{\mathrm{idle}},&b=\mathrm{false}.
\end{cases}
\end{aligned}
$$

Thus

$$
\boxed{\mathrm{Coordinator}=C_{\mathrm{active}}.}
$$

The coordinator starts a round only while idle and sends true to node $1$. After the first returning message it sends exactly the received bit on the second round, without modifying it. The second return is required before its own shutdown; if the attempt failed it remains idle and may try again or become active. It offers no status-change event between starting and finishing the protocol. The two round states are essential: the first $\mathit{ring}.0.\mathrm{true}$ means that the first survey succeeded, whereas the next one acknowledges the circulating decision.

As in part (a), the choices between observable events are expressed using [CSP external choice](../../../../../csp-external-choice.md). Execution is nondeterministic, but there is no hidden irrevocable decision to become active while refusing a message. This keeps the readiness required by the question.

## ↑ Ancestors (11)

1. [B](../b.md)
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
