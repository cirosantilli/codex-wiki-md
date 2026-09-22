<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $M_n=\max_{1\leq j\leq n}W_j$ for [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) with [distribution function](../../../../../cumulative-distribution-function.md) $F$. Then $P(M_n\leq u)=F(u)^n$. Membership in the [maximum domain of attraction](../../../../../maximum-domain-of-attraction.md) of a nondegenerate [distribution function](../../../../../cumulative-distribution-function.md) $G$ means that some deterministic $a_n>0$ and $b_n\in\mathbb R$ satisfy

$$
\boxed{\frac{M_n-b_n}{a_n}\xrightarrow{d}Z,\qquad P(Z\leq x)=G(x),}
$$

or equivalently $F(a_nx+b_n)^n\to G(x)$ at every continuity point of $G$.

Under the stated convergence, put $Z_n=(M_n-b_n)/a_n$, $r_n=\alpha_n/a_n\to a>0$, and $s_n=(\beta_n-b_n)/a_n\to b$. The [Slutsky theorem](../../../../../slutsky-theorem.md) says that combining a sequence with [convergence in distribution](../../../../../convergence-in-distribution.md) with sequences converging in [probability](../../../../../probability.md) to constants preserves the corresponding sum, product and ratio limits, provided a limiting denominator is nonzero. Applying it here gives

$$
\frac{M_n-\beta_n}{\alpha_n}=\frac{Z_n-s_n}{r_n}\xrightarrow{d}\frac{Z-b}{a}.
$$

The limiting [distribution function](../../../../../cumulative-distribution-function.md) is $P((Z-b)/a\leq x)=G(ax+b)$, continuous for every real $x$ because $G$ is continuous and $a>0$. Consequently,

$$
\boxed{F(\alpha_nx+\beta_n)^n\longrightarrow G(ax+b)\quad\text{for every real }x.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
