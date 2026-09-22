<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [character of an algebra](../../../../../../character-of-an-algebra.md) is a nonzero multiplicative complex [linear functional](../../../../../../linear-functional.md) $\phi:A\to\mathbb C$. Nonzeroness and multiplicativity force $\phi(1)=1$, so it is onto $\mathbb C$. Its kernel is an [ideal](../../../../../../ideal.md), and the quotient is the [field](../../../../../../field.md) $\mathbb C$, making the kernel maximal.

[Continuity](../../../../../../continuous-function.md) is automatic. The element $a-\phi(a)1$ cannot be invertible, since applying $\phi$ to an inverse equation would give $0=1$. On the other hand $a-\lambda1$ is invertible whenever $|\lambda|>\|a\|$, by the [Neumann series](../../../../../../neumann-series.md). Hence $|\phi(a)|\leq\|a\|$, the [automatic continuity of characters](../../../../../../automatic-continuity-of-characters.md) bound.

Conversely let $M$ be a [maximal ideal](../../../../../../maximal-ideal.md). Its closure is an [ideal](../../../../../../ideal.md), because multiplication is continuous. That closure is proper: otherwise there would be $m\in M$ with $\|1-m\|<1$, making $m$ invertible by the [Neumann series](../../../../../../neumann-series.md) and forcing $M=A$. Maximality gives $\overline M=M$. The quotient $A/M$ is consequently a [Banach algebra](../../../../../../banach-algebra-split.md). It is a division [algebra](../../../../../../algebra-split.md): for any $a\notin M$, the larger [ideal](../../../../../../ideal.md) $M+Aa$ equals $A$, so the class of $a$ has an inverse. By the [Gelfand-Mazur theorem](../../../../../../gelfand-mazur-theorem.md), $A/M\cong\mathbb C$, and its quotient map gives a continuous [character of an algebra](../../../../../../character-of-an-algebra.md) with kernel $M$.

If two [algebra characters](../../../../../../character-of-an-algebra.md) have the same kernel, then $a-\phi(a)1$ lies in the second kernel, giving $\psi(a)=\phi(a)$ for every $a$. Thus

$$
\boxed{\Phi_A\longrightarrow\mathcal M_A,\qquad\phi\longmapsto\ker\phi}
$$

is a bijection. This proves that [maximal ideals of a commutative complex unital Banach algebra are character kernels](../../../../../../maximal-ideals-of-a-commutative-complex-unital-banach-algebra-are-character-kernels.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
