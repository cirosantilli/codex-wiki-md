<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [partial computable function](../../../../../computable-function.md) may return a natural-number output or diverge. One concrete definition uses finite deterministic [Turing machines](../../../../../turing-machine.md); code the finite transition table by an integer $e$. Every single transition and every bounded simulation is computable, and the universal simulation gives a [universal partial computable function](../../../../../universal-partial-computable-function.md)

$$
U(e,x)\simeq\varphi_e(x).
$$

The symbol $\simeq$ means equal outputs when defined and simultaneous divergence otherwise. A [total computable function](../../../../../total-computable-function.md) is a [partial computable function](../../../../../computable-function.md) defined on every input. Different program codes may compute the same partial function; this distinction between syntax and computed behavior is crucial.

The equivalent recursive description starts with zero, successor and projections and closes under composition and [primitive recursion](../../../../../primitive-recursion.md), giving the [primitive recursive functions](../../../../../primitive-recursive-function.md). Add [unbounded minimization](../../../../../mu-operator.md): search for the first $y$ at which a predicate returns zero, requiring every preceding tested computation to have converged. This gives the partial recursive functions. To see the connection with machines, encode finite configurations and histories. Checking a proposed halting history is a primitive recursive predicate $T(e,x,t)$, and a [primitive recursive function](../../../../../primitive-recursive-function.md) $V$ extracts its output. Thus a machine computation has the normal form $V(\mu t\,T(e,x,t))$. Conversely a machine can implement composition, [primitive recursion](../../../../../primitive-recursion.md) and this successive search. This proves equivalence of the formal definitions. The [Church–Turing thesis](../../../../../church-turing-thesis.md) identifying them with informal effective calculability is a thesis, not an additional formal theorem used in the proof.

A [computably enumerable set](../../../../../recursively-enumerable-set.md) is one enumerated by a program, equivalently the domain of a [partial computable function](../../../../../computable-function.md). For the forward implication wait until the given input is enumerated; for the reverse implication run all input computations by [dovetailing](../../../../../dovetailing.md), outputting those that halt. A [set](../../../../../set-split.md) is decidable if its characteristic function is total computable. It is decidable exactly when both it and its complement are computably enumerable: dovetail their enumerators and stop when one lists the input.

The [S-m-n theorem](../../../../../smn-theorem.md) supplies effective specialization of parameters. Given a code for a program on $(a,x)$, compile the constant $a$ into a wrapper that writes it and then calls that program. The wrapper's transition table is computably produced from the original table and $a$, yielding a [total computable function](../../../../../total-computable-function.md) $s$ with $\varphi_{s(e,a)}(x)\simeq\varphi_e(a,x)$. This elementary code-construction proof is all the specialization machinery needed below.

The diagonal [halting problem](../../../../../halting-problem.md) $K=\{e:\varphi_e(e)\downarrow\}$ is computably enumerable by universal simulation but not decidable. If a total decider $h$ existed, the program that halts on $x$ precisely when $h(x)=0$ would have an index $d$. Evaluating it at $d$ gives $d\in K$ exactly when $d\notin K$, a contradiction.

For [Rice theorem](../../../../../rice-s-theorem.md), let $\mathcal C$ be a nontrivial collection of [partial computable functions](../../../../../computable-function.md), and let its [index set](../../../../../index-set.md) be $S=\{e:\varphi_e\in\mathcal C\}$. Membership must depend only on the computed function, not on its code. Let $\bot$ be the nowhere-defined function. First suppose $\bot\notin\mathcal C$, and choose a computable partial function $g\in\mathcal C$ with a fixed program. Uniformly from $e$, produce the following program on input $x$: first simulate $\varphi_e(e)$; if it halts, then simulate $g(x)$ and return that output. Its index $r(e)$ is total computable by specialization, and

$$
\varphi_{r(e)}=\begin{cases}g,&e\in K,\\ \bot,&e\notin K.\end{cases}
$$

Therefore $e\in K$ iff $r(e)\in S$, so a decider for $S$ would decide $K$. If instead $\bot\in\mathcal C$, apply the same argument to the nontrivial complement collection, whose [index set](../../../../../index-set.md) would also be decidable if $S$ were. We conclude

$$
\boxed{\text{Every nontrivial extensional index set is undecidable.}}
$$

For computably enumerable languages, use the same waiting program before beginning a fixed enumeration, taking the empty language as the bottom object. Properties such as having finite domain, computing a total function or recognizing a particular nontrivial language are therefore undecidable. Purely syntactic properties such as the parity of the code are excluded: they are not extensional. Rice's conclusion is undecidability, not that every such [index set](../../../../../index-set.md) must fail to be computably enumerable.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
