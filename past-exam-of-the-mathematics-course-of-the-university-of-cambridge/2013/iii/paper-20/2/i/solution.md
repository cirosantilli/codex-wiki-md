<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

If $M$ halts on every input, simulate $M$ on input $n$ while counting its steps, and output that count when it halts. The resulting function $t_M(n)$ is a [total computable function](../../../../../../total-computable-function.md). Consequently **yes: one may take the exact running time**,

$$
\boxed{f(n)=t_M(n)}.
$$

This construction does not promise a simple closed expression or a bound of any particular complexity class; it uses the promised totality of this particular machine.

For a machine computing a [partial computable function](../../../../../../computable-function.md), its exact halting-time function is still a [partial computable function](../../../../../../computable-function.md), with the same domain. A finite bound cannot cover a genuinely infinite computation. Even restricting attention to inputs on which $M$ halts, a [total computable function](../../../../../../total-computable-function.md) bounding all halting times need not exist. In fact the precise characterization is the [computable bound on halting time](../../../../../../computable-bound-on-halting-time.md) criterion:

$$
\boxed{\exists\text{ total computable }f\ \forall n\in\operatorname{dom}M\;t_M(n)\leq f(n)
\quad\Longleftrightarrow\quad\operatorname{dom}M\text{ is decidable}.}
$$

For the forward implication, compute $f(n)$ and simulate $M(n)$ for that many steps. If it has not halted, the proposed bound ensures that it never will. This decides the domain. Conversely, first decide whether $n$ is in the domain; return zero outside it and the simulated halting time inside it. This defines a [total computable function](../../../../../../total-computable-function.md) satisfying the bound. The time needed to compute the bound itself is irrelevant to this argument.

A universal halting recognizer has undecidable domain by the [halting problem](../../../../../../halting-problem.md), so it has no such total bound. On the other hand, a machine that immediately halts on even inputs and loops on odd inputs computes a nontotal [partial computable function](../../../../../../computable-function.md) but has a constant bound on its halting times. Thus **nontotality alone does not decide whether a total bound exists**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
