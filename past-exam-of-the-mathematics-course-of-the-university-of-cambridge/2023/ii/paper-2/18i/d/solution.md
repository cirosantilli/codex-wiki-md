<h1 id="18i/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume now that $g$ is irreducible and separable. Its splitting field $L/K$ is [Galois](../../../../../../finite-galois-extension.md), and its Galois group acts transitively on the roots $y_i$ by the [Galois group of a polynomial](../../../../../../galois-group-of-a-polynomial.md). Part (c) extends every such automorphism uniquely to $M$. If $x_i^p=y_i$, the extension sends $x_i$ to the unique $p$th root above the image of $y_i$. The [transitivity lifted through unique pth roots](../../../../../../transitivity-lifted-through-unique-pth-roots.md) therefore shows that

$$
\operatorname{Aut}(M/K)
$$

acts transitively on the roots of $f$.

Every automorphism of $M/K$ preserves $L$, because $L$ is the splitting field of $g$ over $K$. Transitivity therefore implies that either all roots $x_i$ lie in $L$ or none does. Since $x_i^p\in L$, the [minimal polynomial of a purely inseparable element](../../../../../../minimal-polynomial-of-a-purely-inseparable-element.md) has degree either one or $p$. Consequently,

$$
\boxed{\text{either every root lies in }L,\text{ or every root has degree }p\text{ over }L.}
$$

Let $h\in K[T]$ be a monic irreducible factor of $f$. If $h$ is inseparable, part (a) gives

$$
h(T)=q(T^p)
$$

for a nonconstant monic $q\in K[T]$. Since $q(T^p)$ divides $g(T^p)$, polynomial division in $K[U]$ and substitution $U=T^p$ show that $q$ divides $g$. Irreducibility of $g$ forces $q=g$, hence $h=f$. Therefore

$$
\boxed{h=f\quad\text{or}\quad h\text{ is separable},}
$$

which is the [irreducible factors after Frobenius substitution](../../../../../../irreducible-factors-after-frobenius-substitution.md) dichotomy.

If every coefficient of $g$ is a $p$th power, say

$$
g(T)=\sum_i a_i^pT^i,
$$

then

$$
f(T)=g(T^p)
=\left(\sum_i a_iT^i\right)^p,
$$

so $f$ is reducible.

Conversely, suppose $f$ is reducible and factor it into distinct monic irreducibles:

$$
f=\prod_i h_i^{e_i}.
$$

Every $h_i$ is then a proper factor, hence separable by the preceding dichotomy. Since $f'=0$, unique factorization and $h_i'\ne0$ force $p\mid e_i$ for every $i$. Thus $f=q^p$ for some monic $q\in K[T]$. The [Frobenius endomorphism](../../../../../../frobenius-endomorphism.md) raises coefficients to their $p$th powers, and the coefficient of $T^{ip}$ in $f=g(T^p)$ is the coefficient of $T^i$ in $g$. Hence every coefficient of $g$ is a $p$th power in $K$. We have proved the [reducibility criterion after Frobenius substitution](../../../../../../reducibility-criterion-after-frobenius-substitution.md):

$$
\boxed{g(T^p)\text{ is reducible over }K
\iff\text{ every coefficient of }g\text{ is a }p\text{th power in }K.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [18I](../../18i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
