<h1 id="33c/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Given a solution $u(t)$, construct $a_j(t)=\tfrac12e^{u_j(t)/2}$ and hence the smooth matrices $L(t)$ and $B(t)$. Let $U(t)$ solve the [linear ordinary differential equation](../../../../../../../linear-ordinary-differential-equation.md)

$$
\dot U(t)=B(t)U(t),
\qquad U(0)=I.
$$

Because $B(t)$ is [skew-symmetric](../../../../../../../skew-symmetric-matrix.md),

$$
\frac d{dt}(U^TU)=U^T(B^T+B)U=0,
$$

so $U(t)$ is an [orthogonal matrix](../../../../../../../orthogonal-matrix.md) and is invertible. Moreover,

$$
\frac d{dt}\left(U^{-1}LU\right)
=U^{-1}\bigl(\dot L-[B,L]\bigr)U=0.
$$

It follows that

$$
\boxed{L(t)=U(t)L(0)U(t)^{-1}.}
$$

Thus the [Lax pair](../../../../../../../lax-pair.md) flow is an [Isospectral Lax equation](../../../../../../../isospectral-lax-equation.md): every $L(t)$ is [similar](../../../../../../../matrix-similarity.md) to $L(0)$ and has the same [eigenvalues](../../../../../../../eigenvalue.md) and [characteristic polynomial](../../../../../../../characteristic-polynomial.md).

Every symmetric function of these constant eigenvalues is a [first integral](../../../../../../../first-integral.md). In particular, the [trace invariants of a Lax equation](../../../../../../../trace-invariants-of-a-lax-equation.md)

$$
I_k=\operatorname{tr}(L^k),
\qquad k=1,2,\ldots,
$$

are constant because the [cyclic property of the trace](../../../../../../../cyclic-property-of-the-trace.md) gives

$$
\frac d{dt}I_k
=k\operatorname{tr}(L^{k-1}[B,L])=0.
$$

For example,

$$
\operatorname{tr}(L^2)=2\sum_{j=1}^{n-1}a_j^2
=\frac12\sum_{j=1}^{n-1}e^{u_j}
$$

is an explicit first integral of equation $(\dagger)$.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [33C](../../../33c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
