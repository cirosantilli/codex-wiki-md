<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [circuit size class](../../../../../../circuit-size-class.md) $\mathrm{SIZE}(T(n))$ consists of languages whose length-$n$ [indicator functions](../../../../../../indicator-function.md) have [Boolean circuits](../../../../../../boolean-circuit.md) of size at most $T(n)$, for all sufficiently large $n$, over a fixed finite bounded-fan-in complete basis. The notation $\mathrm{SIZE}(O(T(n)))$ allows a constant factor. Input-node counting conventions do not affect the polynomial and exponential bounds here.

The nonuniform class [P/poly](../../../../../../p-poly.md) is

$$
\boxed{\mathrm{P/poly}=\bigcup_{d\geq0}\mathrm{SIZE}(O(n^d))}.
$$

There is no requirement that a uniform algorithm construct the [Boolean circuits](../../../../../../boolean-circuit.md). Equivalently, a polynomial-time machine can receive polynomial-length advice depending only on the input length, and the advice need not be computable.

Choose an [undecidable](../../../../../../undecidable-decision-problem.md) set $A\subseteq\mathbb N$, for example the set in the [halting problem](../../../../../../halting-problem.md) of indices of machines that halt on empty input, and define $U_A=\{1^n:n\in A\}$. For each length $n$, use a constant-zero [Boolean circuit](../../../../../../boolean-circuit.md) if $n\notin A$, and an AND of all $n$ input bits if $n\in A$. These [Boolean circuits](../../../../../../boolean-circuit.md) have size $O(n+1)$ and accept exactly $U_A$. Thus [undecidable unary languages with linear-size circuits](../../../../../../undecidable-unary-languages-with-linear-size-circuits.md) belong to [P/poly](../../../../../../p-poly.md).

Every [NP](../../../../../../np-complexity.md) language is decidable by enumerating its finitely many polynomial-length [certificate](../../../../../../certificate-complexity.md) encodings and running the polynomial-time verifier. If $U_A$ were decidable, testing $1^n$ would decide $A$, a contradiction. Therefore

$$
\boxed{U_A\in\mathrm{P/poly}\setminus\mathrm{NP},\qquad\mathrm{P/poly}\ne\mathrm{NP}}.
$$

This separates the classes in the stated direction; it does not claim that [NP](../../../../../../np-complexity.md) is not contained in [P/poly](../../../../../../p-poly.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
