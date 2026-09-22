<h1 id="8d/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take $G=S_3$ and its [normal subgroup](../../../../../../../normal-subgroup.md) $N=A_3=\langle r\rangle$, where $r=(1\ 2\ 3)$. Normality follows either from the [sign of a permutation](../../../../../../../sign-of-a-permutation.md) or directly from conjugation sending $r$ to $r$ or $r^{-1}$. The [quotient group](../../../../../../../quotient-group.md) has order two, and $t=(1\ 2)$ provides a section $i:C_2\to S_3$ because $t^2=1$ and $tN$ is its nonidentity coset.

However, the map $\Phi(q,n)=i(q)n$ from the [direct product of groups](../../../../../../../direct-product-of-groups.md) is not a [group homomorphism](../../../../../../../group-homomorphism.md). In its domain $(1,r)$ commutes with $(tN,1)$, whereas their images $r$ and $t$ do not commute: $trt^{-1}=r^{-1}\ne r$. This is a [split group extension](../../../../../../../split-group-extension.md) giving a genuine [semidirect product](../../../../../../../semidirect-product.md) instead of a direct product. **The pair $S_3,A_3$ supplies the required split but non-direct example.**

For the general bijectivity assertion, let $\pi:G\to G/N$ be the quotient projection and assume $\pi\circ i$ is the identity. Given $g\in G$, put $q=\pi(g)$ and $n=i(q)^{-1}g$. Then $\pi(n)=q^{-1}q=1$, so $n\in N$ and $g=i(q)n$. This proves surjectivity of $\Phi$. If $i(q)n=i(q')n'$, applying $\pi$ gives $q=q'$, after which cancellation gives $n=n'$. Thus

$$
\boxed{\Phi:(G/N)\times N\longrightarrow G\text{ is always a bijection.}}
$$

This [section normal form for a split group extension](../../../../../../../section-normal-form-for-a-split-group-extension.md) does not require finiteness. The obstruction to its being a homomorphism is the nontrivial conjugation action of the section on $N$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [8D](../../../8d.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ia](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
