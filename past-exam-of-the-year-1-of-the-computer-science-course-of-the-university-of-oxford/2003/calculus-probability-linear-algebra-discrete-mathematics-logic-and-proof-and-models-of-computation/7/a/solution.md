<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First, the [product order](../../../../../product-order.md) is a [partial order](../../../../../partially-ordered-set.md). Reflexivity and transitivity hold in each coordinate. If $(p,q)\le_R(p',q')$ and $(p',q')\le_R(p,q)$, antisymmetry in $P,Q$ gives $p=p'$ and $q=q'$, proving antisymmetry in the product.

Let $D$ be a nonempty [directed set](../../../../../directed-set.md) in $P\times Q$. Its coordinate projections

$$
D_P=\{p:\exists q\;(p,q)\in D\},\qquad D_Q=\{q:\exists p\;(p,q)\in D\}
$$

are [directed sets](../../../../../directed-set.md). For example, if $p_1,p_2\in D_P$, choose $(p_1,q_1),(p_2,q_2)\in D$. Directedness supplies $(p_3,q_3)\in D$ above both, so $p_3\in D_P$ is a common [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md) of $p_1,p_2$ inside $D_P$. The argument for $D_Q$ is identical.

By the assumed [directed-complete partial order](../../../../../directed-complete-partial-order.md) property, $p_* =\sup D_P$ and $q_* =\sup D_Q$ exist. Every $(p,q)\in D$ satisfies $p\le_Pp_*$ and $q\le_Qq_*$, so $(p_*,q_*)$ is an [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md) of $D$. If $(u,v)$ is any other [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md), then $u$ bounds $D_P$ and $v$ bounds $D_Q$. Hence $p_*\le_Pu$, $q_*\le_Qv$, proving leastness. Thus

$$
\boxed{\sup D=(\sup D_P,\sup D_Q),\qquad P\times Q\text{ is directed-complete}.}
$$

The printed definition of a [directed set](../../../../../directed-set.md) also permits $D=\varnothing$.[Printed p. 5, definitions preceding Question 7](../../../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-examination-paper-by-the-university-of-oxford-2003.md) Under that convention, the hypotheses require $P,Q$ to have [least elements](../../../../../least-element.md), namely the [least upper bounds](../../../../../least-upper-bound-in-a-partially-ordered-set.md) of their empty subsets. Their pair is the [least element](../../../../../least-element.md) of the product and is $\sup\varnothing$ there. This handles the empty case as well; under the convention restricting [directed sets](../../../../../directed-set.md) to nonempty sets, only the preceding nonempty argument is needed.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
