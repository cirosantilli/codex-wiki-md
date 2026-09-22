<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [overspill lemma](../../../../../../overspill-lemma.md) says that if $\mathcal M$ is a [nonstandard model of Peano arithmetic](../../../../../../non-standard-model-of-arithmetic.md) and a definable property $\varphi(x,\bar a)$, possibly with parameters from $\mathcal M$, holds for every standard natural number, then it also holds for some nonstandard element of $\mathcal M$.

Let

$$
A=\{x\in M:\mathcal M\models\varphi(x,\bar a)\}.
$$

If $A$ had no nonstandard member, its complement would be nonempty. The [least-number principle](../../../../../../least-number-principle.md) in [Peano arithmetic](../../../../../../peano-arithmetic.md) would give a least $c\notin A$. Because every standard number belongs to $A$, the element $c$ would be nonstandard and nonzero. Its predecessor $c-1$ would also be nonstandard, so the supposition gives $c-1\notin A$, whereas the minimality of $c$ gives $c-1\in A$. This contradiction proves that $A$ contains a nonstandard element.

Applying this argument to $\psi(y)\equiv\forall x\leq y\,\varphi(x,\bar a)$ gives the useful stronger form: there is a nonstandard $b$ such that $\varphi(x,\bar a)$ holds for every $x\leq b$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
