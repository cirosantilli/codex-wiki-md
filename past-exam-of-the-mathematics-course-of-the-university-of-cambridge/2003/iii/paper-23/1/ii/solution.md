<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Kronecker–Weber theorem](../../../../../../kronecker-weber-theorem.md) says that **every finite abelian extension of $\mathbb Q$ is contained in a cyclotomic field**. We prove its quadratic case by identifying the [ramification](../../../../../../ramification-mathematics.md) that a [quadratic number field](../../../../../../quadratic-field.md) must have.

For an odd prime $\ell$, the cyclic [Galois group](../../../../../../galois-group.md) of $\mathbb Q(\zeta_\ell)/\mathbb Q$ has exactly one subgroup of index two. Its fixed field $F_\ell$ is quadratic and is [unramified](../../../../../../unramified-extension.md) at every finite prime other than $\ell$. For a squarefree integer $d$, the [discriminant](../../../../../../discriminant.md) of $\mathbb Q(\sqrt d)$ is $d$ if $d\equiv1\pmod4$, and $4d$ otherwise. A nontrivial quadratic [discriminant](../../../../../../discriminant.md) supported on the odd prime $\ell$ must therefore be

$$
\ell^*=(-1)^{(\ell-1)/2}\ell.
$$

Indeed $d=\pm1$ cannot give a nontrivial extension unramified at two, whereas exactly one of $\ell,-\ell$ is congruent to one modulo four. Thus

$$
F_\ell=\mathbb Q(\sqrt{\ell^*})\subseteq\mathbb Q(\zeta_\ell).
$$

This identifies the [quadratic subfield of a prime cyclotomic field](../../../../../../quadratic-subfield-of-a-prime-cyclotomic-field.md) using [ramification](../../../../../../ramification-mathematics.md), without a Gaussian-sum computation.

Now let $F=\mathbb Q(\sqrt d)$ with $d$ squarefree. Multiply $d$ by $\prod_{\ell\mid d,\ \ell\text{ odd}}\ell^*$. Every odd prime then occurs with even exponent, so its [square class](../../../../../../square-class.md) is represented by one of $1,-1,2,-2$. Thus adjoining the square roots of the $\ell^*$ removes all possible odd-prime [ramification](../../../../../../ramification-mathematics.md); the remaining quadratic factor is contained in

$$
\mathbb Q(\zeta_8)=\mathbb Q(i,\sqrt2),\qquad \sqrt2=\zeta_8+\zeta_8^{-1}.
$$

The original $\sqrt d$ is a rational multiple of a product of these square roots. It belongs to the [compositum](../../../../../../field-compositum.md) of $\mathbb Q(\zeta_8)$ and the prime [cyclotomic fields](../../../../../../cyclotomic-field.md) just used. This [compositum](../../../../../../field-compositum.md) is itself contained in a [cyclotomic field](../../../../../../cyclotomic-field.md), proving the theorem for $F$.

The sharper conductor statement follows from the same [ramification](../../../../../../ramification-mathematics.md) calculation. For the fundamental [discriminant](../../../../../../discriminant.md) $D$ of $F$, put

$$
D=D_2\prod_{\substack{\ell\mid D\\\ell\text{ odd}}}\ell^*,\qquad D_2\in\{1,-4,8,-8\}.
$$

The possibilities for $D_2$ follow immediately from the quadratic [discriminant](../../../../../../discriminant.md) formula. The corresponding fields are trivial, $\mathbb Q(i)$, $\mathbb Q(\sqrt2)$ and $\mathbb Q(\sqrt{-2})$, lying in the [cyclotomic fields](../../../../../../cyclotomic-field.md) of conductors $1,4,8,8$. Their conductors are coprime to the odd primes in the product. Hence [quadratic Kronecker–Weber theorem by ramification](../../../../../../quadratic-kronecker-weber-theorem-by-ramification.md) gives the explicit conclusion

$$
\boxed{\mathbb Q(\sqrt D)\subseteq\mathbb Q(\zeta_{|D|}).}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
