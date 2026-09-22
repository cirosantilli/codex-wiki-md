<h1 id="19g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [character](../../../../../../character-of-a-representation.md) of a [permutation representation](../../../../../../permutation-representation.md) at $g$ equals the number of points fixed by $g$, because a permuted basis [vector](../../../../../../vector.md) contributes one to the trace exactly when it is fixed. Thus the [character inner product](../../../../../../character-inner-product.md) is

$$
\langle\chi_X,\chi_Y\rangle=\frac1{|G|}\sum_{g\in G}|X^g||Y^g|=\frac1{|G|}\sum_{g\in G}|(X\times Y)^g|.
$$

To identify the last average, count pairs $(g,z)$ with $gz=z$. Each orbit contributes $|G|$, since its number of elements times their common stabilizer size is $|G|$ by the [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md). Therefore

$$
\boxed{\langle\chi_X,\chi_Y\rangle=\#\bigl(G\backslash(X\times Y)\bigr).}
$$

The conjugation in the usual [character inner product](../../../../../../character-inner-product.md) has no effect here because the permutation [characters](../../../../../../character-of-a-representation.md) are real-valued.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [19G](../../19g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
