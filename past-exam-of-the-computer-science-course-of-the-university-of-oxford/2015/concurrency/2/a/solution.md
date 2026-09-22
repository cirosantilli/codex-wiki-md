<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a finite [CSP trace](../../../../../csp-trace.md) $s$, let $L(s)$ be its sequence of values on $\mathit{left}$ and $O(s)$ its sequence of values on $\mathit{right}$, with channel names removed. Restrict the external alphabet to these two channels. The behavioural [CSP trace](../../../../../csp-trace.md) specification for an unbounded [FIFO buffer](../../../../../fifo-buffer.md) is

$$
\boxed{\forall s\in\operatorname{traces}(P):\quad O(s)\preceq L(s),}
$$

where $\preceq$ means [prefix of a list](../../../../../prefix-of-a-list.md), not merely [subsequence](../../../../../subsequence.md). Outputs must therefore occur in input order, cannot duplicate or invent values, and cannot precede their inputs. Applying the condition to every [CSP trace](../../../../../csp-trace.md) also checks every execution prefix.

For a legal $s$, write $L(s)=O(s)\mathbin{\frown}q(s)$, so $q(s)$ is the pending [FIFO queue](../../../../../fifo-queue.md) content. Define the events that must remain available by

$$
E(q)=\{\mathit{left}.x:x\in T\}\cup\begin{cases}\varnothing,&q=\langle\rangle,\\\{\mathit{right}.\operatorname{head}(q)\},&q\ne\langle\rangle.\end{cases}
$$

In addition to the [CSP trace](../../../../../csp-trace.md) condition, require the behavioural [CSP stable failure](../../../../../csp-stable-failure.md) condition

$$
\boxed{\forall(s,X)\in\operatorname{failures}(P):\quad X\cap E(q(s))=\varnothing.}
$$

Thus an unbounded [FIFO buffer](../../../../../fifo-buffer.md) cannot stably refuse any new input, and a nonempty [FIFO buffer](../../../../../fifo-buffer.md) cannot stably refuse its oldest pending output. An empty [FIFO buffer](../../../../../fifo-buffer.md) can refuse every output. Readiness of an input and readiness of an output are required together; the environment may choose either. These conditions do not require an output while the environment refuses to accept it. In a [CSP failures-divergences model](../../../../../csp-failures-divergences-model.md) specification, also exclude [CSP divergence](../../../../../csp-divergence.md); the stable-readiness condition alone does not rule out an implementation that loops internally forever without reaching a [CSP stable state](../../../../../csp-stable-state.md).

## ↑ Ancestors (11)

1. [A](../a.md)
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
