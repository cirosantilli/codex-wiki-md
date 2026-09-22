<h1 id="a/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An [arithmetic](../../../../../arithmetic-split.md) theory is [one-consistent](../../../../../one-consistency.md) if there is no [bounded arithmetic formula](../../../../../arithmetic-bounded-formula.md) $\delta(x)$ for which it proves $\exists x\,\delta(x)$ and also proves $\neg\delta(\overline n)$ for every standard [natural number](../../../../../natural-number.md) $n$. A finite tuple of existential witnesses can be coded by one [natural number](../../../../../natural-number.md). The associated [Sigma-1 soundness](../../../../../sigma-1-soundness.md) property says that every $\Sigma_1$ sentence it proves is true in the standard [natural numbers](../../../../../natural-number.md).

Suppose first that the theory is one-consistent, but proves a false $\Sigma_1$ sentence $\exists x\,\delta(x)$. For every standard $n$, $\neg\delta(\overline n)$ is then a true bounded sentence. Bounded completeness makes each such sentence a theorem, violating one-consistency.

Conversely suppose the theory is $\Sigma_1$-sound. If it proved both the existential sentence and every negated standard instance, soundness would supply an actual witness $n$. Its positive instance $\delta(\overline n)$ is a true bounded sentence and hence provable. Together with the assumed negative instance this would make the theory inconsistent; an inconsistent theory proves a false $\Sigma_1$ sentence, contrary to soundness. Thus

$$
\boxed{\text{one-consistency}\ \Longleftrightarrow\ \Sigma_1\text{-soundness}}
$$

under the stated bounded-completeness assumption. In particular either condition implies that the theory is a [consistent first-order theory](../../../../../consistent-first-order-theory.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
