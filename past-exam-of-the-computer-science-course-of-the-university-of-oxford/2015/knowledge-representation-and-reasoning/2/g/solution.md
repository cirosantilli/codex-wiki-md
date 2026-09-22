<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The complete numbered axioms in the rule fragment [RL description logic](../../../../../rl-description-logic.md) are $\boxed{(1),(3),(4)}$. Their translations to [Datalog](../../../../../datalog.md) with constraints are

$$
\boxed{\begin{aligned}
R(x,y)&\to C(y),\\
R(x,y)\land R(y,z)\land A(z)\land R(x,w)&\to A(w),\\
R(x,y)\land R(y,z)\land B(z)\land R(x,w)&\to A(w),\\
A(x)\land B(x)&\to\bot.
\end{aligned}}
$$

The first rule is (1). For (3), its existential antecedent needs a two-edge $R$ path ending at an $A$ or $B$ element. Split that disjunction into two [Datalog](../../../../../datalog.md) rules, and use a separate variable $w$ for an arbitrary immediate $R$-successor of $x$. The conclusion applies to every such successor, not merely the path witness $y$.

The last rule is a constraint: a ground instance with both premises true makes the [knowledge base](../../../../../knowledge-base.md) inconsistent. If an implementation permits only positive [Datalog](../../../../../datalog.md) heads, replace $\bot$ by a fresh nullary predicate $\mathit{Bad}$ and separately check that it is never derived. Merely deriving $\mathit{Bad}$ without that check would not express disjointness.

Axiom (2) requires an existential witness in its head and is outside [RL description logic](../../../../../rl-description-logic.md). Axiom (5), considered as the whole equivalence, is outside for the same reason in the direction $C\sqsubseteq\exists P.\top$. If definitions are split before selecting eligible [general concept inclusions](../../../../../general-concept-inclusion.md), its reverse direction is eligible and adds $\boxed{P(x,y)\to C(x)}$. Keep the difference between selecting the complete equivalence and retaining its rule-expressible half explicit. The permitted positions of existential and universal restrictions are specified in the [Section 4.2.3: subclass and superclass expressions; Section 4.2.5: class axioms](../../../../../owl-2-web-ontology-language-profiles-second-edition.md).

## ↑ Ancestors (11)

1. [G](../g.md)
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
