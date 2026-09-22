<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the corrected [Lie algebra representation](../../../../../lie-algebra-representation.md) $E=-e$, $H=h$, $F=f$ from part (i). A [vector subspace](../../../../../vector-subspace.md) is invariant under $E,H,F$ exactly when it is invariant under the printed $e,h,f$, since changing the sign of a [linear map](../../../../../linear-map.md) does not change its [invariant subspaces](../../../../../invariant-subspace.md). Define

$$
W=\bigoplus_{i\geq1}kv_i.
$$

This is a nonzero proper [submodule](../../../../../submodule.md): $H$ preserves each $kv_i$, $F$ increases the index, $E(v_1)=0$, and $E(v_i)=-(i-1)v_{i-1}\in W$ for $i\geq2$.

We must rule out [submodules](../../../../../submodule.md) consisting only of mixtures of [weight vectors](../../../../../weight-vector.md). Let $U\ne0$ be any [submodule](../../../../../submodule.md), and choose $u=\sum_{j\in S}a_jv_j\in U$ with $S$ finite and every $a_j\ne0$. The [eigenvalues](../../../../../eigenvalue.md) $-2j$ of $H$ are distinct. For $i\in S$, the [Lagrange interpolation polynomial](../../../../../lagrange-polynomial.md)

$$
p_i(t)=\prod_{\substack{j\in S\\j\ne i}}\frac{t+2j}{-2i+2j}
$$

satisfies $p_i(H)u=a_iv_i$. Since $U$ is invariant under $H$, it is invariant under every [polynomial](../../../../../polynomial-split.md) in $H$, so $v_i\in U$.

If $i=0$, repeated applications of $F$ give $F^mv_0=m!v_m$, and $U=V$. If $i\geq1$, repeated applications of $E$ give a nonzero multiple of $v_1$, because the successive coefficients $-(i-1),\ldots,-1$ are nonzero in [characteristic zero](../../../../../characteristic-zero.md). Repeated applications of $F$ to $v_1$ then give every $v_j$ with $j\geq1$, so $W\subseteq U$.

Finally, if such a $U$ contains any vector outside $W$, that vector has a nonzero coefficient of $v_0$; the same [polynomial interpolation](../../../../../polynomial-interpolation.md) extracts $v_0$, forcing $U=V$. Hence the complete list of [submodules](../../../../../submodule.md) is $0,W,V$. In particular, $W$ is a [simple module](../../../../../irreducible-module.md). The [quotient module](../../../../../quotient-module.md) $V/W$ has [basis](../../../../../basis.md) $\overline v_0$; $E\overline v_0=H\overline v_0=0$ and $F\overline v_0=\overline v_1=0$. It is the one-dimensional [trivial Lie algebra representation](../../../../../trivial-lie-algebra-representation.md).

The [module extension](../../../../../module-extension.md) does not split. If $V=W\oplus U$ for a [submodule](../../../../../submodule.md) $U$, then $U$ would be a one-dimensional [trivial Lie algebra representation](../../../../../trivial-lie-algebra-representation.md), since it maps isomorphically to $V/W$. But $\ker H=kv_0$ and $Fv_0=v_1\ne0$, so no such $U$ exists. Thus

$$
\boxed{\begin{gathered}W=\bigoplus_{i\geq1}kv_i,\qquad V/W\cong k_{\mathrm{triv}},\\\text{Submodules: }0,W,V;\qquad V\text{ is not semisimple}.\end{gathered}}
$$

Here [semisimple module](../../../../../semisimple-module.md) means a [direct sum of modules](../../../../../direct-sum-of-modules.md) that are [simple modules](../../../../../irreducible-module.md), equivalently a module in which every [submodule](../../../../../submodule.md) has a complementary [submodule](../../../../../submodule.md). This is the [nonsplit zero-weight Verma extension for sl2](../../../../../nonsplit-zero-weight-verma-extension-for-sl2.md): rescaling to $w_i=i!v_i$ gives $Fw_i=w_{i+1}$ and $Ew_i=i(1-i)w_{i-1}$. Its [infinite-dimensional vector space](../../../../../infinite-dimensional-vector-space.md) is outside the hypotheses of the [Weyl complete reducibility theorem](../../../../../weyl-complete-reducibility-theorem.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the lie algebras course of Part C of the mathematics course of the University of Oxford](../../../../split.md)
6. [Lie algebras course of Part C of the mathematics course of the University of Oxford](../../../../../lie-algebras-course-of-part-c-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
