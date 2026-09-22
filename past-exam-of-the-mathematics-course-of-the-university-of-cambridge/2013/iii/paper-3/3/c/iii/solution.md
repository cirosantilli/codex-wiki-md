<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Taking diagonal blocks is a homomorphism $P\to L$. Its kernel is $Q$, and block-diagonal inclusion is a section. For any $g\in P$, remove its diagonal element $\ell\in L$ by $g\ell^{-1}\in Q$. Also $Q\cap L=1$. Thus

$$
\boxed{P=Q\rtimes L.}
$$

Using $|\operatorname{GL}_k(q)|=q^{k(k-1)/2}\prod_{i=1}^k(q^i-1)$ and part (a), the product simplifies to

$$
\boxed{|P|=q^{m^2}\left(\prod_{i=1}^k(q^i-1)\right)
\left(\prod_{j=1}^{m-k}(q^{2j}-1)\right).}
$$

The exponent simplification is $2k(m-k)+k(k+1)/2+k(k-1)/2+(m-k)^2=m^2$.

For an independent [orbit-stabilizer theorem](../../../../../../../orbit-stabilizer-theorem.md) count, choose an ordered independent isotropic tuple $f_1,\ldots,f_k$. After $r$ choices, their span has $q^r$ elements and its [orthogonal complement](../../../../../../../orthogonal-complement.md) has dimension $2m-r$. The next choice therefore has $q^{2m-r}-q^r$ possibilities. The number of tuples is

$$
T_k=q^{k(k-1)/2}\prod_{j=m-k+1}^m(q^{2j}-1).
$$

Every totally isotropic $k$-space has $|\operatorname{GL}_k(q)|$ ordered bases, so the number of such spaces is

$$
N_k=\frac{\prod_{j=m-k+1}^m(q^{2j}-1)}{\prod_{i=1}^k(q^i-1)}.
$$

Each tuple extends to a [symplectic basis](../../../../../../../symplectic-basis.md) by successively choosing paired partners and taking orthogonal complements. Consequently the [symplectic group](../../../../../../../symplectic-group.md) is transitive on these spaces. The [stabilizer subgroup](../../../../../../../stabilizer-subgroup.md) of $W$ also preserves $W^\perp$, and so is exactly $P$. Dividing $|\operatorname{Sp}_{2m}(q)|$ by $N_k$ reproduces the boxed answer. Dividing by $T_k$ instead would count the pointwise [stabilizer subgroup](../../../../../../../stabilizer-subgroup.md) of the ordered tuple, a different subgroup.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
