<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $L$ be any degree-zero [line bundle](../../../../../../line-bundle.md) on the genus-one [smooth projective curve](../../../../../../smooth-projective-curve.md). The twist $M=L\otimes\mathcal O(p_0)$ has degree one. The [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) gives

$$
h^0(M)-h^0(K_X\otimes M^{-1})=1.
$$

The second [line bundle](../../../../../../line-bundle.md) has degree $2g-2-1=-1$, so it has no nonzero section: the zero divisor of such a section would be effective of negative degree. Hence $h^0(M)=1$. A nonzero section has an effective zero [divisor](../../../../../../divisor.md) of degree one, which is a single point $p$. It is a $k$-rational point even over a general field, since a degree-one effective divisor has residue degree one. Thus $M\cong\mathcal O(p)$ and $L\cong\mathcal O(p-p_0)=\alpha(p)$.

This proves surjectivity; part (a) gives injectivity. Hence **$\alpha$ is a bijection**, as in the [Abel-Jacobi map of a genus-one curve](../../../../../../abel-jacobi-map-of-a-genus-one-curve.md). Define

$$
\boxed{p\oplus q=\alpha^{-1}\bigl(\alpha(p)\otimes\alpha(q)\bigr),\qquad \ominus p=\alpha^{-1}\bigl(\alpha(p)^{-1}\bigr).}
$$

Tensor product of [line bundles](../../../../../../line-bundle.md) is associative and commutative, so this is an [abelian group](../../../../../../abelian-group.md) law on $X(k)$. Its identity is $p_0$, since $\alpha(p_0)=\mathcal O_X$. Equivalently, $p\oplus q$ is the unique point $r$ with $\mathcal O(r-p_0)\cong\mathcal O(p+q-2p_0)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
