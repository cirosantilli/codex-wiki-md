# Minimal polynomial of a companion block chain

↑ **Parent:** [Minimal polynomial](minimal-polynomial.md)

Let $A$ be a [companion matrix](companion-matrix.md) of a monic [irreducible polynomial](irreducible-polynomial.md) $f\in F[x]$ of degree $n$. Form the $N$-by-$N$ [block matrix](block-matrix.md) $B$ with $A$ on its diagonal, $I_n$ immediately above the diagonal, and zero elsewhere. If the [field characteristic](characteristic-of-a-field.md) is $p>0$, write $f(x)=h(x^q)$ with $q=p^r$ maximal, so that $h'\ne0$; in characteristic zero take $q=1$ and $h=f$. Then

$$
\boxed{m_B(x)=f(x)^{\lceil N/q\rceil},\qquad
\det(xI-B)=f(x)^N.}
$$

Thus a [separable polynomial](separable-polynomial.md) gives $m_B=f^N$, but an irreducible [polynomial](polynomial-split.md) with zero [formal derivative](formal-derivative.md) can give a smaller exponent. For example, over the [rational function field](rational-function-field.md) $\mathbb F_2(t)$, the irreducible [polynomial](polynomial-split.md) $f(x)=x^2-t$ has $q=2$, so a two-block chain still has [minimal polynomial](minimal-polynomial.md) $f$.

To prove the formula, write $B=D+K$, where $D$ has diagonal blocks $A$ and $K$ is the block shift. These are [commuting operators](commuting-operators.md), and $K^j$ vanishes exactly when $j\geq N$. The [binomial theorem](binomial-theorem.md) in positive [field characteristic](characteristic-of-a-field.md) gives $B^q=D^q+K^q$. Expanding $h(D^q+K^q)$ gives $f(B)=K^qH$, with $H$ commuting with $K$. The diagonal blocks of $H$ are $h'(A^q)$, which are invertible by [Bézout's identity for polynomials](bezout-s-identity-for-polynomials.md), since $h$ is irreducible with nonzero [formal derivative](formal-derivative.md) and $h(A^q)=0$. Therefore $f(B)^s=K^{qs}H^s$ vanishes exactly when $qs\geq N$. Finally, the [block upper triangular matrix](block-upper-triangular-matrix.md) determinant gives the displayed [characteristic polynomial](characteristic-polynomial.md), while the [Cayley-Hamilton theorem](cayley-hamilton-theorem-split.md) and irreducibility force the [minimal polynomial](minimal-polynomial.md) to be a power of $f$.

## ↑ Ancestors (7)

1. [Minimal polynomial](minimal-polynomial.md)
2. [Operator theory](linear-operator-theory-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2017/1/b/iii/solution.md)
