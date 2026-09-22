<h1 id="8b/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An [eigenvalue](../../../../../../../eigenvalue.md) can be complex even though $P$ is real, so use the complex [Hermitian inner product](../../../../../../../hermitian-form.md). For a nonzero complex [eigenvector](../../../../../../../eigenvector.md) $\mathbf v$, the real [orthogonal matrix](../../../../../../../orthogonal-matrix.md) also satisfies $P^*P=P^TP=I$. Hence

$$
\|\mathbf v\|^2=\|P\mathbf v\|^2=|\lambda|^2\|\mathbf v\|^2,
$$

and **$\boxed{|\lambda|=1}$**. Taking complex conjugates in $P\mathbf v=\lambda\mathbf v$ gives $P\overline{\mathbf v}=\overline\lambda\,\overline{\mathbf v}$ because $P$ is real. The conjugate vector is nonzero, so **$\boxed{\lambda^*=\overline\lambda\text{ is also an eigenvalue}}$**.

For the unheaded geometrical conclusion, the third [eigenvalue](../../../../../../../eigenvalue.md) of $Q$ must be real: nonreal [eigenvalues](../../../../../../../eigenvalue.md) of a real matrix occur in conjugate pairs. Its modulus is one, so it is $1$ or $-1$. Exact [algebraic multiplicity](../../../../../../../algebraic-multiplicity.md) two for $1$ excludes a third $1$, leaving $-1$. By the supplied diagonalisability fact, the $1$-[eigenspace](../../../../../../../eigenspace.md) is a two-dimensional [plane](../../../../../../../plane.md) and the $-1$-[eigenspace](../../../../../../../eigenspace.md) is a line. They are [orthogonal](../../../../../../../orthogonal-vectors.md): preservation of the [inner product](../../../../../../../inner-product.md) between a fixed vector and a negated vector gives $\mathbf u\cdot\mathbf v=-\mathbf u\cdot\mathbf v$. Therefore **$Q$ is the [orthogonal reflection](../../../../../../../reflection-in-a-hyperplane.md) in its fixed [plane](../../../../../../../plane.md)**. It fixes the two tangential directions and reverses the normal direction; with unit normal $\mathbf n$, $Q=I-2\mathbf n\mathbf n^T$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8B](../../../8b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
