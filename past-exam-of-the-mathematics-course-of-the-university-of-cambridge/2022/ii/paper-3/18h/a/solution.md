<h1 id="18h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The automorphisms $1,\sigma,\ldots,\sigma^{n-1}$ are distinct and hence linearly independent as maps $L\to L$ by the [linear independence of distinct field embeddings](../../../../../../linear-independence-of-distinct-field-embeddings.md). Therefore the operator

$$
T=\sum_{j=0}^{n-1}\zeta^{-j}\sigma^j
$$

is not the zero map. Choose $\beta\in L$ for which $\alpha=T(\beta)\ne0$. Reindexing the sum and using $\sigma^n=1$ gives

$$
\sigma(\alpha)
=\sum_{j=0}^{n-1}\zeta^{-j}\sigma^{j+1}(\beta)
=\zeta\alpha.
$$

This is the [Lagrange resolvent eigenvector for a cyclic field automorphism](../../../../../../lagrange-resolvent-eigenvector-for-a-cyclic-field-automorphism.md).

Let $F=L^\sigma$ be the [fixed field](../../../../../../fixed-field.md). Since $\sigma(\alpha^n)=\alpha^n$, the element $\alpha$ is a root of

$$
X^n-\alpha^n\in F[X].
$$

Its orbit under $\langle\sigma\rangle$ is

$$
\alpha,\zeta\alpha,\ldots,\zeta^{n-1}\alpha,
$$

and these $n$ elements are distinct because $\alpha\ne0$ and $\zeta$ is a [primitive root of unity](../../../../../../primitive-root-of-unity.md). Hence the [minimal polynomial](../../../../../../minimal-polynomial.md) has at least $n$ distinct roots. It also divides the displayed degree-$n$ polynomial, so

$$
\boxed{m_{\alpha,F}(X)=X^n-\alpha^n}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
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
