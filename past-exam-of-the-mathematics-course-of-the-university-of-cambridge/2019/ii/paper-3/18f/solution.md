<h1 id="18f/solution">Solution</h1>

↑ **Parent:** [18F](../18f.md)

Let $L$ be a [splitting field](../../../../../splitting-field.md) of $f(X)=X^m-1$ over $k$. Its [formal derivative](../../../../../formal-derivative.md) is

$$
f'(X)=mX^{m-1}.
$$

The assumption on the [characteristic](../../../../../characteristic-of-a-field.md) of $k$ says that $m\ne0$ in $k$. Any root $\alpha$ of $f$ is nonzero, and hence $f'(\alpha)=m\alpha^{m-1}\ne0$. Thus $f$ and $f'$ have no common root, so $f$ is a [separable polynomial](../../../../../separable-polynomial.md). Since it has degree $m$ and splits over $L$, it has exactly $m$ distinct roots. This is the [separability of roots of unity](../../../../../separability-of-roots-of-unity.md).

Fix a [primitive root of unity](../../../../../primitive-root-of-unity.md) $\zeta_m=e^{2\pi i/m}$. Define the $m$th [cyclotomic polynomial](../../../../../cyclotomic-polynomial.md) by

$$
\boxed{\Phi_m(X)=
\prod_{\substack{1\leq a\leq m\\(a,m)=1}}
(X-\zeta_m^a).}
$$

It is [monic](../../../../../monic-polynomial.md) and has degree given by the [Euler totient function](../../../../../euler-totient-function.md) $\varphi(m)$. Partitioning all $m$th [roots of unity](../../../../../root-of-unity.md) according to their exact [multiplicative order](../../../../../multiplicative-order.md) gives the [cyclotomic factorization](../../../../../cyclotomic-factorization.md)

$$
X^m-1=\prod_{d\mid m}\Phi_d(X).
$$

We now prove by [mathematical induction](../../../../../mathematical-induction.md) that $\Phi_m\in\mathbb Z[X]$. The base case is $\Phi_1=X-1$. If the result holds for every proper divisor $d$ of $m$, then

$$
G(X)=\prod_{\substack{d\mid m\\d<m}}\Phi_d(X)
$$

is monic and belongs to $\mathbb Z[X]$. Polynomial division of $X^m-1$ by the monic integer polynomial $G$ produces a quotient and remainder in $\mathbb Z[X]$. The factorization over $\mathbb C$ says that the remainder is zero and the quotient is $\Phi_m$, proving the claim.

It remains to prove [irreducibility of cyclotomic polynomials](../../../../../irreducibility-of-cyclotomic-polynomials.md). Let $f\in\mathbb Z[X]$ be a monic [irreducible polynomial](../../../../../irreducible-polynomial.md) dividing $\Phi_m$, let $\varepsilon$ be a root of $f$, and write $\Phi_m=fg$. We claim that $\varepsilon^p$ is a root of $f$ for every [prime number](../../../../../prime-number.md) $p\nmid m$. Otherwise $\varepsilon^p$ is a root of $g$, so $\varepsilon$ is a root of $g(X^p)$. Since $f$ is the [minimal polynomial](../../../../../minimal-polynomial.md) of $\varepsilon$ over $\mathbb Q$, [Gauss lemma for polynomials](../../../../../gauss-lemma-for-polynomials.md) gives

$$
f(X)\mid g(X^p)\qquad\text{in }\mathbb Z[X].
$$

After [reduction of an integer polynomial modulo a prime](../../../../../reduction-of-an-integer-polynomial-modulo-a-prime.md), the [Frobenius endomorphism](../../../../../frobenius-endomorphism.md) gives

$$
\bar f(X)\mid \bar g(X^p)=\bar g(X)^p.
$$

Choose an irreducible factor $h$ of the nonconstant monic polynomial $\bar f$. Then $h\mid\bar g$, so $h^2\mid\bar f\bar g=\bar\Phi_m$. The [cyclotomic factorization](../../../../../cyclotomic-factorization.md) would then make $h^2$ divide $X^m-1$ over $\mathbb F_p$. This is impossible because its derivative $mX^{m-1}$ is coprime to it when $p\nmid m$.

Thus $f(\varepsilon^p)=0$ for every prime $p\nmid m$. Iterating this fact over a prime factorization shows that $f(\varepsilon^a)=0$ whenever $(a,m)=1$. These are all $\varphi(m)$ primitive $m$th roots, so

$$
\deg f\geq\varphi(m)=\deg\Phi_m.
$$

Because $f$ divides $\Phi_m$, equality holds and $f=\Phi_m$. Hence every cyclotomic polynomial is irreducible over $\mathbb Q$.

Finally, direct multiplication gives

$$
(X^2-X+1)F=X^{10}-X^5+1.
$$

Also

$$
X^{15}+1=(X^5+1)(X^{10}-X^5+1).
$$

Applying the [cyclotomic factorization](../../../../../cyclotomic-factorization.md) to the two factors on the right gives

$$
X^{15}+1=\Phi_2\Phi_6\Phi_{10}\Phi_{30},
\qquad
X^5+1=\Phi_2\Phi_{10},
$$

and therefore

$$
X^{10}-X^5+1=\Phi_6(X)\Phi_{30}(X).
$$

Since $X^2-X+1=\Phi_6(X)$, cancellation yields

$$
\boxed{F(X)=\Phi_{30}(X).}
$$

The [thirtieth cyclotomic polynomial](../../../../../thirtieth-cyclotomic-polynomial.md) is irreducible over $\mathbb Q$ by the theorem just proved, so $F$ is irreducible.

## ↑ Ancestors (10)

1. [18F](../18f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
