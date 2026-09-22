<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Here is an elementary [polynomial pencil with four square members](../../../../../../polynomial-pencil-with-four-square-members.md) argument. Suppose first that $u,v$ are linearly dependent. Their [coprimality of polynomials](../../../../../../coprime-polynomials.md) then forces both to be constant. Otherwise write the four distinct members as $L_j=\alpha_j u+\beta_jv=s_j^2$. They are nonzero and pairwise [coprime polynomials](../../../../../../coprime-polynomials.md): a common nonconstant factor of two members would divide both $u$ and $v$.

Put $d=\max(\deg u,\deg v)>0$. At most one member of the pencil has [degree of a polynomial](../../../../../../degree-of-a-polynomial.md) smaller than $d$, since cancellation of its leading coefficient determines a unique projective pair. Choose a member $L_k$ of minimal degree $e$ and any independent member $L_l$ of degree $d$. The [polynomial](../../../../../../polynomial-split.md)

$$
W=L_k^{\prime}L_l-L_kL_l^{\prime}
$$

is nonzero: otherwise the [rational function](../../../../../../rational-function.md) $L_k/L_l$ would have zero [derivative](../../../../../../derivative.md), hence would be constant in characteristic zero. Its degree is at most $d+e-1$; if both members have degree zero the original $d>0$ assumption has already failed.

Replacing this pair by any other independent pair changes $W$ only by a nonzero scalar. Since $L_j=s_j^2$, each $s_j$ divides $W$. The pairwise [coprimality of polynomials](../../../../../../coprime-polynomials.md) therefore gives $\prod_j s_j\mid W$. But three members have degree $d$, so

$$
\deg W\ \geq\sum_{j=1}^4\deg s_j
\ \geq\frac{3d+e}{2}
\ >d+e-1,
$$

a contradiction. **Consequently $u$ and $v$ are constant.** The possibility that a member is zero was already covered by linear dependence.

To apply this to an [elliptic curve](../../../../../../elliptic-curve.md), complete the square in its [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) and work over $\mathbb C$. Nonsingularity gives three distinct roots $e_1,e_2,e_3$, so the equation becomes $y^2=\prod_{j=1}^3(x-e_j)$. A nonconstant [rational parametrization of an algebraic curve](../../../../../../rational-parametrization-of-an-algebraic-curve.md) would have $x=u/v$ with [coprime polynomials](../../../../../../coprime-polynomials.md). Clearing denominators gives

$$
(yv^2)^2=v(u-e_1v)(u-e_2v)(u-e_3v).
$$

The four factors are pairwise [coprime polynomials](../../../../../../coprime-polynomials.md). A [rational function](../../../../../../rational-function.md) whose square is a [polynomial](../../../../../../polynomial-split.md) is itself a [polynomial](../../../../../../polynomial-split.md), by comparing numerator and denominator in lowest terms. [Unique factorization](../../../../../../unique-factorization-in-an-integral-domain.md), and the fact that every nonzero complex constant has a square root, make each of these four factors a square in $\mathbb C[t]$. They correspond to four distinct projective pairs. The result just proved forces $u,v$ to be constant, and the equation then forces $y$ to be constant as well. **This proves the [nonparametrizability of an elliptic curve](../../../../../../nonparametrizability-of-an-elliptic-curve.md).**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
