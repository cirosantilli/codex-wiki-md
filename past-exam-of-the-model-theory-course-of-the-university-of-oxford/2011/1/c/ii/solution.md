<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [partial type](../../../../../partial-type.md) $p(\mathbf x)$ is a set of $L$-[first-order formulas](../../../../../first-order-formula.md) in a fixed tuple $\mathbf x=(x_1,\ldots,x_n)$ jointly consistent with $T$. A [complete type](../../../../../complete-type.md), the usual meaning of an $n$-type here, is maximal among such consistent sets: for each [first-order formula](../../../../../first-order-formula.md) $\varphi(\mathbf x)$ it contains exactly one of $\varphi,\neg\varphi$.

Add new constants $\mathbf c$ and consider

$$
T\cup\{\varphi(\mathbf c):\varphi\in p\}.
$$

Every finite subset is satisfiable by consistency of the type. The [compactness theorem](../../../../../compactness-theorem.md) gives a [first-order model](../../../../../model-of-a-first-order-theory.md) of the full set. Its $L$-reduct is a [first-order model](../../../../../model-of-a-first-order-theory.md) of $T$, and the interpretations of $\mathbf c$ realize $p$. This proof applies to partial as well as complete types.

For a [complete theory](../../../../../complete-theory.md) in a countable language, **the types realized in every [first-order model](../../../../../model-of-a-first-order-theory.md) are exactly the isolated types**. An [isolated type](../../../../../isolated-type.md) has a consistent [first-order formula](../../../../../first-order-formula.md) $\theta\in p$ such that $T\models\forall\mathbf x(\theta\to\varphi)$ for every $\varphi\in p$. Completeness forces $T\models\exists\mathbf x\theta$, so every [first-order model](../../../../../model-of-a-first-order-theory.md) realizes $p$; the converse is the [omitting types theorem](../../../../../omitting-types-theorem.md). Countability is a hypothesis of that converse, not of the preceding compactness realization argument. For a [partial type](../../../../../partial-type.md) the corresponding criterion is an isolating consistent [first-order formula](../../../../../first-order-formula.md), together with its existence in every [first-order model](../../../../../model-of-a-first-order-theory.md); it need not itself belong to the [partial type](../../../../../partial-type.md).

If $T$ is not complete, no one complete $n$-type can be realized in every [first-order model](../../../../../model-of-a-first-order-theory.md) of $T$: a [complete type](../../../../../complete-type.md) decides sentences, and two completions of $T$ disagree on some sentence. Thus the completeness and countability hypotheses must be retained when using the isolated-type characterization.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
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
