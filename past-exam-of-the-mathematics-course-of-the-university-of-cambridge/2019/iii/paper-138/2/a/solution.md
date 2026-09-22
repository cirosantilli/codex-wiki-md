<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $g$ be a [p-regular element](../../../../../../p-regular-element.md). Its eigenvalues on $M$ are roots of unity of order prime to $p$. If $\widehat\lambda_1,\ldots,\widehat\lambda_d$ are their [Teichmuller lifts](../../../../../../teichmuller-representative.md) to characteristic-zero roots of unity, the [Brauer character](../../../../../../brauer-character.md) is

$$
\boxed{\chi_M(g)=\sum_{r=1}^d\widehat\lambda_r.}
$$

It depends only on the conjugacy class of $g$, is additive in short exact sequences, and equals the restriction of an ordinary character whenever the representation lifts.

For linear independence, choose a splitting [p-modular system](../../../../../../p-modular-system.md) and let $P_i$ be the [projective cover](../../../../../../projective-cover.md) of the simple module $S_i$. A projective lattice lifting $P_i$ has an ordinary character $\Phi_i$ that vanishes on p-singular elements. Reduction and ordinary character orthogonality give

$$
\frac1{|G|}\sum_{g\ p\text{-regular}}
\Phi_i(g^{-1})\chi_{S_j}(g)
=\dim\operatorname{Hom}_{kG}(P_i,S_j)
=\delta_{ij},
$$

because $S_i$ is the head of $P_i$. Pairing a relation $\sum_jc_j\chi_{S_j}=0$ with every $\Phi_i$ yields $c_i=0$ for every $i$. Hence

$$
\boxed{\{\chi_{S_i}\}\text{ is linearly independent over }\mathbb C.}
$$

This is the linear-independence part of the [Brauer–Nesbitt theorem](../../../../../../brauer-nesbitt-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
