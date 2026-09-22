<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Using the absorbed [TBox](../../../../../tbox.md) with its primitive inclusion, translate [description logic concepts](../../../../../description-logic-concept.md) as unary predicates and [description logic roles](../../../../../description-logic-role.md) as binary predicates. [Concept satisfiability](../../../../../concept-satisfiability.md) means that some element belongs to $A\sqcap C$, while every element satisfies the [TBox](../../../../../tbox.md) axioms. The required [first-order sentence](../../../../../first-order-sentence.md) is

$$
\boxed{\begin{aligned}
&\exists x\,(A(x)\land C(x))\\
{}\land{}&\forall u\,(A(u)\to\neg B(u))\\
{}\land{}&\forall u\,\bigl(C(u)\leftrightarrow\exists v\,P(u,v)\bigr).
\end{aligned}}
$$

Only $\mathcal T_u$ is included here, as requested. There is no requirement to satisfy (1), (2) or (3). For instance, one element with $A=C=\{d\}$, $B=\varnothing$ and $P=\{(d,d)\}$ satisfies this [first-order sentence](../../../../../first-order-sentence.md).

Alternatively, unfolding the absorbed [TBox](../../../../../tbox.md) first gives the existential [first-order sentence](../../../../../first-order-sentence.md) $\exists x\exists y\,(A_0(x)\land\neg B(x)\land P(x,y))$. The interpretation of the eliminated names is then recovered by $A=A_0\setminus B$ and $C=\{x:\exists y\,P(x,y)\}$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Knowledge representation and reasoning](../../../knowledge-representation-and-reasoning-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
