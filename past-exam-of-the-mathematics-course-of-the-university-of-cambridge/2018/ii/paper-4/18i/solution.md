<h1 id="18i/solution">Solution</h1>

↑ **Parent:** [18I](../18i.md)

Because $K$ has [characteristic](../../../../../characteristic-of-a-field.md) $p$, the [prime field](../../../../../prime-field.md) $\mathbb F_p$ lies in $K$, and

$$
f(\alpha+c)=(\alpha+c)^p-(\alpha+c)+a=f(\alpha)+c^p-c=0
$$

for every $c\in\mathbb F_p$. These are all $p$ roots. Moreover $f'(t)=-1$, so $f$ is a [separable polynomial](../../../../../separable-polynomial.md).

Let $m(t)$ be the [minimal polynomial of an algebraic element](../../../../../minimal-polynomial-of-an-algebraic-element.md) of $\alpha$ over $K$. Translation by $c\in\mathbb F_p$ sends an irreducible factor $g(t)$ of $f(t)$ to the irreducible factor $g(t-c)$. The [additive group](../../../../../additive-group.md) of $\mathbb F_p$ therefore acts on the irreducible factors, and every orbit has size $1$ or $p$. An orbit of size $p$ would already contribute $p\deg m$ to the degree-$p$ polynomial $f$, forcing $\deg m=1$. Then $\alpha\in K$, all roots $\alpha+c$ lie in $K$, and $L=K$, contrary to the hypothesis.

Thus $m(t-c)=m(t)$ for every $c\in\mathbb F_p$. If $1\leq d=\deg m<p$, comparison of the coefficient of $t^{d-1}$ in $m(t-c)-m(t)$ for $c\ne0$ gives $-dc$ times the nonzero leading coefficient, a contradiction. Hence $\deg m=p$, and since $m$ is a monic divisor of the monic degree-$p$ polynomial $f$, we have $m=f$. Thus **$f$ is irreducible over $K$**.

All roots $\alpha+c$ already belong to $K(\alpha)$, so the [splitting field](../../../../../splitting-field.md) is

$$
\boxed{L=K(\alpha)}.
$$

As the splitting field of a separable polynomial, $L/K$ is a [Galois extension](../../../../../finite-galois-extension.md). For each $c\in\mathbb F_p$, irreducibility gives a distinct $K$-automorphism

$$
\sigma_c(\alpha)=\alpha+c,
\qquad
\sigma_c\sigma_d=\sigma_{c+d}.
$$

These exhaust the $p=[L:K]$ automorphisms. This is an [Artin–Schreier extension](../../../../../artin-schreier-extension.md), and

$$
\boxed{\operatorname{Gal}(L/K)\cong(\mathbb F_p,+)\cong C_p}.
$$

## ↑ Ancestors (10)

1. [18I](../18i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
