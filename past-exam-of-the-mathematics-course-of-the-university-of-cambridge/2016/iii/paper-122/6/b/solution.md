<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use right [comodules](../../../../../../comodule.md) with [coaction](../../../../../../coaction.md) $u\mapsto\sum u_{(0)}\otimes u_{(1)}$. Fix the convention that $\diamond$ is induced by $m$ and $\bullet$ by $n$. We classify lax monoidal structures first; the strong case is identified at the end.

Every [natural transformation](../../../../../../natural-transformation.md) of the indicated tensor bifunctors is determined by a [linear functional](../../../../../../linear-functional.md) $\gamma:H\otimes H\to k$, and its components have the [comodule tensor transformation formula](../../../../../../comodule-tensor-transformation-formula.md)

$$
\boxed{\varphi_{M,N}(u\otimes v)=\sum u_{(0)}\otimes v_{(0)}\gamma(u_{(1)},v_{(1)}).}
$$

To prove the assertion, set $\gamma=(\varepsilon\otimes\varepsilon)\varphi_{H,H}$. On the cofree [comodules](../../../../../../comodule.md) $V\otimes H,W\otimes H$, [naturality](../../../../../../naturality.md) with respect to $h\mapsto v\otimes h$ forces the component to act as $\varphi_{H,H}$ on the two $H$ factors. Apply [naturality](../../../../../../naturality.md) to the pair of coactions $M\to M\otimes H$, $N\to N\otimes H$, then apply their [counits](../../../../../../counit.md). This yields the formula. Conversely the formula is plainly natural with respect to comodule morphisms, and recovers $\gamma$ from the regular [comodules](../../../../../../comodule.md).

It remains to impose exactly three kinds of equations. First, the component must be $H$-colinear from the tensor with product $n$ to the tensor with product $m$. Expanding its two coactions gives **(C)**, the [multiplication compatibility for a comodule tensor transformation](../../../../../../multiplication-compatibility-for-a-comodule-tensor-transformation.md)

$$
\boxed{\sum m(a_{(1)},b_{(1)})\gamma(a_{(2)},b_{(2)})=\sum\gamma(a_{(1)},b_{(1)})n(a_{(2)},b_{(2)}).}
$$

Necessity follows by taking $M=N=H$ and applying the two [counits](../../../../../../counit.md); sufficiency follows by substituting the identity into the coaction formula for arbitrary $M,N$.

Second, the two unit triangles in the preceding part are exactly **(U)**:

$$
\boxed{\gamma(1,a)=\varepsilon(a),\qquad\gamma(a,1)=\varepsilon(a).}
$$

Here $1=j(1_k)$ is the common algebra unit. These identities are forced by the regular [comodule](../../../../../../comodule.md) and sufficient by the counit law.

Third, expand the associativity diagram on three right [comodules](../../../../../../comodule.md). The two scalar factors, after their [counits](../../../../../../counit.md) are removed, are **(A)**:

$$
\boxed{\sum\gamma(m(a_{(1)},b_{(1)}),c)\gamma(a_{(2)},b_{(2)})=\sum\gamma(a,m(b_{(1)},c_{(1)}))\gamma(b_{(2)},c_{(2)}).}
$$

The product in this expression is $m$, because the intermediate arguments $M\diamond N$ and $N\diamond P$ are source-tensor objects. Necessity follows from the three regular [comodules](../../../../../../comodule.md); sufficiency is the same substitution for arbitrary coactions. Using (C), the same condition can equivalently be written with the target product $n$:

$$
\sum\gamma(a_{(1)},b_{(1)})\gamma(n(a_{(2)},b_{(2)}),c)=\sum\gamma(b_{(1)},c_{(1)})\gamma(a,n(b_{(2)},c_{(2)})).
$$

This is the normalized [bialgebra scalar cocycle](../../../../../../bialgebra-scalar-cocycle.md) equation for that convention.

**Thus the required structures correspond bijectively to all linear maps $\gamma$ satisfying (C), (U) and (A).** No convolution invertibility has been imposed for a [lax monoidal functor](../../../../../../monoidal-functor.md) structure. If “monoidal” is required to mean strong, add precisely that $\gamma$ is invertible under the [convolution product for coalgebra maps](../../../../../../convolution-product-for-coalgebra-maps.md) on $\operatorname{Hom}_k(H\otimes H,k)$. Its convolution inverse $\bar\gamma$ supplies the inverse component by the same displayed formula; conversely natural inverse components recover a convolution inverse by the regular-comodule argument. In that case (C) is the explicit [bialgebra cocycle twist](../../../../../../bialgebra-cocycle-twist.md) relation

$$
\boxed{n(a,b)=\sum\bar\gamma(a_{(1)},b_{(1)})m(a_{(2)},b_{(2)})\gamma(a_{(3)},b_{(3)}).}
$$

This also records which multiplication lies on each side of the twist. Interchanging the names of $m,n$ interchanges the two tensor conventions, rather than silently changing the equation.

For a concrete lax example, take the two-dimensional [bialgebra](../../../../../../bialgebra.md) with basis $1,e$, product $e^2=e$, and $\Delta(e)=e\otimes e$, $\varepsilon(e)=1$. Set $m=n$ and $\gamma(1,1)=\gamma(1,e)=\gamma(e,1)=1$, $\gamma(e,e)=0$. Normalization and (C) hold, and (A) follows by checking the eight basis triples: triples involving $1$ reduce to normalization, and the triple $(e,e,e)$ has both sides zero. But the $(e,e)$ tensor component is zero, so this [lax monoidal functor](../../../../../../monoidal-functor.md) is not strong.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
