<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The multiplicative [Hilbert theorem 90](../../../../../../hilbert-s-theorem-90.md) states that, for a finite [Galois extension](../../../../../../finite-galois-extension.md) $L/K$ with [Galois group](../../../../../../galois-group.md) $G$, every multiplicative [cocycle](../../../../../../cocycle.md) $c:G\to L^\times$ satisfying $c_{\sigma\tau}=c_\sigma\sigma(c_\tau)$ has the form $c_\sigma=\sigma(y)/y$ for some $y\in L^\times$. In the cyclic case $G=\langle\sigma\rangle$, it says

$$
\boxed{N_{L/K}(x)=1\iff x=\sigma(y)/y\text{ for some }y\in L^\times.}
$$

Here is the full existence argument. Distinct [field homomorphisms](../../../../../../field-homomorphism.md) $\sigma:L\to L$ are linearly independent as functions over $L$. To see this [Artin independence theorem](../../../../../../linear-independence-of-distinct-field-embeddings.md) directly, assume a nonzero identically vanishing relation with the fewest nonzero coefficients. There are at least two terms. Choose two participating embeddings $\sigma_1,\sigma_j$ and an element $a$ with $\sigma_1(a)\ne\sigma_j(a)$. Evaluate the relation at $at$ and subtract $\sigma_j(a)$ times its value at $t$. The $j$th term disappears while the first remains nonzero, giving a shorter vanishing relation, a contradiction.

Apply this independence to

$$
A(t)=\sum_{\sigma\in G}c_\sigma^{-1}\sigma(t).
$$

The coefficients are nonzero, so $A$ is not identically zero; choose $t$ with $y=A(t)\ne0$. The [cocycle](../../../../../../cocycle.md) identity gives $\tau(c_\sigma^{-1})=c_{\tau\sigma}^{-1}c_\tau$, and hence

$$
\tau(y)=\sum_{\sigma\in G}\tau(c_\sigma^{-1})\tau\sigma(t)
=c_\tau\sum_{\rho\in G}c_\rho^{-1}\rho(t)=c_\tau y.
$$

This proves the general statement. In the cyclic case, given $N(x)=1$, set $c_1=1$ and $c_{\sigma^j}=x\sigma(x)\cdots\sigma^{j-1}(x)$ for $1\leq j<n$. The norm-one identity makes this definition compatible with $\sigma^n=1$, and the [cocycle](../../../../../../cocycle.md) identity follows by concatenating the products. The argument above gives $\sigma(y)/y=x$. Conversely that quotient has norm one because its conjugate product telescopes.

Finally let $L/K$ be [unramified](../../../../../../unramified-extension.md), and take its [arithmetic Frobenius](../../../../../../frobenius-automorphism.md) $\phi$. For a unit $x$ of norm one, the cyclic theorem gives $b\in L^\times$ with $\phi(b)/b=x$. Write $r=v_L(b)$ and choose the common [uniformizer](../../../../../../uniformizer.md) $\pi\in K$. Then $y=\pi^{-r}b$ has valuation zero, and $\phi(\pi)=\pi$ implies $\phi(y)/y=\phi(b)/b=x$. Thus the [unit form of Hilbert theorem 90](../../../../../../unit-form-of-hilbert-theorem-90.md) is

$$
\boxed{x\in\mathcal O_L^\times,\ N_{L/K}(x)=1\Longrightarrow\exists y\in\mathcal O_L^\times:\ \phi(y)/y=x.}
$$

The unramified hypothesis is what permits shifting an arbitrary integer valuation of $b$ by a power of a uniformizer belonging to $K$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
