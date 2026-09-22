<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each node let

$$
\begin{aligned}
A_n&=\{\mathit{active}.n,\mathit{idle}.n,\mathit{shutdown}.n\}\\
&\quad\cup\{\mathit{ring}.n.b,\mathit{ring}.(n\oplus1).b:b\in\mathrm{Bool}\},\\
P_0&=\mathrm{Coordinator},\qquad P_n=\mathrm{Node}(n)\quad(1\leq n<N).
\end{aligned}
$$

The required [CSP alphabetized parallel composition](../../../../../csp-alphabetized-parallel-composition.md) is

$$
\boxed{\mathrm{System}=\mathop{\Vert}_{n=0}^{N-1}[A_n]\ P_n.}
$$

Each message [CSP event](../../../../../csp-event.md) belongs to exactly the sender's and receiver's alphabets and synchronizes those two processes. A status signal belongs only to its own node. Using the common set of all message events as an all-node synchronization alphabet would be incorrect: unrelated nodes would then have to participate in each point-to-point transfer. The initial definitions in parts (a) and (b) make every node active. Keep the message [CSP events](../../../../../csp-event.md) visible here; later checks can apply [CSP hiding](../../../../../csp-hiding.md) as needed.

## ↑ Ancestors (11)

1. [C](../c.md)
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
