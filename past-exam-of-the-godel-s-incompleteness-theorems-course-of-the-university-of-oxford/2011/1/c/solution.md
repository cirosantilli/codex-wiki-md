<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $S$ is inconsistent, it proves $\neg R$ by [explosion](../../../../logical-falsity-elimination-rule.md). Conversely, suppose $S$ is consistent and, towards a contradiction, has a proof of $\neg R$ with standard code $n$. Consistency excludes any proof of $R$. In particular, for each $k\leq n$, the closed bounded statement $\neg\operatorname{Prov}(\ulcorner R\urcorner,\overline k)$ is true and is provable in $S$ by [Sigma-1 completeness](../../../../sigma-1-completeness.md). The true bounded statement $\operatorname{Prov}(\ulcorner\neg R\urcorner,\overline n)$ is also provable.

Using the given finite-numeral exhaustion below $\overline n$, these finitely many nonproof facts give

$$
S\vdash\forall y\leq\overline n\,\neg\operatorname{Prov}(\ulcorner R\urcorner,y).
$$

For arbitrary $y$, the given comparison splits into $y\leq\overline n$ or $\overline n\leq y$. In the first case the antecedent $\operatorname{Prov}(\ulcorner R\urcorner,y)$ is false. In the second case the known negative proof at code $\overline n$ supplies the required witness $z\leq y$. Hence $S$ proves

$$
\forall y\left(\operatorname{Prov}(\ulcorner R\urcorner,y)\to\exists z\leq y\,\operatorname{Prov}(\ulcorner\neg R\urcorner,z)\right).
$$

The [Rosser sentence](../../../../rosser-sentence.md) equivalence now gives $S\vdash R$, contradicting consistency. Thus

$$
\boxed{S\nvdash\neg R\iff S\text{ is consistent}.}
$$

Only a fixed finite list of closed bounded facts was used; no assumption that the [first-order theory](../../../../first-order-theory.md) is omega-consistent is needed.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Gödel's incompleteness theorems course of the University of Oxford](../../../split.md)
5. [Gödel's incompleteness theorems course of the University of Oxford](../../../../godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
