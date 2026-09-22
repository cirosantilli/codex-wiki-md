<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Cook-Levin theorem](../../../../../../cook-levin-theorem.md) states that the [Boolean satisfiability problem](../../../../../../boolean-satisfiability-problem.md) is [NP-complete](../../../../../../np-completeness.md) under [polynomial-time many-one reductions](../../../../../../polynomial-time-many-one-reduction.md). Membership in [NP](../../../../../../np-complexity.md) follows by guessing an assignment and evaluating the formula in time polynomial in its description length.

For hardness, let $L\in\mathrm{NP}$ have a deterministic polynomial-time verifier $M(x,y)$, with a polynomial witness-length bound. Use a fixed polynomial [certificate](../../../../../../certificate-complexity.md) length: a short [certificate](../../../../../../certificate-complexity.md) is encoded by its length followed by padded data, and the verifier checks this encoding. Pad the computation to exactly $T=T(|x|)$ steps, with accepting and rejecting states absorbing. Enlarge $T$ polynomially if necessary to cover input/witness initialization. A standard polynomial slowdown permits a single-tape [Turing machine](../../../../../../turing-machine.md), so it suffices to handle that model.

Encode a tape cell by a fixed number of bits recording its alphabet symbol and either no head or the head's finite control state. Starting with one head, a cell's next label depends only on its own label and the two neighboring labels: a head can change the symbol where it sits and can enter only a neighbor. Each such finite local function has a constant-size [Boolean circuit](../../../../../../boolean-circuit.md). The initial row fixes $x$, blanks and the starting head, leaving only the witness bits as [Boolean circuit](../../../../../../boolean-circuit.md) inputs. There are $O(T)$ relevant cells with blank margins beyond every possible head position, and $T$ updates. Repeating these local [Boolean circuits](../../../../../../boolean-circuit.md) produces a [Boolean circuit](../../../../../../boolean-circuit.md) $C_x(y)$ of size $O(T^2)$, with an output detecting an accepting head in the final row. The construction is computable in [polynomial time](../../../../../../polynomial-time.md). Induction on rows shows that every assignment to $y$ produces exactly the verifier's valid computation; invalid local encodings can be assigned arbitrary [Boolean circuit](../../../../../../boolean-circuit.md) behavior because they never arise from the valid initial row.

Convert this [Boolean circuit](../../../../../../boolean-circuit.md) to [conjunctive normal form](../../../../../../conjunctive-normal-form.md) using a [Tseitin transformation](../../../../../../tseytin-transformation.md). Introduce one variable for each wire, and encode each gate output $z$ by:

| Gate relation | [Clauses](../../../../../../clause-of-a-boolean-formula.md) imposing equivalence |
| --- | --- |
| $z=x\wedge y$ | $(\neg z\vee x)\wedge(\neg z\vee y)\wedge(z\vee\neg x\vee\neg y)$ |
| $z=x\vee y$ | $(z\vee\neg x)\wedge(z\vee\neg y)\wedge(\neg z\vee x\vee y)$ |
| $z=\neg x$ | $(z\vee x)\wedge(\neg z\vee\neg x)$ |

Unit [clauses](../../../../../../clause-of-a-boolean-formula.md) fix constant sources and assert the final output. Each input assignment has exactly one extension to its gate values, so the resulting formula $F_x$ is satisfiable precisely when some witness makes $M(x,y)$ accept. It has $O(T^2)$ [clauses](../../../../../../clause-of-a-boolean-formula.md) of bounded length and is produced in [polynomial time](../../../../../../polynomial-time.md). Thus

$$
\boxed{x\in L\iff F_x\text{ is satisfiable},\qquad\mathrm{SAT}\text{ is NP-complete}}.
$$

This proof also gives hardness for [clauses](../../../../../../clause-of-a-boolean-formula.md) of at most three [literals](../../../../../../boolean-literal.md), without needing a separate satisfiability assumption.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
