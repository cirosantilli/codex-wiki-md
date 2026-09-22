<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The auxiliary [Higman group](../../../../../../higman-group.md) $Q$ has no nontrivial [finite quotients of a group](../../../../../../finite-quotient-of-a-group.md). One can use this permitted property directly, but there is a short verification. In any finite quotient, let $n_i$ be the order of the image of $a_i$. Since conjugation sends $a_{i+1}$ to its square, $n_{i+1}$ must be odd. If some $n_i>1$, choose the least [prime number](../../../../../../prime-number.md) $p$ dividing any $n_i$. It is odd. Conjugation by the preceding generator gives

$$
2^{n_{i-1}}\equiv1\pmod p.
$$

The [multiplicative order](../../../../../../multiplicative-order.md) of $2$ modulo $p$ is therefore a divisor of $n_{i-1}$. It is greater than one and divides $p-1$ by the [Fermat little theorem](../../../../../../fermat-little-theorem.md), so it has a prime divisor smaller than $p$. That prime also divides $n_{i-1}$, contradicting the choice of $p$. Hence every $n_i=1$ and the quotient is trivial.

Given any finitely presented group $P$, form $\widehat P=P*\langle v\rangle$, and apply part (a) to the word $w=v$. This word is nontrivial by the [normal form theorem for a free product](../../../../../../normal-form-theorem-for-a-free-product.md), so the output $J=\widehat P(v)$ contains $P$ by the embedding already proved.

To check its finite quotients, let $f:J\to F$ be any [group homomorphism](../../../../../../group-homomorphism.md) to a [finite group](../../../../../../finite-group.md). The image of the copy of $Q$ is trivial by the preceding property. The identifications $u_j=a_3^{j+1}a_1a_3^{-(j+1)}$ make all $f(u_j)$ trivial. Thus the equations $u_j^{-1}cu_j=g_j$ give, in the image,

$$
f(c)=f(z)=f(d)=f(x_i z)\quad\text{for every input generator }x_i.
$$

Since $f(c)=f(z)$, this forces $f(x_i)=1$ for all generators of $\widehat P$, including $v$. The defining word $c=[v,z]$ then has trivial image, so $f(z)=f(d)=1$ as well. Every generator of $J$ has trivial image. Therefore

$$
\boxed{P\hookrightarrow J,\qquad J\text{ is finitely presented and has no nontrivial finite quotients}.}
$$

This uses the concrete construction of part (a), not an assumption that arbitrary quotients preserve an embedding of $P$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 104](../../../paper-104-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
