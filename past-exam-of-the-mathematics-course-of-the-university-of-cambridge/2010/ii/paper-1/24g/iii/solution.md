<h1 id="24g/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The ideal $(f)$ is prime, since an irreducible element of the polynomial ring is prime. By the [Hilbert Nullstellensatz](../../../../../../hilbert-nullstellensatz.md), it is the full vanishing ideal of $Z(f)$. Its [Zariski tangent space](../../../../../../zariski-tangent-space.md) at a point $a$ is therefore the kernel of the single linear form $df_a$, and has dimension $n-1$ or $n$.

At least one partial derivative $f_j$ is nonzero. In characteristic zero this is immediate for a nonconstant polynomial. In characteristic $p$, if all partial derivatives vanished, all exponents would be multiples of $p$. Since an algebraically closed field is perfect, $f$ would be a $p$th power of a nonconstant polynomial, contradicting irreducibility.

The nonzero $f_j$ cannot vanish everywhere on $Z(f)$: the Nullstellensatz would give $f_j^r\in(f)$, hence $f\mid f_j$, contradicting $\deg f_j<\deg f$. Thus some point has $df_a\ne0$, and the minimum tangent-space dimension is

$$
\boxed{\dim Z(f)=n-1.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [24G](../../24g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
