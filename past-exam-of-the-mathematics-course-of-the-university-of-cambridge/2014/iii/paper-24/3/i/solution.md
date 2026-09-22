<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The geometric sum gives

$$
\frac{1-\zeta_p^i}{1-\zeta_p}=1+\zeta_p+\cdots+\zeta_p^{i-1}\equiv i\pmod{\pi_K}.
$$

Since $\Phi_p(1)=p$, its factorization at the nonidentity $p$th [roots of unity](../../../../../../root-of-unity.md) yields

$$
p=\prod_{i=1}^{p-1}(1-\zeta_p^i)=\pi_K^{p-1}w,\qquad w=\prod_{i=1}^{p-1}\frac{1-\zeta_p^i}{1-\zeta_p}.
$$

Each factor is a [unit](../../../../../../unit-in-a-ring.md), and [Wilson theorem](../../../../../../wilson-s-theorem.md) gives $w\equiv(p-1)!\equiv-1\pmod{\pi_K}$. Set $u=-w^{-1}$. Then $u$ is a [principal unit](../../../../../../principal-unit.md) and

$$
\boxed{\pi_K^{p-1}=-p u,\qquad u\in1+\pi_K\mathcal O_K.}
$$

The minus sign comes from the product of the nonzero elements of the [residue field](../../../../../../residue-field.md), not from an arbitrary choice of [uniformizer](../../../../../../uniformizer.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
