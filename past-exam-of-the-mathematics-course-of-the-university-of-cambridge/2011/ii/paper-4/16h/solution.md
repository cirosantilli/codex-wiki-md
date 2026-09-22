<h1 id="16h/solution">Solution</h1>

↑ **Parent:** [16H](../16h.md)

The [cumulative hierarchy](../../../../../cumulative-hierarchy.md) is defined by [transfinite recursion](../../../../../transfinite-recursion.md):

$$
\boxed{V_0=\varnothing,\qquad V_{\alpha+1}=\mathcal P(V_\alpha),\qquad V_\lambda=\bigcup_{\alpha<\lambda}V_\alpha\ \text{for limit }\lambda.}
$$

Prove transitivity and nesting together by [transfinite induction](../../../../../transfinite-induction.md). The empty set is transitive. If $V_\alpha$ is transitive, each $x\in V_\alpha$ satisfies $x\subseteq V_\alpha$, so $V_\alpha\subseteq\mathcal P(V_\alpha)$. If $y\in x\in\mathcal P(V_\alpha)$, then $y\in V_\alpha\subseteq\mathcal P(V_\alpha)$; thus the successor stage is transitive. At a limit, if $y\in x\in V_\lambda$, choose an earlier stage containing $x$ and apply its transitivity. The union is transitive and contains every earlier stage. These observations also give $V_\alpha\subseteq V_\beta$ for all $\alpha\le\beta$.

By [Axiom of foundation](../../../../../axiom-of-regularity.md) and well-founded recursion, define the [rank of a set](../../../../../rank-of-a-set.md) by $\operatorname{rank}(x)=\sup\{\operatorname{rank}(y)+1:y\in x\}$. [Axiom schema of replacement](../../../../../axiom-schema-of-replacement.md) ensures this is an [ordinal](../../../../../ordinal.md). Induction shows every element of $x$ lies in $V_{\operatorname{rank}(x)}$, so

$$
\boxed{x\in V_{\operatorname{rank}(x)+1}.}
$$

Thus every set appears in the hierarchy; the argument uses foundation, not the existence of a set containing all sets.

If $\operatorname{rank}(x)=\beta$, every subset of $x$ has rank at most $\beta$, while $x$ itself belongs to $\mathcal P(x)$. Consequently

$$
\boxed{\operatorname{rank}(\mathcal P(x))=\beta+1.}
$$

Only successor [ordinals](../../../../../ordinal.md) occur. Conversely $\operatorname{rank}(V_\beta)=\beta$, so choosing $x=V_\beta$ realizes every successor $\beta+1$. **The exact answer is all successor [ordinals](../../../../../ordinal.md), excluding zero and nonzero limit [ordinals](../../../../../ordinal.md).**

## ↑ Ancestors (10)

1. [16H](../16h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
