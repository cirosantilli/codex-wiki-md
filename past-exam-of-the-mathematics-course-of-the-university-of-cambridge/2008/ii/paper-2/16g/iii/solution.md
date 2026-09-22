<h1 id="16g/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The intended [closed-term witness property for quantifier-free existential sentences](../../../../../../closed-term-witness-property-for-quantifier-free-existential-sentences.md) needs at least one closed term. Under this hypothesis, suppose the set $\Gamma=\{\neg\phi(t):t\text{ a closed term}\}$ were consistent. By the [Godel completeness theorem](../../../../../../godel-s-completeness-theorem.md), it has a model $M$. Take the [substructure](../../../../../../substructure-of-a-first-order-structure.md) $M_0$ whose elements are the interpretations of closed terms. It is nonempty and closed under every function symbol. Atomic formulas and their negations have the same truth values in $M_0$ as in $M$, and induction extends this to every [quantifier-free formula](../../../../../../quantifier-free-formula.md).

The provable sentence $\exists x\,\phi(x)$ is true in $M_0$ by soundness. Its witness is $t^{M_0}$ for some closed term $t$, so $M\models\phi(t)$, contradicting $M\models\Gamma$. Hence $\Gamma$ is inconsistent. The [compactness theorem](../../../../../../compactness-theorem.md) gives a finite inconsistent subset, so completeness and classical propositional reasoning yield

$$
\boxed{\vdash\phi(t_1)\lor\cdots\lor\phi(t_n).}
$$

Without a constant or nullary function, the printed assertion is false as written: in the equality-only language there are no closed terms, but $\exists x\,(x=x)$ is provable. Then $\Gamma$ is empty and consistent. One may repair the usual theorem by assuming a nonempty set of closed terms or adjoining a fresh constant; the latter proves a witness disjunction in the enlarged language, not the missing closed terms in the original one.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [16G](../../16g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
