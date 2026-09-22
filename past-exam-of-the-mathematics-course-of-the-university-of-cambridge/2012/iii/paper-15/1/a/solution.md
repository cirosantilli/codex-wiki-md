<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [cotangent bundle](../../../../../../cotangent-bundle.md) coordinates $(q^1,\ldots,q^n,p_1,\ldots,p_n)$, the [Liouville one-form](../../../../../../canonical-one-form-on-a-cotangent-bundle.md) and the canonical [symplectic form](../../../../../../symplectic-form.md) are

$$
\alpha=\sum_i p_i\,dq^i,\qquad
\omega=-d\alpha=\sum_i dq^i\wedge dp_i.
$$

The [twisted cotangent symplectic form](../../../../../../twisted-cotangent-symplectic-form.md) is closed: [pullback of a differential form](../../../../../../pullback-of-a-differential-form.md) commutes with the [exterior derivative](../../../../../../exterior-derivative.md), so

$$
d\omega_\sigma=d\omega+\pi^*(d\sigma)=0.
$$

To prove the form is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md), write a tangent vector in these coordinates as $(u,v)$ and test its pairing with an arbitrary vertical vector $(0,w)$. The base [differential two-form](../../../../../../2-form.md) has zero pairing with vertical vectors, hence

$$
\omega_\sigma((u,v),(0,w))=u^iw_i.
$$

A vector in the [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md) therefore has $u=0$. Pairing it next with every $(z,0)$ gives $-z^iv_i=0$, so $v=0$. Thus the kernel is zero at every point, independently of the size or rank of $\sigma$. Together with closedness, this proves **$\omega_\sigma$ is a [symplectic form](../../../../../../symplectic-form.md)**. The argument is local only for convenience; the [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) property is intrinsic and the coordinate charts cover the whole [cotangent bundle](../../../../../../cotangent-bundle.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
