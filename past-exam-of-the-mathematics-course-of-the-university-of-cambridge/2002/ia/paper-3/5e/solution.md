<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

Using [Einstein summation convention](../../../../../einstein-notation.md) and the [contraction of two Levi-Civita symbols](../../../../../contraction-of-two-levi-civita-symbols.md),

$$
\begin{aligned}
[a\times(b\times c)]_i
&=\epsilon_{ijk}\epsilon_{k\ell m}a_jb_\ell c_m\\
&=(\delta_{i\ell}\delta_{jm}-\delta_{im}\delta_{j\ell})a_jb_\ell c_m\\
&=b_i(a\cdot c)-c_i(a\cdot b).
\end{aligned}
$$

This proves the [vector triple product identity](../../../../../vector-triple-product.md) directly from the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) and [Kronecker delta](../../../../../kronecker-delta.md).

Define the [scalar triple product](../../../../../scalar-triple-product.md) by $[a,b,c]=a\cdot(b\times c)$. Its expression $\epsilon_{ijk}a_ib_jc_k$ is unchanged by cyclically relabeling the three indices: a three-cycle has positive sign. Thus

$$
[a,b,c]=[b,c,a]=[c,a,b].
$$

In particular, let $\Delta=[e_1,e_2,e_3]$. Since the three vectors form a [basis](../../../../../basis.md), their [determinant](../../../../../determinant.md) $\Delta$ is nonzero, so their [reciprocal basis](../../../../../reciprocal-basis.md) vectors are well defined. Cyclic invariance and vanishing of a [scalar triple product](../../../../../scalar-triple-product.md) with repeated vectors give

$$
\widehat e_i\cdot e_j=\delta_{ij}.
$$

To calculate the new [scalar triple product](../../../../../scalar-triple-product.md) explicitly, apply the already proved [vector triple product identity](../../../../../vector-triple-product.md) with $A=e_3\times e_1$:

$$
\begin{aligned}
\widehat e_2\times\widehat e_3
&=\frac{(e_3\times e_1)\times(e_1\times e_2)}{\Delta^2}\\
&=\frac{[(e_3\times e_1)\cdot e_2]e_1-[(e_3\times e_1)\cdot e_1]e_2}{\Delta^2}
=\frac{e_1}{\Delta}.
\end{aligned}
$$

Consequently

$$
\boxed{[\widehat e_1,\widehat e_2,\widehat e_3]=\frac1\Delta\neq0,}
$$

so the reciprocal vectors also form a [basis](../../../../../basis.md). Taking the [reciprocal basis](../../../../../reciprocal-basis.md) of that [basis](../../../../../basis.md) now gives

$$
\widehat{\widehat e}_1
=\frac{\widehat e_2\times\widehat e_3}{[\widehat e_1,\widehat e_2,\widehat e_3]}
=\frac{e_1/\Delta}{1/\Delta}=e_1.
$$

The same cyclic calculation gives $\widehat{\widehat e}_2=e_2$ and $\widehat{\widehat e}_3=e_3$, proving [reciprocal basis involution](../../../../../reciprocal-basis-involution.md).

Finally, write $V=V_1e_1+V_2e_2+V_3e_3$. Taking a [dot product](../../../../../dot-product.md) with $\widehat e_j$ isolates $V_j$. Applying the same argument to the [reciprocal basis](../../../../../reciprocal-basis.md), whose reciprocal is the original [basis](../../../../../basis.md), gives the two sets of coordinates:

$$
\boxed{V_j=V\cdot\widehat e_j,\qquad \widehat V_j=V\cdot e_j.}
$$

No [orthonormality](../../../../../orthonormal-set.md) assumption is needed; the [reciprocal basis](../../../../../reciprocal-basis.md) is what makes these coordinate-extraction formulas work.

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
