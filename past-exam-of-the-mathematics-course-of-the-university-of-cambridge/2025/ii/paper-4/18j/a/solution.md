<h1 id="18j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix a primitive $n$th root of unity $\zeta_n$. The $n$th [cyclotomic polynomial](../../../../../../cyclotomic-polynomial.md) is

$$
\Phi_n(X)=
\prod_{\substack{1\leq a\leq n\\(a,n)=1}}
(X-\zeta_n^a).
$$

Its roots are exactly the roots of unity of order $n$.

Partitioning all $n$th roots of unity by exact order gives the [cyclotomic factorization](../../../../../../cyclotomic-factorization.md)

$$
X^n-1=\prod_{d\mid n}\Phi_d(X).
$$

We prove $\Phi_n\in\mathbb Z[X]$ by induction on $n$. The assertion is clear for $n=1$. If it holds for every proper divisor of $n$, then

$$
\Phi_n(X)=\frac{X^n-1}{\prod_{d\mid n,\ d<n}\Phi_d(X)}.
$$

The denominator is monic and belongs to $\mathbb Z[X]$. Exact polynomial division shows that the quotient lies in $\mathbb Q[X]$, and Gauss's lemma makes this monic quotient an element of $\mathbb Z[X]$.

Now let $K\subseteq\mathbb C$. The minimal polynomial of $\zeta_n$ over $K$ divides $\Phi_n$, so every $K$-conjugate of $\zeta_n$ is another primitive root $\zeta_n^a$ and lies in $K(\zeta_n)$. The extension is therefore normal. It is separable because the characteristic is zero, and hence it is Galois.

Every $\sigma\in\operatorname{Gal}(K(\zeta_n)/K)$ has

$$
\sigma(\zeta_n)=\zeta_n^a
$$

for some $a\in(\mathbb Z/n\mathbb Z)^\times$. Since $\zeta_n$ generates the extension, this gives an injective homomorphism

$$
\operatorname{Gal}(K(\zeta_n)/K)
\hookrightarrow(\mathbb Z/n\mathbb Z)^\times.
$$

The group on the right is abelian, so the Galois group is abelian, as summarized by the [cyclotomic field](../../../../../../cyclotomic-field.md) construction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18J](../../18j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
