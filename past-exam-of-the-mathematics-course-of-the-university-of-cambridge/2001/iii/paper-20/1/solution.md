<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

We first give an auxiliary-integral proof, rather than deducing both requested results from a theorem only stated later. The following [symmetric Hermite integral obstruction](../../../../../symmetric-hermite-integral-obstruction.md) will do both jobs. Suppose

$$
k+\sum_{j=1}^s b_je^{\beta_j}=0,
$$

where $k\ne0$ and $b_j$ are [integers](../../../../../integer.md), the distinct nonzero algebraic exponents form a Galois-stable set, and their weights are invariant under conjugation. Choose $P\in\mathbb Z[X]$ vanishing at those exponents, with $P(0)\ne0$, and a positive [integer](../../../../../integer.md) $c$ for which every $c\beta_j$ is an [algebraic integer](../../../../../algebraic-integer.md). For a large [prime number](../../../../../prime-number.md) $p$, let

$$
D=(\deg P+1)p-1,\qquad f_p(X)=\frac{c^DX^{p-1}P(X)^p}{(p-1)!},\qquad F_p(X)=\sum_{r=0}^D f_p^{(r)}(X).
$$

At zero, derivatives below $p-1$ vanish; the derivative of order $p-1$ equals $c^DP(0)^p$. All higher derivatives at zero are [integers](../../../../../integer.md) divisible by $p$. At each $\beta_j$, derivatives below $p$ vanish and all higher derivatives belong to $p\mathcal O_L$ in a Galois [splitting field](../../../../../splitting-field.md) $L$. Indeed their coefficients contain $r!/(p-1)!$, divisible by $p$ for $r\ge p$, and every $c^D\beta_j^u$ is integral for $u\le D$. Consequently

$$
I_p=kF_p(0)+\sum_jb_jF_p(\beta_j)\in\mathbb Z,\qquad I_p\equiv kc^DP(0)^p\pmod p.
$$

Galois invariance makes the sum rational, and integrality makes it an [integer](../../../../../integer.md). For [prime numbers](../../../../../prime-number.md) not dividing $kcP(0)$ it is nonzero.

But $F_p-F_p'=f_p$, so integration along the straight segment to $\beta$ gives

$$
e^\beta F_p(0)-F_p(\beta)=\int_0^\beta e^{\beta-z}f_p(z)\,dz.
$$

Multiply by the weights and use the assumed exponential relation. This expresses $-I_p$ as the sum of these integrals. On the finitely many fixed segments, their absolute values are at most $C^p/(p-1)!$ for a fixed $C$: all [polynomial](../../../../../polynomial-split.md) and exponential factors have fixed bounds, and $D$ is linear in $p$. Thus $|I_p|\to0$, contradicting its being a nonzero [integer](../../../../../integer.md). The obstruction is proved.

If $e$ were algebraic, an integral [polynomial](../../../../../polynomial-split.md) relation would give $a_0+\sum_{j=1}^s a_je^j=0$ with $a_0\ne0$. [Integer](../../../../../integer.md) exponents and weights satisfy the obstruction, so **$e$ is transcendental**.

If $\pi$ were algebraic, put $\alpha=i\pi$ and let $\alpha_1,\ldots,\alpha_d$ be its algebraic conjugates. Since $1+e^\alpha=0$, the product $\prod_j(1+e^{\alpha_j})$ vanishes. Expand it and collect equal subset sums. The zero sums contribute a positive [integer](../../../../../integer.md) $k\ge1$; the nonzero sums give a Galois-stable list $\beta_j$ with positive integral multiplicities. This is precisely the prohibited relation. Hence **$\pi$ is transcendental**.

The general [Lindemann–Weierstrass theorem](../../../../../lindemann-weierstrass-theorem.md) states that exponentials of distinct [algebraic numbers](../../../../../algebraic-number.md) are linearly independent over $\overline{\mathbb Q}$. Suppose the sine quotient were algebraic, say $\gamma$. The denominator is nonzero: $\sin\beta=0$ would give a forbidden relation between the exponentials of the distinct [algebraic numbers](../../../../../algebraic-number.md) $i\beta,-i\beta$. The quotient identity would give

$$
e^{i\alpha}-e^{-i\alpha}-\gamma e^{i\beta}+\gamma e^{-i\beta}=0.
$$

The four exponents are distinct under the stated nonzero and non-opposite assumptions, so this also contradicts [linear independence](../../../../../linear-independence.md). Therefore

$$
\boxed{\sin\alpha/\sin\beta\text{ is transcendental}}.
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
