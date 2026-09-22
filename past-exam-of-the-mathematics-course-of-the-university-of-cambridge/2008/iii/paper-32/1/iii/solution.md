<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $\alpha=44^{1/11}$ and $L=\mathbb Q(\alpha)$. The [Eisenstein criterion](../../../../../../eisenstein-criterion.md) at $11$ shows that $X^{11}-44$ is an [irreducible polynomial](../../../../../../irreducible-polynomial.md), so $[L:\mathbb Q]=11$. Its derivative is $11X^{10}$, and the [polynomial discriminant](../../../../../../polynomial-discriminant.md) is

$$
\operatorname{disc}(X^{11}-44)=-11^{11}44^{10}=-2^{20}11^{21}.
$$

The [discriminant-index formula for an integral lattice](../../../../../../discriminant-index-formula-for-an-integral-lattice.md) implies that the [field discriminant](../../../../../../field-discriminant.md) has no prime divisor outside $\{2,11\}$. By the [discriminant obstruction to ramification](../../../../../../discriminant-obstruction-to-ramification.md), every other prime is unramified.

To prove that neither candidate disappears through an index correction, let $\mathfrak p$ lie above $p\in\{2,11\}$ and normalize its [valuation](../../../../../../valuation.md) to have value group $\mathbb Z$. If $e=e_{\mathfrak p/p}$, the relation $\alpha^{11}=44$ gives

$$
11v_{\mathfrak p}(\alpha)=e\,v_p(44)=\begin{cases}2e,&p=2,\\e,&p=11.\end{cases}
$$

In both cases $11\mid e$. The [fundamental identity for prime decomposition](../../../../../../fundamental-identity-for-prime-decomposition.md), $\sum_{\mathfrak p\mid p}e_{\mathfrak p/p}f_{\mathfrak p/p}=11$, now forces exactly one [prime ideal](../../../../../../prime-ideal.md) above each candidate, with $e=11$ and $f=1$. This is [ramification forced by a coprime root valuation](../../../../../../ramification-forced-by-a-coprime-root-valuation.md); at $2$ it avoids an invalid direct application of the [Eisenstein criterion](../../../../../../eisenstein-criterion.md), since $4\mid44$. Hence

$$
\boxed{\text{The ramified rational primes are exactly }2\text{ and }11;\ \text{both are totally ramified}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
