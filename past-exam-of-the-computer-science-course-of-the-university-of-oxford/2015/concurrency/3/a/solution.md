<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the intended nontrivial [ring network](../../../../../ring-network.md), with $N\geq2$, and let $n\oplus1=(n+1)\bmod N$. A [CSP event](../../../../../csp-event.md) $\mathit{ring}.n.b$ is one synchronized transfer from the predecessor to receiver $n$, rather than a separate enqueue and dequeue. Let $s$ be the [Boolean](../../../../../boolean-data-type.md) saying whether node $n$ is active. For $1\leq n<N$, define

$$
\begin{aligned}
V(n,s)&=\begin{cases}\mathit{idle}.n\to\mathrm{Free}(n,\mathrm{false}),&s=\mathrm{true},\\\mathit{active}.n\to\mathrm{Free}(n,\mathrm{true}),&s=\mathrm{false},\end{cases}\\
\mathrm{Free}(n,s)&=V(n,s)\mathbin\square\bigl(\mathit{ring}.n?b:\mathrm{Bool}\to\mathit{ring}.(n\oplus1).(b\land\neg s)\to\mathrm{Second}(n,s)\bigr),\\
\mathrm{Second}(n,s)&=\mathit{ring}.n?b:\mathrm{Bool}\to\mathit{ring}.(n\oplus1).b\to\begin{cases}\mathit{shutdown}.n\to\mathrm{STOP},&b=\mathrm{true},\\\mathrm{Free}(n,s),&b=\mathrm{false}.
\end{cases}
\end{aligned}
$$

Initially the node is active:

$$
\boxed{\mathrm{Node}(n)=\mathrm{Free}(n,\mathrm{true}).}
$$

The [CSP external choice](../../../../../csp-external-choice.md) in $\mathrm{Free}$ always offers both possible incoming message values as well as the permitted status change. Thus a decision to change status cannot internally withdraw readiness to receive a message. When the first message arrives, an active node forces its forwarded bit to false; an idle node preserves the bit. The status $s$ is retained until the second-round message has been forwarded. Neither the forwarding prefix nor $\mathrm{Second}$ offers status-change events, enforcing the protocol's freeze. On a false second-round message the node resumes its previous status; on a true one it forwards the bit before announcing shutdown.

## ↑ Ancestors (11)

1. [A](../a.md)
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
