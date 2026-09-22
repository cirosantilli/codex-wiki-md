<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $T_e$ be the theory of the [extension axioms for an unrestricted binary relation](../../../../../../extension-axioms-for-an-unrestricted-binary-relation.md). It has [quantifier elimination](../../../../../../quantifier-elimination.md). To prove this, consider a conjunction of literals $\theta(y,\mathbf x)$. A witness $y$ equal to one of the parameters is handled by substitution. A witness distinct from them is governed entirely by a finite pattern of incoming edges, outgoing edges and its loop. For each equality pattern of the parameter tuple, incompatible literals make the pattern impossible, and every compatible pattern is supplied by the appropriate extension axiom. Thus existence of a witness is a finite disjunction of quantifier-free conditions on the parameters. Disjunctive normal form and induction on formulas eliminate all remaining quantifiers.

Given any formula $\phi(\mathbf x)$, choose a quantifier-free $\psi(\mathbf x)$ with

$$
T_e\models\forall\mathbf x\,[\phi(\mathbf x)\leftrightarrow\psi(\mathbf x)].
$$

By [compactness theorem](../../../../../../compactness-theorem.md), finitely many extension axioms $\sigma_1,\ldots,\sigma_s$ already entail this particular universally quantified equivalence. Each has asymptotic probability one by the assumption. The union bound gives

$$
\Pr\!\left(\bigwedge_{j=1}^s\sigma_j\right)
\ge1-\sum_{j=1}^s\Pr(\neg\sigma_j)\longrightarrow1.
$$

Therefore the universal equivalence also has asymptotic probability one. We obtain **asymptotic equivalence to a [quantifier-free formula](../../../../../../quantifier-free-formula.md)**, uniformly over every tuple in each structure satisfying those finitely many axioms. An infinite conjunction of probability-one events is not used; the finite consequence supplied by compactness is essential.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9](../../9.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
