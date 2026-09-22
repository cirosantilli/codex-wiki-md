<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the language of a single edge relation $E$, axiomatize an undirected loop-free graph by

$$
\forall x\,\neg E(x,x),\qquad
\forall x\forall y\,(E(x,y)\leftrightarrow E(y,x)).
$$

For every pair of nonnegative integers $r,s$, add the extension axiom demanding, for any distinct $u_1,\ldots,u_r,v_1,\ldots,v_s$, a new vertex $z$ such that

$$
z\ne u_i,v_j,\qquad E(z,u_i)\ (1\le i\le r),\qquad
\neg E(z,v_j)\ (1\le j\le s).
$$

These axioms form the [theory of the random graph](../../../../../../theory-of-the-random-graph.md). Repetition of the fresh-vertex requirement also forces infinitude.

To prove [quantifier elimination](../../../../../../quantifier-elimination.md), first eliminate one existential quantifier from a [quantifier-free formula](../../../../../../quantifier-free-formula.md). Put that formula into disjunctive normal form, so it suffices to consider a conjunction of literals in a new variable $z$ and the parameter variables. There are two possibilities for a witness: $z$ equals one of the parameters, in which case substitution gives a quantifier-free condition; or $z$ is distinct from all of them. In the latter case, the graph axioms reduce all requirements involving $z$ to specified adjacency or nonadjacency to the distinct parameter vertices. A requirement $E(z,z)$ is impossible, and conflicting requirements at equal parameter vertices are impossible. Every other consistent adjacency pattern is realized by the extension axiom.

There are only finitely many equality patterns of the given parameter tuple. For each, consistency of the literals is a quantifier-free condition, including the unchanged relations among the parameters. Their finite disjunction describes exactly when a witness exists. Thus $\exists z\,\theta(z,\mathbf x)$ is equivalent to a [quantifier-free formula](../../../../../../quantifier-free-formula.md) whenever $\theta$ is quantifier-free. [Mathematical induction](../../../../../../mathematical-induction.md) on formulas now eliminates all quantifiers, using $\forall z\,\theta\equiv\neg\exists z\,\neg\theta$. Hence **the random-graph theory eliminates quantifiers**. The extension axioms also yield the usual countable random graph by a back-and-forth construction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
