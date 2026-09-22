<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Ostrowski theorem](../../../../../../ostrowski-s-theorem.md) says that every nontrivial [absolute value on a field](../../../../../../absolute-value-algebra.md) defined on $\mathbb Q$ is equivalent either to the usual absolute value or to $|\cdot|_p$ for a unique prime $p$.

Let an absolute value on the [number field](../../../../../../number-field.md) $K$ extend $|\cdot|_p$. Its valuation ring determines

$$
\mathfrak p=\{x\in\mathcal O_K:|x|<1\},
$$

a [prime ideal](../../../../../../prime-ideal.md) satisfying $\mathfrak p\cap\mathbb Z=(p)$. Conversely, each prime $\mathfrak p$ above $p$ defines the normalized absolute value

$$
|x|_{\mathfrak p}=p^{-v_{\mathfrak p}(x)/e_{\mathfrak p}},
$$

where $e_{\mathfrak p}=v_{\mathfrak p}(p)$. It restricts to $|\cdot|_p$. The correspondence between extensions and primes follows either from the valuation ring or from [local factorization and extended absolute values](../../../../../../local-factorization-and-extended-absolute-values.md); distinct primes give inequivalent valuations. Thus these $|\cdot|_{\mathfrak p}$ are exactly the extensions, up to equivalence.

For the tensor-product assertion, choose a [primitive element of a field extension](../../../../../../primitive-element-of-a-field-extension.md) $\alpha$ for $K/\mathbb Q$, with minimal polynomial $f$. Because number fields are separable, over $\mathbb Q_p$ it factors into distinct irreducibles

$$
f=f_1\cdots f_r,
$$

indexed by the primes $\mathfrak p\mid p$. The [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) gives

$$
K\otimes_{\mathbb Q}\mathbb Q_p
\cong\mathbb Q_p[X]/(f)
\cong\prod_{i=1}^r\mathbb Q_p[X]/(f_i).
$$

The $i$th factor is the [completion of a number field at a prime ideal](../../../../../../completion-of-a-number-field-at-a-prime-ideal.md) $K_{\mathfrak p_i}$. Under these identifications the isomorphism is the natural diagonal map $x\otimes a\mapsto(ax)_{\mathfrak p}$, proving the [p-adic tensor decomposition of a number field](../../../../../../p-adic-tensor-decomposition-of-a-number-field.md)

$$
\boxed{K\otimes_{\mathbb Q}\mathbb Q_p\cong\prod_{\mathfrak p\mid p}K_{\mathfrak p}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
