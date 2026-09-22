<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $L/\mathbb Q_p$ be finite, with ring of integers $\mathcal O_L$ and maximal ideal $\mathfrak m_L$. The [formal group of an elliptic curve](../../../../../../formal-group-of-an-elliptic-curve.md) on an integral [Weierstrass model](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) is a [formal group law](../../../../../../formal-group-law.md) $F(X,Y)\in\mathcal O_L[[X,Y]]$, and $\widehat E(L)$ denotes its points with parameter in $\mathfrak m_L$. Its multiplication series is

$$
[m]_F(T)=mT+\sum_{j\ge2}a_jT^j,\qquad a_j\in\mathcal O_L.
$$

Since $p\nmid m$, the linear coefficient $m$ is a unit. Construct a compositional inverse $g(T)=m^{-1}T+\sum_{j\ge2}b_jT^j$ recursively: at degree $j$, the coefficient of $b_j$ in $[m]_F(g(T))$ is $m$, so the equation making that degree vanish uniquely determines $b_j\in\mathcal O_L$. The inverse on the other side is the same series, by uniqueness of formal composition inverses.

Both series converge on $\mathfrak m_L$, since their coefficients are integral and powers of an element of $\mathfrak m_L$ tend to zero. Their formal identities therefore hold as identities of convergent values. Thus for every $P$ there is a unique $Q$ with $[m]Q=P$, and

$$
\boxed{[m]:\widehat E(L)\xrightarrow{\sim}\widehat E(L).}
$$

This proves unique divisibility for every finite extension, including ramified extensions and negative $m$. It uses [prime-to-residue-characteristic multiplication on a formal group](../../../../../../prime-to-residue-characteristic-multiplication-on-a-formal-group.md), not an unjustified logarithm isomorphism on the entire maximal ideal.

Now assume [good reduction of an elliptic curve](../../../../../../good-reduction-of-an-elliptic-curve.md). For a finite local extension $M$, the reduction sequence is

$$
0\longrightarrow\widehat E(\mathfrak m_M)\longrightarrow E(M)\longrightarrow\widetilde E(k_M)\longrightarrow0.
$$

Properness defines reduction for all points, smoothness and the [Hensel lemma](../../../../../../hensel-s-lemma.md) make it surjective, and its kernel is precisely the formal group. Let $K$ be the maximal unramified extension and take $P\in E(K)$. Its coordinates lie in a finite unramified extension $L/\mathbb Q_p$. Over the algebraic closure of the residue field, the isogeny $[m]$ is surjective, so choose $\overline Q$ with $[m]\overline Q=\widetilde P$. This residue point is defined over a finite residue extension. Choose the corresponding finite unramified extension $M/L$ inside $K$, and lift it to $Q_0\in E(M)$ by smooth reduction.

Then $P-[m]Q_0$ lies in the reduction kernel. The first argument gives a unique kernel point $R$ with $[m]R=P-[m]Q_0$. Hence $Q=Q_0+R\in E(M)\subseteq E(K)$ satisfies $[m]Q=P$. Consequently

$$
\boxed{E(K)\text{ is divisible by }m.}
$$

Every lifting and convergence argument was made in a finite complete extension; $K$ itself need not be complete. Unique divisibility is asserted only for the formal group. For $|m|>1$, good reduction also lifts the prime-to-$p$ torsion, so $E(K)$ has nonzero $m$-torsion and division there is not unique. The construction is [unramified division points at good reduction](../../../../../../unramified-division-torsors-at-good-primes.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
