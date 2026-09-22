<h1 id="10e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a coprime presentation

$$
f(X,Y)=\frac{p(X,Y)}{q(X,Y)},
\qquad p,q\in\mathbb C[X,Y].
$$

For a [polynomial](../../../../../../polynomial-split.md) $r$, write $r^*(X,Y)=r(Y,X)$. Symmetry of $f$ gives

$$
p q^*=p^*q.
$$

Since $\mathbb C[X,Y]$ is a [unique factorization domain](../../../../../../unique-factorization-domain.md) and $\gcd(p,q)=1$, one has $p\mid p^*$ and $q\mid q^*$. Exchanging the variables preserves total degree, so

$$
p^*=\lambda p,\qquad q^*=\mu q
$$

for nonzero constants $\lambda,\mu$. The displayed identity gives $\lambda=\mu$, and applying the exchange twice gives $\lambda^2=1$.

If $\lambda=-1$, then $p(X,X)=q(X,X)=0$, so $X-Y$ divides both [polynomials](../../../../../../polynomial-split.md), contradicting coprimality. Therefore $\lambda=1$, and both $p$ and $q$ are symmetric. Taking $g=p$ and $h=q$ proves the claim, which is the [symmetric rational function in two variables](../../../../../../symmetric-rational-function-in-two-variables.md) result.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10E](../../10e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
