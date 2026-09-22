<h1 id="1/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

An exponential increase is unavoidable for an equivalent [conjunctive normal form](../../../../../../conjunctive-normal-form.md) over the original variables. Consider the linear-size [Boolean formula](../../../../../../boolean-formula.md)

$$
F_n=\bigvee_{i=1}^{n}(p_i\land q_i).
$$

Distributing gives the $2^n$ [Boolean clauses](../../../../../../clause-of-a-boolean-formula.md)

$$
F_n\equiv\bigwedge_{(r_1,\ldots,r_n)\in\{p_1,q_1\}\times\cdots\times\{p_n,q_n\}}(r_1\lor\cdots\lor r_n).
$$

To prove that the growth is necessary, fix one choice $r_i\in\{p_i,q_i\}$. Let $\alpha_r$ make every $r_i$ false and its partner true. Each pair then contains a false variable, so $F_n$ is false. Any equivalent [conjunctive normal form](../../../../../../conjunctive-normal-form.md) must contain a [Boolean clause](../../../../../../clause-of-a-boolean-formula.md) $C$ falsified by $\alpha_r$ and entailed by $F_n$.

Every individual term $p_i\land q_i$ entails $C$, because that term implies $F_n$. After tautological [Boolean clauses](../../../../../../clause-of-a-boolean-formula.md) are discarded, this forces $C$ to contain a positive $p_i$ or positive $q_i$ for every $i$: otherwise set both variables in that pair true and independently falsify all [Boolean literals](../../../../../../boolean-literal.md) of $C$, contradicting the entailment. Since $C$ is false at $\alpha_r$, it must contain the false member $r_i$, never its true partner. Consequently the same $C$ cannot be false at any different $\alpha_s$. The $2^n$ different assignments therefore require at least $2^n$ different [Boolean clauses](../../../../../../clause-of-a-boolean-formula.md).

Writing the answer already takes $\boxed{\Omega(2^n)\text{ time in the worst case}}$. This obstruction applies to [first-order logic](../../../../../../first-order-logic.md) as well, since the example can be expressed using ground unary [atomic formulas](../../../../../../atomic-formula.md). It concerns exact equivalence without auxiliary symbols. A [Tseytin transformation](../../../../../../tseytin-transformation.md) can produce a polynomial-size equisatisfiable [conjunctive normal form](../../../../../../conjunctive-normal-form.md) with auxiliary variables, so the statement must not be extended to that different task.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Knowledge representation and reasoning](../../../../knowledge-representation-and-reasoning-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
