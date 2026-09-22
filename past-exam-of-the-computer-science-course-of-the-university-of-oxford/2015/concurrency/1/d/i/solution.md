<h1 id="1/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use a chain of identical storage cells, each retaining the first value it sees and passing later values to the next cell. On the return journey it passes the next cell's reversed output before emitting its own retained value. This turns the chain into a distributed [LIFO stack](../../../../../../stack-data-structure.md).

Here is one cell template. Its ports $l,r$ carry incoming values towards the tail; $v,u$ carry returning values towards the front. Each port carries values in $T\cup\{\mathit{end}\}$, with the [sentinel value](../../../../../../sentinel-value.md) outside $T$:

$$
\begin{aligned}
\mathrm{Cell}&=l?x:T\to\mathrm{Hold}(x),\\
\mathrm{Hold}(x)&=\bigl(l?y:T\to r!y\to\mathrm{Hold}(x)\bigr)\\
&\quad\mathbin\square\bigl(l.\mathit{end}\to r.\mathit{end}\to\mathrm{Drain}(x)\bigr),\\
\mathrm{Drain}(x)&=\bigl(v?y:T\to u!y\to\mathrm{Drain}(x)\bigr)\\
&\quad\mathbin\square\bigl(v.\mathit{end}\to u!x\to u.\mathit{end}\to\mathrm{STOP}\bigr).
\end{aligned}
$$

An input such as $l?x:T$ abbreviates an indexed [CSP external choice](../../../../../../csp-external-choice.md) over the corresponding [CSP events](../../../../../../csp-event.md). An output $r!y$ is the [CSP prefixing](../../../../../../csp-prefixing.md) action $r.y$. There is no extra controller process.

For $n\geq1$, take $n$ copies of this same template. Introduce channels $d_i,u_i$ for $0\leq i\leq n$ and apply port [CSP event renaming](../../../../../../csp-event-renaming.md) to copy $i$, for $1\leq i\leq n$, as follows:

$$
l.x\mapsto d_{i-1}.x,\quad r.x\mapsto d_i.x,\quad v.x\mapsto u_i.x,\quad u.x\mapsto u_{i-1}.x.
$$

At the front put $d_0=\mathit{in}$ and $u_0=\mathit{out}$. Adjacent cells synchronize on every shared $d_i$ or $u_i$ [CSP event](../../../../../../csp-event.md). The two tail channels $d_n,u_n$ are sentinel-only: $d_n.\mathit{end}$ and $u_n.\mathit{end}$ are local tail [CSP events](../../../../../../csp-event.md), with no other participant required. Disable all $d_n.x,u_n.x$ for $x\in T$. Formally, use a partial relational [CSP event renaming](../../../../../../csp-event-renaming.md) for the last copy, omitting the pairs for its $r.x,v.x$ with $x\in T$; an unmapped transition is blocked. This explicitly prevents a fictitious tail from generating data.

Let $C_i$ be the resulting port-renamed cell and $A_i$ its visible alphabet. With $H$ consisting of the internal link [CSP events](../../../../../../csp-event.md), including the two tail [CSP events](../../../../../../csp-event.md), the answer is

$$
\boxed{\mathrm{Reverse}_n=\left(\mathop{\Vert}_{i=1}^{n}[A_i]\ C_i\right)\setminus H.}
$$

Here the indexed operator is [CSP alphabetized parallel composition](../../../../../../csp-alphabetized-parallel-composition.md): each [CSP event](../../../../../../csp-event.md) is synchronized by all cells whose alphabets contain it. There are exactly $n$ storage-cell processes; port wiring and the sentinel-only tail adapt their interfaces, without adding a helper process. The local tail [CSP events](../../../../../../csp-event.md) are hidden, as are all inter-cell communications.

To see correctness, after inputs $x_1,\ldots,x_n$ have propagated, cell $i$ retains $x_i$. The input [sentinel value](../../../../../../sentinel-value.md) propagates to the tail. The last cell performs its two local tail [CSP events](../../../../../../csp-event.md), then returns $x_n,\mathit{end}$. Inductively, if the suffix after cell $i$ returns $x_n,\ldots,x_{i+1},\mathit{end}$, cell $i$ relays those values, replaces the final [sentinel value](../../../../../../sentinel-value.md) by $x_i,\mathit{end}$, and stops. Hence the external output is

$$
\boxed{\mathit{out}.x_n,\ldots,\mathit{out}.x_1,\mathit{out}.\mathit{end},}
$$

and starts only after $\mathit{in}.\mathit{end}$. Shared links provide [synchronization](../../../../../../synchronization-computing.md) rather than an assumption that all cells take steps simultaneously. For the degenerate known-empty input, no storage is needed: the interface is simply $\mathit{in}.\mathit{end}\to\mathit{out}.\mathit{end}\to\mathrm{STOP}$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Concurrency](../../../../concurrency-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
