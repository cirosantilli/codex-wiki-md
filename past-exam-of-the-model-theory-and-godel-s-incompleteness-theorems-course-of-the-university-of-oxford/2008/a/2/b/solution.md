<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If PA is inconsistent, every desired conclusion is already a theorem, so it suffices to analyze the [first-order consistent](../../../../../first-order-consistency.md) case. Use $Q(u,v)$ for the bounded [arithmetical proof relation](../../../../../arithmetical-proof-relation.md) and $\operatorname{neg}(u)$ for the code of the [negation](../../../../../negation.md) of the [logical formula](../../../../../logical-formula.md) coded by $u$.

Suppose $PA\vdash E_n$ and let $m$ be the code of an actual [formal proof](../../../../../formal-proof.md). By [first-order consistency](../../../../../first-order-consistency.md) there is no [formal proof](../../../../../formal-proof.md) of $\neg E_n$, in particular none with code at most $m$. Thus

$$
Q(\bar n,\bar m)\wedge(\forall z\le\bar m)\neg Q(\overline{\operatorname{neg}(n)},z)
$$

is a true [bounded arithmetic sentence](../../../../../bounded-arithmetic-sentence.md). [Bounded completeness of an arithmetic theory](../../../../../bounded-completeness-of-an-arithmetic-theory.md) proves it in PA, and existential introduction gives $PA\vdash\operatorname{Pr}_{PA}^*(\bar n)$.

Conversely suppose $PA\vdash\neg E_n$ and choose an actual [formal proof](../../../../../formal-proof.md) code $k$ of that [negation](../../../../../negation.md). [First-order consistency](../../../../../first-order-consistency.md) excludes every [formal proof](../../../../../formal-proof.md) of $E_n$, so each of the finitely many statements $\neg Q(\bar n,\bar j)$ for $j<k$ is true and provable. The supplied finite-case theorem permits PA to combine them into the assertion that no [formal proof](../../../../../formal-proof.md) code below $k$ proves $E_n$.

PA also proves $Q(\overline{\operatorname{neg}(n)},\bar k)$. For any candidate [formal proof](../../../../../formal-proof.md) code $v\ge\bar k$, this one code already refutes the universal no-earlier-negation condition in the Rosser [predicate symbol](../../../../../predicate-symbol.md). For $v<\bar k$, the finite verification refutes its positive [formal proof](../../../../../formal-proof.md) condition. The supplied order dichotomy and finite-case expansion cover all $v$. Therefore

$$
\boxed{PA\vdash\neg\operatorname{Pr}_{PA}^*(\bar n).}
$$

The argument uses bounded verification of a finite initial segment and one fixed counter-witness beyond it; it does not infer that PA proves the absence of all ordinary [formal proofs](../../../../../formal-proof.md) merely from [first-order consistency](../../../../../first-order-consistency.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
