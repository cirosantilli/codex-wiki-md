<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [character of an algebra](../../../../../../character-of-an-algebra.md) is a nonzero multiplicative complex-linear functional $\varphi:A\to\mathbb C$, and the [character space of an algebra](../../../../../../character-space-of-an-algebra.md) is the set $\Phi_A$ of all such characters. Since $A$ is unital, $\varphi(1)=1$. Moreover $\varphi(a)\in\sigma_A(a)$: otherwise $a-\varphi(a)1$ would be invertible, while applying $\varphi$ to its inverse identity would give $0=1$. The [spectral radius](../../../../../../spectral-radius.md) estimate therefore yields

$$
|\varphi(a)|\leq r(a)\leq\|a\|.
$$

Thus every character is continuous and has norm one.

Let $M$ be a [maximal ideal](../../../../../../maximal-ideal.md). Its norm closure is again an ideal. It cannot equal $A$, because then some $m\in M$ would satisfy $\|1-m\|<1$, making $m$ invertible by the [Neumann series](../../../../../../neumann-series.md) and forcing $M=A$. Hence $M$ is closed. The quotient $A/M$ is a complex unital Banach division algebra, so the [Gelfand-Mazur theorem](../../../../../../gelfand-mazur-theorem.md) identifies it with $\mathbb C$. Composing the quotient map with this isomorphism gives a character with kernel $M$. Conversely, a character kernel is maximal because its quotient is $\mathbb C$.

Now $\lambda\in\sigma_A(x)$ exactly when $x-\lambda1$ is not invertible, equivalently when it lies in some maximal ideal. The preceding result turns that ideal into $\ker\varphi$, giving $\varphi(x)=\lambda$. The reverse implication follows from the first paragraph, so

$$
\sigma_A(x)=\{\varphi(x):\varphi\in\Phi_A\}.
$$

The [Gelfand topology](../../../../../../gelfand-topology.md) is the [weak-star topology](../../../../../../weak-star-topology.md) on $\Phi_A\subseteq A^*$. The [Gelfand transform](../../../../../../gelfand-representation.md) is

$$
x\longmapsto\widehat x,
\qquad
\widehat x(\varphi)=\varphi(x).
$$

Its values are continuous by the definition of the topology, and multiplicativity and linearity of characters show that it is a unital algebra homomorphism. Finally

$$
\|\widehat x\|_\infty=\sup_{\varphi\in\Phi_A}|\varphi(x)|\leq\|x\|,
$$

so it is continuous.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
