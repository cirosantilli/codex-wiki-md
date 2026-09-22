<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $P_0=|\psi_0\rangle\langle\psi_0|$ and $Q_0=I-P_0$. [Frustration freeness](../../../../../../../frustration-freeness.md) implies that every local [orthogonal projection](../../../../../../../orthogonal-projection.md) fixes $|\psi_0\rangle$ on both the left and right. Hence

$$
KP_0=P_0K=P_0,\qquad
K=P_0+Q_0KQ_0.
$$

The [spectral gap](../../../../../../../spectral-gap.md) makes $\operatorname{supp}H=Q_0\mathcal H$. The supplied [detectability lemma](../../../../../../../detectability-lemma.md) gives

$$
q:=\left(1+\frac{\Delta}{2}\right)^{-1/3}<1,\qquad
\|Q_0KQ_0\|\leq q.
$$

Consequently

$$
\boxed{\|K^m-P_0\|\leq q^m=e^{-\alpha m},
\qquad
\alpha=\frac13\ln\left(1+\frac{\Delta}{2}\right).}
$$

No assumption that $K$ is Hermitian or normal is needed.

A stronger estimate will keep this same $\alpha$ when we count the two projection layers in (ii). On $Q_0\mathcal H$, put $P=P_{\rm odd}-P_0$ and $Q=P_{\rm even}-P_0$. They are [orthogonal projections](../../../../../../../orthogonal-projection.md), with $\|PQ\|\leq q$. For $m\geq1$,

$$
(PQ)^m=PQ(QPQ)^{m-1},\qquad
\|QPQ\|=\|PQ\|^2,
$$

so the [powers of a product of two orthogonal projections](../../../../../../../powers-of-a-product-of-two-orthogonal-projections.md) satisfy

$$
\boxed{\|K^m-P_0\|\leq q^{\,2m-1}.}
$$

This extra estimate uses the projection structure, rather than generic submultiplicativity alone.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 67](../../../../paper-67-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
