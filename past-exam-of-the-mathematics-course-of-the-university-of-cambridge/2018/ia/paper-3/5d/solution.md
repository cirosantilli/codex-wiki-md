<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

For $\sigma\in S_n$, let $P_\sigma$ be its [permutation matrix](../../../../../permutation-matrix.md) and define

$$
\operatorname{sgn}(\sigma)=\det P_\sigma\in\{\pm1\}.
$$

Since a transposition exchanges two columns, it has determinant $-1$. Thus any expression of $\sigma$ as $r$ transpositions has sign $(-1)^r$, proving that the parity is independent of the expression. Moreover, $P_{\sigma\tau}=P_\sigma P_\tau$, so the [determinant](../../../../../determinant.md) proves

$$
\operatorname{sgn}(\sigma\tau)=\operatorname{sgn}(\sigma)\operatorname{sgn}(\tau).
$$

Hence the [sign homomorphism](../../../../../sign-homomorphism.md) is a surjective homomorphism for $n\geq2$.

For any homomorphism $\varphi:S_n\to\{\pm1\}$, all transpositions have the same image because they are conjugate. Since transpositions generate $S_n$, image $+1$ would make $\varphi$ trivial. Surjectivity therefore forces every transposition to map to $-1$, and hence **$\varphi=\operatorname{sgn}$**.

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
