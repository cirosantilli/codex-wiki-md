<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An oracle can recognize a solution without disclosing it in advance. If an efficiently evaluable or black-box predicate has the promised unique marked input, write $f(x)=1$ exactly for that input. A [Boolean quantum oracle](../../../../../../boolean-quantum-oracle.md) computes this predicate reversibly as

$$
|x\rangle|b\rangle\longmapsto|x\rangle|b\oplus f(x)\rangle.
$$

Its diagonal projector on the search register is $\sum_x f(x)|x\rangle\langle x|=|w\rangle\langle w|$. To implement a selectable phase, compute $f(x)$ into a zero [quantum ancilla](../../../../../../quantum-ancilla.md), apply a known phase to its $1$ component, and uncompute. The search register then undergoes

$$
|x\rangle\longmapsto e^{-i\Delta t f(x)}|x\rangle
=e^{-i\Delta tP_w}|x\rangle.
$$

This requires evaluation access to the predicate, not classical knowledge of which input passes it. The $P_\psi$ term is known from the [Hadamard transform](../../../../../../hadamard-transform.md). With Hamiltonian-oracle access, or by controlled short-time simulations of the two terms, their sum can realize [continuous-time quantum search](../../../../../../continuous-time-quantum-search.md).

**The unknown projector is supplied through an oracle or a physically encoded recognition rule.** It cannot be manufactured for an arbitrary hidden $w$ with no such input-dependent resource. The oracle assumption and the fixed energy scale $\Delta$ are essential when interpreting the square-root search time as a computational advantage.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
