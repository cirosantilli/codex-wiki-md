<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The problem belongs to [NP](../../../../../../np-complexity.md): an assignment in $\mathbb F_2^n$ is a polynomial-length [certificate in computational complexity](../../../../../../certificate-complexity.md), and substitution verifies every equation in polynomial time.

For [NP-hardness](../../../../../../np-hardness.md), reduce the [Circuit satisfiability problem](../../../../../../circuit-satisfiability-problem.md). Introduce one variable in $\mathbb F_2$ for every wire of a [Boolean circuit](../../../../../../boolean-circuit.md). A [logical negation](../../../../../../negation.md) gate $w=\neg u$ is enforced by $w=1-u$, and a [logical conjunction](../../../../../../logical-conjunction.md) gate $w=u\wedge v$ is enforced by $w=uv$. For a [logical disjunction](../../../../../../logical-disjunction.md) gate use the suggested quadratic equation

$$
(1-u)(1-v)=1-w,
$$

which is equivalent to $w=u\vee v$ for bits $u,v,w$. Add the linear equation $w_{\rm out}=1$ for the designated output wire.

The construction introduces one variable and one equation per wire or gate, so it is a [polynomial-time many-one reduction](../../../../../../polynomial-time-many-one-reduction.md). A satisfying circuit input extends uniquely through its gates to a solution of the equations, and any solution gives a consistent accepting circuit computation. Since circuit satisfiability is NP-complete, [quadratic-equation satisfiability over F2](../../../../../../quadratic-equation-satisfiability-over-f2.md) is therefore

$$
\boxed{\mathbf{NP}\text{-complete}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
