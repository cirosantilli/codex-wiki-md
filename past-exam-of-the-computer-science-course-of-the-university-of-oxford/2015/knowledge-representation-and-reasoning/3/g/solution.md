<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The satisfiability problem is $\boxed{\text{decidable}}$. Partition the positive facts according to their predicate symbols. Let $\mathcal A_{\mathcal T}$ contain those using [description logic concepts](../../../../../description-logic-concept.md) or [description logic roles](../../../../../description-logic-role.md) from $\mathcal T$. Run an ordinary [ALC](../../../../../alc.md) [knowledge base](../../../../../knowledge-base.md) consistency procedure on $(\mathcal T,\mathcal A_{\mathcal T})$. Return `no` if it is inconsistent, and `yes` otherwise.

The `no` answer is sound because any model of the whole [knowledge base](../../../../../knowledge-base.md) would restrict to a model of $(\mathcal T,\mathcal A_{\mathcal T})$. For the converse, take a model $\mathcal I$ of that [ALC](../../../../../alc.md) part. Keep its domain, individual interpretations and [TBox](../../../../../tbox.md) predicates. Interpret every predicate used by the positive [Datalog](../../../../../datalog.md) rules as the full relation of its arity on this same domain. This is possible because those predicates are disjoint from the [TBox](../../../../../tbox.md) predicates. Every [Datalog](../../../../../datalog.md) rule head is then true under every variable assignment, so every positive rule and every remaining positive fact is satisfied. Predicates occurring only in facts can likewise be interpreted as full relations. Any individual name not already interpreted can denote an arbitrary domain element.

Consequently,

$$
\boxed{(\mathcal T,\mathcal R,\mathcal A)\text{ is satisfiable}\quad\Longleftrightarrow\quad(\mathcal T,\mathcal A_{\mathcal T})\text{ is satisfiable}.}
$$

The argument depends on both restrictions in the question: disjoint predicate vocabularies and positive rule heads. A rule concluding $\bot$ would not be made true by filling all relations. Sharing constants alone causes no problem, since the expansion uses the same domain and the same interpretations of those constants.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [3](../../3.md)
3. [Knowledge representation and reasoning](../../../knowledge-representation-and-reasoning-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
