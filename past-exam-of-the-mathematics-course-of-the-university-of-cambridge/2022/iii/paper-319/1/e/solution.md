<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The family

$$
\widehat U(t)=e^{-\omega t}U(t)
$$

inherits the identity, [semigroup property](../../../../../../semigroup-property.md), and [strong continuity](../../../../../../strong-continuity.md) from $U$, while

$$
\|\widehat U(t)u\|\leq M\|u\|.
$$

Its difference quotient satisfies

$$
\frac{\widehat U(h)u-u}{h}
=e^{-\omega h}\frac{U(h)u-u}{h}
+\frac{e^{-\omega h}-1}{h}u\longrightarrow Au-\omega u
$$

for $u\in D(A)$. Conversely, existence of this limit implies existence of the generator limit for $U$, so $D(\widehat A)=D(A)$ and

$$
\boxed{\widehat A=A-\omega I}.
$$

This is the [exponentially shifted semigroup](../../../../../../exponentially-shifted-semigroup.md) construction.

The [Hille-Yosida theorem](../../../../../../hille-yosida-theorem.md) in the uniformly bounded case says that a [linear operator](../../../../../../linear-operator.md) $B$ on a [Banach space](../../../../../../banach-space-split.md) generates a [C0-semigroup](../../../../../../c0-semigroup.md) with $\|e^{tB}\|\leq M$ if and only if:


- $B$ is a [closed linear operator](../../../../../../closed-linear-operator.md) whose domain is a [dense subset](../../../../../../dense-set.md) of the [Banach space](../../../../../../banach-space-split.md);
- $(0,\infty)\subseteq\rho(B)$;
- for every $\lambda>0$ and integer $n\geq1$,


$$
\boxed{\|\lambda^n(\lambda I-B)^{-n}\|\leq M}.
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 319](../../../paper-319-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
