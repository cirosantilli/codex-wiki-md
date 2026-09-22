<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

We first give an auxiliary-[polynomial](../../../../../polynomial-split.md) proof, rather than assuming a transcendence theorem for exponentials. Suppose $i\pi$ were algebraic, and let $\delta_1=i\pi,\delta_2,\ldots,\delta_t$ be its conjugates. Since the first factor vanishes,

$$
\prod_{\nu=1}^t(1+e^{\delta_\nu})=0.
$$

Expand and collect equal subset sums of the $\delta_\nu$. This gives $k+\sum_{j=1}^s b_je^{\beta_j}=0$, where $k\geq1$ counts the zero sums, the $\beta_j$ are distinct nonzero [algebraic numbers](../../../../../algebraic-number.md), and each $b_j$ is a positive [integer](../../../../../integer.md). The exponents and their weights are invariant under every Galois permutation.

Choose a positive [integer](../../../../../integer.md) $c$ such that all $c\beta_j$ are [algebraic integers](../../../../../algebraic-integer.md). Their Galois-invariant [monic polynomial](../../../../../monic-polynomial.md) $R(u)=\prod_j(u-c\beta_j)$ has rational algebraic-[integer](../../../../../integer.md) coefficients, hence lies in $\mathbb Z[u]$. Its constant term $A=R(0)$ is a nonzero [integer](../../../../../integer.md). For a [prime](../../../../../prime-number.md) $p$ define

$$
f_p(z)=\frac{(cz)^{p-1}R(cz)^p}{(p-1)!},\qquad
F_p(z)=\sum_{h=0}^{(s+1)p-1}f_p^{(h)}(z).
$$

At each $\beta_j$, derivatives below order $p$ vanish. Every higher derivative is $c^h h!/(p-1)!$ times an [algebraic integer](../../../../../algebraic-integer.md), so $F_p(\beta_j)$ is divisible by $p$ in the ring of [algebraic integers](../../../../../algebraic-integer.md). At zero the only derivative not visibly divisible by $p$ is the one of order $p-1$, and thus

$$
F_p(0)\in\mathbb Z,\qquad F_p(0)\equiv c^{p-1}A^p\pmod p.
$$

Galois invariance makes $\sum_jb_jF_p(\beta_j)$ rational; it is therefore an [integer](../../../../../integer.md), divisible by $p$. Consequently

$$
S_p=kF_p(0)+\sum_jb_jF_p(\beta_j)\in\mathbb Z,\qquad
S_p\equiv kc^{p-1}A^p\pmod p.
$$

For every [prime](../../../../../prime-number.md) not dividing $kcA$, this is a nonzero [integer](../../../../../integer.md).

The finite derivative sum satisfies $F_p'-F_p=-f_p$, so integration along the straight segment to $\beta_j$ gives

$$
e^{\beta_j}F_p(0)-F_p(\beta_j)
=e^{\beta_j}\int_0^{\beta_j}e^{-z}f_p(z)\,dz.
$$

Sum with weights $b_j$ and use $\sum b_je^{\beta_j}=-k$. The result is

$$
S_p=-\sum_jb_je^{\beta_j}\int_0^{\beta_j}e^{-z}f_p(z)\,dz.
$$

On these finitely many fixed compact segments, $|cz|$, $|R(cz)|$ and $|e^{-z}|$ are bounded independently of $p$. Hence $|S_p|\leq C_1C_2^p/(p-1)!\to0$. There are arbitrarily large [primes](../../../../../prime-number.md) not dividing the fixed [integer](../../../../../integer.md) $kcA$, contradicting $|S_p|\geq1$. Therefore **$\boxed{\pi\text{ is transcendental}}$**. This is the [Hermite auxiliary-polynomial proof for pi](../../../../../hermite-auxiliary-polynomial-proof-for-pi.md).

The more general [Lindemann–Weierstrass theorem](../../../../../lindemann-weierstrass-theorem.md) states that exponentials of distinct [algebraic numbers](../../../../../algebraic-number.md) are linearly independent over $\overline{\mathbb Q}$. Equivalently, exponentials of rationally independent [algebraic numbers](../../../../../algebraic-number.md) are algebraically independent over $\overline{\mathbb Q}$. In particular, the exponential of a nonzero [algebraic number](../../../../../algebraic-number.md) is transcendental.

Suppose $C=\cos\alpha\cos\beta$ were algebraic. The exponential formula for [cosine](../../../../../cosine.md) gives

$$
e^{i(\alpha+\beta)}+e^{i(\alpha-\beta)}+e^{i(-\alpha+\beta)}+e^{-i(\alpha+\beta)}-4C e^0=0.
$$

After combining equal exponents this is an algebraic-coefficient linear relation among exponentials of distinct [algebraic numbers](../../../../../algebraic-number.md). At least one exponent is nonzero, since $\alpha+\beta$ and $\alpha-\beta$ cannot both vanish when $\alpha,\beta\ne0$. Its coefficient is a positive [integer](../../../../../integer.md), even when two exponents coincide. The relation is therefore nontrivial and contradicts the theorem. Thus **$\boxed{\cos\alpha\cos\beta\text{ is transcendental}}$**, including the cases $\alpha=\pm\beta$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
