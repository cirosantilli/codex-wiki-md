<h1 id="18h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [algebraic closure](../../../../../../algebraic-closure.md) of a field $K$ is an [algebraically closed field](../../../../../../algebraically-closed-field.md) that is an algebraic extension of $K$.

By definition, every element of

$$
\overline{\mathbb Q}
=\{z\in\mathbb C:z\text{ is algebraic over }\mathbb Q\}
$$

is algebraic over $\mathbb Q$, and the question allows us to use that this set is a field. It remains to prove that it is algebraically closed.

Let $f\in\overline{\mathbb Q}[X]$ be nonconstant. Its finitely many coefficients generate a finite extension $E/\mathbb Q$. By the [fundamental theorem of algebra](../../../../../../fundamental-theorem-of-algebra.md), $f$ has a root $z\in\mathbb C$. Since $z$ is a root of a polynomial over $E$, it is algebraic over $E$; since $E/\mathbb Q$ is algebraic, [transitivity of algebraic extensions](../../../../../../transitivity-of-algebraic-extensions.md) makes $z$ algebraic over $\mathbb Q$. Thus $z\in\overline{\mathbb Q}$. Repeating after division by $X-z$ shows that $f$ splits there, so $\overline{\mathbb Q}$ is algebraically closed and is an algebraic closure of $\mathbb Q$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18H](../../18h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
