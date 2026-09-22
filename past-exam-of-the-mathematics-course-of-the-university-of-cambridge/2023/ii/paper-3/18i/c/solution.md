<h1 id="18i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [cyclotomic polynomial](../../../../../../cyclotomic-polynomial.md) is

$$
\Phi_n(X)=\prod_{\substack{1\leq a\leq n\\(a,n)=1}}
(X-\zeta_n^a),
$$

where $\zeta_n$ is primitive. Partitioning all $n$th roots by exact order gives the [cyclotomic factorization](../../../../../../cyclotomic-factorization.md)

$$
X^n-1=\prod_{d\mid n}\Phi_d(X).
$$

Induct on $n$. The quotient of the monic integer polynomial $X^n-1$ by the product of the already constructed monic $\Phi_d$, $d<n$, lies in $\mathbb Q[X]$ and is monic. [Gauss lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md) then shows that this quotient $\Phi_n$ lies in $\mathbb Z[X]$.

If the prime $p$ does not divide $n$, then over $\mathbb F_p$,

$$
\gcd(X^n-1,nX^{n-1})=1.
$$

**Thus $X^n-1$ has no repeated root. Every factor, including the reduction of $\Phi_n$, is square-free, proving the [Separability of a cyclotomic polynomial modulo p](../../../../../../separability-of-a-cyclotomic-polynomial-modulo-p.md).**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18I](../../18i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
