<h1 id="18h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $\operatorname{char}K=0$, the finite extension $M/K$ is separable. By the [primitive element theorem](../../../../../../primitive-element-theorem.md), write $M=K(\theta)$. The [minimal polynomial](../../../../../../minimal-polynomial.md) of $\theta$ over $K$ has a root in the [algebraically closed field](../../../../../../algebraically-closed-field.md) $L$, so sending $\theta$ to that root defines a $K$-[field embedding](../../../../../../field-embedding.md) $\iota:M\hookrightarrow L$.

The cyclic group $\langle\sigma\rangle$ acts faithfully on $L$ after replacing $d$ by the order of $\sigma$. The [Artin fixed-field theorem](../../../../../../artin-fixed-field-theorem.md) gives

$$
[L:K]=|\langle\sigma\rangle|
$$

and says that $L/K$ is a finite Galois extension with cyclic Galois group $\langle\sigma\rangle$. The image $E=\iota(M)$ is an [intermediate field](../../../../../../intermediate-field.md). Every subgroup of a cyclic group is normal, so the [normal subextension criterion](../../../../../../normal-subextension-criterion.md) shows that $E/K$ is Galois, and its Galois group is a quotient of $\langle\sigma\rangle$, hence cyclic. Transporting this structure through $\iota$ proves that $M/K$ is Galois with cyclic Galois group. This is the [finite extensions of the fixed field of a finite-order automorphism of an algebraically closed field](../../../../../../finite-extensions-of-the-fixed-field-of-a-finite-order-automorphism-of-an-algebraically-closed-field.md) theorem.

Algebraic closedness is necessary. Take $L=\mathbb Q$ and $\sigma=\operatorname{id}$, so $K=L^\sigma=\mathbb Q$, and let $M=\mathbb Q(\sqrt[3]{2})$. The extension has degree three but is not normal, since the two nonreal roots of $X^3-2$ do not belong to $M$. It is therefore not Galois.

## ↑ Ancestors (11)

1. [C](../c.md)
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
