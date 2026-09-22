<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $u=\sum_\lambda a_\lambda e(\lambda)$ with finite support. The [root reflection](../../../../../../root-reflection.md) is an involution, and $s_\alpha u=-u$ implies $a_{s_\alpha\lambda}=-a_\lambda$. Any fixed [weight](../../../../../../weight-representation-theory.md) has coefficient zero. For each nonfixed orbit choose its representative $\lambda$ with

$$
m=\lambda(H_\alpha)>0,\qquad
s_\alpha\lambda=\lambda-m\alpha.
$$

Integrality of $m$ follows because $\lambda$ belongs to the [weight lattice](../../../../../../weight-lattice.md); positivity is ensured by our choice of orbit representative. Pairing the orbit coefficients gives

$$
u=\sum_{\text{chosen }\lambda}a_\lambda[e(\lambda)-e(\lambda-m\alpha)].
$$

For each pair, elementary finite telescoping shows

$$
e(\lambda)-e(\lambda-m\alpha)
=(1-e(\alpha))\left[-\sum_{r=1}^me(\lambda-r\alpha)\right].
$$

There are finitely many chosen orbits, and each inner sum is finite. This proves the [root-binomial divisibility of reflection anti-invariants](../../../../../../root-binomial-divisibility-of-reflection-anti-invariants.md):

$$
\boxed{\frac{u}{1-e(\alpha)}
=-\sum_{\text{chosen }\lambda}a_\lambda\sum_{r=1}^{\lambda(H_\alpha)}
e(\lambda-r\alpha)\in\mathbb Z[\Lambda_W].}
$$

For precision, the geometric-series expression is interpreted coefficientwise. Its coefficient at a [weight](../../../../../../weight-representation-theory.md) $\nu$ is $\sum_{n\geq0}a_{\nu-n\alpha}$, which is a finite sum because $u$ has finite support. On each coset of $\mathbb Z\alpha$, reflection pairs the coefficients with opposite signs, so their total is zero. These cumulative sums vanish both before the smallest occupied [weight](../../../../../../weight-representation-theory.md) and after the largest occupied [weight](../../../../../../weight-representation-theory.md). Only finitely many cosets are occupied, hence the product of the formal series with $u$ has finite support and equals the boxed quotient.

The individual terms $e(n\alpha)u$ need not vanish for large $n$. For example, $u=e(\alpha)-e(-\alpha)$ is anti-invariant, and its quotient is $-1-e(-\alpha)$. Thus **“finite sum” means a finite result after coefficientwise cancellation**, not an actually truncated geometric series. No analytic convergence assumption is involved.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
