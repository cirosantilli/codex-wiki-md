<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The characteristic of $K$ is either a prime $p$ or zero. In characteristic $p$, it is a [finitely generated algebra](../../../../../../finitely-generated-algebra.md) over $\mathbb F_p$. The course's [Zariski lemma](../../../../../../zariski-s-lemma.md) says that a [field](../../../../../../field.md) finitely generated as an algebra over a [field](../../../../../../field.md) is a finite algebraic extension of that [field](../../../../../../field.md). Therefore

$$
\boxed{\operatorname{char}K=p\Longrightarrow |K|=p^d\text{ for some finite }d}.
$$

It remains to exclude characteristic zero. Write $K=\mathbb Z[a_1,\ldots,a_m]$. Because $K$ is then a [field](../../../../../../field.md) containing $\mathbb Q$, also $K=\mathbb Q[a_1,\ldots,a_m]$. [Zariski lemma](../../../../../../zariski-s-lemma.md) makes $K/\mathbb Q$ finite algebraic. Each $a_i$ has a monic equation with rational coefficients. Choose a positive integer $N$ clearing all their coefficient denominators. Each $a_i$ is then integral over $A=\mathbb Z[1/N]$, so $A[a_1,\ldots,a_m]$ is integral over $A$. This algebra equals $K$: it contains the given integer algebra $K$, and $1/N$ already lies in the [field](../../../../../../field.md) $K$.

An [integral field extension forces the base domain to be a field](../../../../../../integral-field-extension-forces-the-base-domain-to-be-a-field.md). To see it here, for a nonzero $a\in A$ its inverse in $K$ satisfies

$$
(a^{-1})^r+c_{r-1}(a^{-1})^{r-1}+\cdots+c_0=0,\qquad c_i\in A.
$$

Multiplying by $a^{r-1}$ gives

$$
a^{-1}=-(c_{r-1}+c_{r-2}a+\cdots+c_0a^{r-1})\in A.
$$

Thus $A$ would be a [field](../../../../../../field.md). But choose a prime $\ell\nmid N$. Reduction modulo $\ell$ is a well-defined map $\mathbb Z[1/N]\to\mathbb F_\ell$, so the nonzero element $\ell$ is not invertible in $A$. This contradiction rules out characteristic zero. Therefore the [finite-field theorem for finitely generated integer algebras](../../../../../../finite-field-theorem-for-finitely-generated-integer-algebras.md) yields

$$
\boxed{K\text{ is a finite field}}.
$$

This uses [Zariski lemma](../../../../../../zariski-s-lemma.md) and elementary integrality, not a claim that a [field](../../../../../../field.md) merely finitely generated as a [field extension](../../../../../../field-extension.md) must be algebraic.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
