<h1 id="2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take a countable [elementary substructure](../../../../../elementary-substructure.md) $\mathcal B'$ of $\mathcal A'$ containing the named constant, using the [Downward Lowenheim-Skolem theorem](../../../../../downward-lowenheim-skolem-theorem.md). Its reduct $\mathcal B$ has infinitely many singleton and doubleton classes. In particular it contains the partner of each of its non-singleton elements, and its interpretation of $P$ is exactly the singleton-class predicate.

Choose new distinct elements $u,v\notin B$. Define

$$
C=B\cup\{u\},\qquad D=B\cup\{u,v\}.
$$

In $\mathcal C$, make $u$ a new singleton class. In $\mathcal D$, make $\{u,v\}$ a new doubleton class; keep every old class of $\mathcal B$ unchanged. All three reducts are [first-order models](../../../../../model-of-a-first-order-theory.md) of the [complete theory](../../../../../complete-theory.md), and $\mathcal B\subseteq\mathcal C\subseteq\mathcal D$.

Expand $\mathcal C,\mathcal D$ by interpreting $P$ as singleton-class membership and retaining the original named constant from $B$. The resulting countable [first-order structures](../../../../../first-order-structure.md) $\mathcal C',\mathcal D'$ are each isomorphic to $\mathcal B'$: all have infinitely many classes of each size, and the bijections of classes can be chosen to preserve the constant and its class. Hence they are [first-order models](../../../../../model-of-a-first-order-theory.md) of $\operatorname{Th}(\mathcal A')$. Both inclusions $\mathcal B'\subseteq\mathcal C'$ and $\mathcal B'\subseteq\mathcal D'$ are genuine [structure embeddings](../../../../../structure-embedding.md), since no class meeting $B$ was changed. The given [quantifier elimination](../../../../../quantifier-elimination.md), together with the preceding implication to [first-order model](../../../../../model-of-a-first-order-theory.md) completeness, yields

$$
\mathcal B'\preceq\mathcal C',\qquad\mathcal B'\preceq\mathcal D'.
$$

Taking reducts gives $\boxed{\mathcal B\preceq\mathcal C,\quad\mathcal B\preceq\mathcal D}$. But

$$
\mathcal C\models\neg\exists y(E(u,y)\land y\ne u),\qquad\mathcal D\models\exists y(E(u,y)\land y\ne u),
$$

so $\boxed{\mathcal C\npreceq\mathcal D}$. There is no conflict with [quantifier elimination](../../../../../quantifier-elimination.md) in the expanded language: $P(u)$ changes truth value, so $\mathcal C'$ is not a substructure of $\mathcal D'$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the model theory course of the University of Oxford](../../../../split.md)
6. [Model theory course of the University of Oxford](../../../../../model-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
