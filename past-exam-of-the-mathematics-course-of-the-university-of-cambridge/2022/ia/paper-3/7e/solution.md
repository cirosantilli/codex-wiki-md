<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

A [subgroup](../../../../../subgroup.md) $N\leq G$ is [normal](../../../../../normal-subgroup.md) when

$$
gNg^{-1}=N\qquad(g\in G).
$$

Its left and right cosets then agree, and multiplication

$$
(gN)(hN)=ghN
$$

is well defined on the cosets. The identity is $N$, the inverse of $gN$ is $g^{-1}N$, and associativity descends from $G$, so these cosets form the [quotient group](../../../../../quotient-group.md) $G/N$.

For a [group homomorphism](../../../../../group-homomorphism.md) $\theta:G\to H$, its [kernel](../../../../../kernel-of-a-group-homomorphism.md) and [image](../../../../../image-of-a-group-homomorphism.md) are

$$
\ker\theta=\{g:\theta(g)=e_H\},
\qquad
\operatorname{im}\theta=\{\theta(g):g\in G\}.
$$

The kernel is normal because

$$
\theta(gkg^{-1})
=\theta(g)\theta(k)\theta(g)^{-1}
=e_H
$$

whenever $k\in\ker\theta$. Conversely, if $K\trianglelefteq G$, the quotient map

$$
q:G\longrightarrow G/K,\qquad q(g)=gK,
$$

is a homomorphism with kernel $K$. The image of any homomorphism is closed under products and inverses, so it is a subgroup of $H$. Finally, the map

$$
G/\ker\theta\longrightarrow\operatorname{im}\theta,
\qquad
g\ker\theta\longmapsto\theta(g)
$$

is well defined and bijective and preserves multiplication. This is the [first isomorphism theorem](../../../../../first-isomorphism-theorem.md).

Define

$$
\Phi:(\mathbb R,+)\longrightarrow(\mathbb C\setminus\{0\},\cdot),
\qquad
\Phi(t)=e^{2\pi it}.
$$

[Euler's formula](../../../../../euler-s-formula.md) shows that $\Phi$ is a homomorphism, its image is the [complex unit circle](../../../../../complex-unit-circle.md), and its kernel is $\mathbb Z$. The first isomorphism theorem therefore gives

$$
\boxed{\mathbb R/\mathbb Z\cong S^1}.
$$

The image of $\mathbb Q/\mathbb Z$ consists exactly of the [roots of unity](../../../../../root-of-unity.md): if $t=p/q$, then $\Phi(t)^q=1$, while every element of finite order on the unit circle has an argument that is a rational multiple of $2\pi$.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
