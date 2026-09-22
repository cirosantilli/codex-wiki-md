# Boolean valuation

↑ **Parent:** [Propositional logic](propositional-logic.md)

A [Boolean valuation](boolean-valuation.md) $v$ assigns each primitive [proposition](proposition.md) a value in $\{\mathrm F,\mathrm T\}$, equivalently $\{0,1\}$, and extends recursively to every [propositional formula](propositional-formula.md) using the classical [logical connectives](logical-connective.md). The same primitive [proposition](proposition.md) always receives the same value within one [Boolean valuation](boolean-valuation.md). For compound [propositional formulas](propositional-formula.md) $A$ and $B$,

$$
\begin{aligned}
v(\neg A)=\mathrm T&\iff v(A)=\mathrm F,\\
v(A\land B)=\mathrm T&\iff v(A)=\mathrm T\text{ and }v(B)=\mathrm T,\\
v(A\lor B)=\mathrm T&\iff v(A)=\mathrm T\text{ or }v(B)=\mathrm T,\\
v(A\to B)=\mathrm F&\iff v(A)=\mathrm T\text{ and }v(B)=\mathrm F.
\end{aligned}
$$

Every other case receives the opposite value. Thus $v(p)=\mathrm T,v(q)=\mathrm F$ gives $v((p\to q)\land p)=\mathrm F$. A [truth table](truth-table.md) varies the assignment; recursive evaluation computes one row. The truth-functional restriction means that changing what the primitive [propositions](proposition.md) describe, while retaining their values, cannot change the value of the compound [propositional formula](propositional-formula.md). See [forall x: Calgary, chapter 9](https://forallx.openlogicproject.org/html/Ch9.html) and [section 10.1](https://forallx.openlogicproject.org/html/Ch10.html).

**Table of contents**

- [Truth table](truth-table.md)

## ↑ Ancestors (6)

1. [Propositional logic](propositional-logic.md)
2. [Mathematical logic](mathematical-logic-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (13)

- [3-SAT reduction to vertex cover](3-sat-reduction-to-vertex-cover.md)
- [Boolean valuation](boolean-valuation.md)
- [Extended omitting types theorem for propositional logic](extended-omitting-types-theorem-for-propositional-logic.md)
- [Logical validity](logical-validity.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-20/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-38/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/16i/solution.md)
- [Propositional formula](propositional-formula.md)
- [Propositional logic](propositional-logic.md)
- [Propositional theory](propositional-theory.md)
- [Propositional type](propositional-type.md)
- [Tautology](tautology.md)
- [Truth table](truth-table.md)
