<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The first [Hadamard transform](../../../../../../hadamard-transform.md) prepares a uniform [superposition](../../../../../../superposition-principle.md) in the first register while the second stays zero. The [Boolean quantum oracle](../../../../../../boolean-quantum-oracle.md), now with an $n$-bit output register and bitwise addition, therefore gives

$$
\boxed{|\Omega\rangle=2^{-n/2}\sum_{x\in\mathbb F_2^n}|x\rangle|f(x)\rangle.}
$$

This state is normalized because distinct $x$ labels are orthogonal, even when their oracle outputs coincide. Addition in the oracle is bitwise exclusive-or, making the oracle reversible; replacing the first register by $f(x)$ would not define a [unitary gate](../../../../../../quantum-logic-gate.md) for a two-to-one function.

For the later recovery steps we use the intended nonzero hidden-period promise $s\ne0$. Then two-to-one behavior and $f(x+s)=f(x)$ force each fibre to be exactly $\{x,x+s\}$. The printed allowance $s\in\{0,1\}^n$ does not explicitly exclude zero. If zero were allowed without a nonzero-period promise, the displayed identity would hold trivially for every function and would not specify [Simon's problem](../../../../../../simon-s-problem.md). That distinction is addressed again in the query count.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2](../../2.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
