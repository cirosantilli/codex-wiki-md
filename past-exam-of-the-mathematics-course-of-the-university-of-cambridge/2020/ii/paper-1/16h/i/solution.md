<h1 id="16h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose sets $K,L,M$ of cardinalities $\kappa,\lambda,\mu$. Their [cardinal arithmetic](../../../../../../cardinal-arithmetic.md) operations are

$$
\kappa+\lambda=|K\sqcup L|,
\qquad
\kappa\lambda=|K\times L|,
\qquad
\kappa^\lambda=|K^L|,
$$

where $K^L$ is the set of functions $L\to K$. The relation $\kappa\le\lambda$ means that there is an [injective function](../../../../../../injective-function.md) $K\to L$.

The [currying law for cardinal exponentiation](../../../../../../currying-law-for-cardinal-exponentiation.md) follows from the explicit [bijection](../../../../../../bijection.md)

$$
(K^L)^M\longleftrightarrow K^{L\times M},
\qquad
f\longmapsto\bigl((l,m)\mapsto f(m)(l)\bigr),
$$

and proves

$$
\boxed{(\kappa^\lambda)^\mu=\kappa^{\lambda\mu}}.
$$

Moreover, $2^\kappa$ is the cardinality of the [power set](../../../../../../power-set.md) of a set of size $\kappa$, so [Cantor theorem](../../../../../../cantor-s-theorem.md) gives

$$
\boxed{2^\kappa>\kappa}.
$$

For completeness, identify each cardinal with its [initial ordinal](../../../../../../initial-ordinal.md). Suppose that some infinite $\kappa$ violates $\kappa^2=\kappa$, and choose the least such cardinal. Well-order the pairs $(\alpha,\beta)\in\kappa^2$ first by $\max\{\alpha,\beta\}$ and then lexicographically. Every proper initial segment is contained in $\gamma^2$ together with finitely many boundary pieces for some $\gamma<\kappa$, and has cardinality below $\kappa$ by minimality. The resulting well-order therefore has cardinality at most $\kappa$. The reverse inequality is immediate from $\alpha\mapsto(\alpha,0)$, contradicting the choice of $\kappa$. Thus the [square of an infinite cardinal](../../../../../../square-of-an-infinite-cardinal.md) satisfies $\kappa^2=\kappa$.

If $\nu=\max\{\kappa,\lambda\}$, monotonicity now gives

$$
\nu\le\kappa+\lambda\le\nu+\nu=\nu,
\qquad
\nu\le\kappa\lambda\le\nu^2=\nu.
$$

Hence the [sum and product of two infinite cardinals](../../../../../../sum-and-product-of-two-infinite-cardinals.md) obey

$$
\boxed{\kappa+\lambda=\kappa\lambda=\max\{\kappa,\lambda\}}.
$$

Assertion (i) can be false. For any infinite $\lambda$, take $\kappa=(2^\lambda)^+$. Then $\kappa^\lambda\ge\kappa>2^\lambda$, so

$$
\boxed{\kappa^\lambda=2^\lambda\text{ is not always true}}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [16H](../../16h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
