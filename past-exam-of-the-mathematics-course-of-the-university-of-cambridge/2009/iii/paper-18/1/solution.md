<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Throughout the algebraic questions, $C$ is a smooth projective connected [algebraic curve](../../../../../algebraic-curve.md) over the [algebraically closed field](../../../../../algebraically-closed-field.md) $k$. This is the curve convention needed for the [Jacobian variety](../../../../../jacobian-variety.md); for an arbitrary singular or nonproper curve the assertions need not hold. Choose $P_0\in C(k)$ and write $\pi:C\times T\to T$.

The degree-$d$ [Picard functor of a curve](../../../../../picard-functor-of-a-curve.md) is

$$
\mathcal P^d(T)=\{\mathcal L\in\operatorname{Pic}(C\times T):\deg\mathcal L_t=d\text{ for every geometric }t\}/\pi^*\operatorname{Pic}(T),
$$

with pullback as its action on morphisms. Equivalently, normalize $\mathcal L$ by tensoring with $\pi^*(\mathcal L|_{P_0\times T})^{-1}$ and remember the resulting trivialization along $P_0\times T$. Since $\pi_*\mathcal O_{C\times T}=\mathcal O_T$, an automorphism of a [line bundle](../../../../../line-bundle.md) is multiplication by a base unit; preservation of this trivialization forces that unit to be $1$. Thus normalized [line bundles](../../../../../line-bundle.md) have effective descent and the displayed [functor](../../../../../functor.md) is already the appropriate sheaf, rather than just a list of classes over fields.

Here is a construction of its representing [scheme](../../../../../scheme.md). The [symmetric product of a curve](../../../../../symmetric-product-of-a-curve.md) $C^{(r)}$ represents relative effective degree-$r$ [Cartier divisors](../../../../../cartier-divisor-split.md). It is projective, and its completed local ring at $\sum m_iQ_i$ is a power-series ring in the elementary symmetric coefficients of $m_i$ local parameters at each $Q_i$. Thus it is smooth of dimension $r$, in every characteristic. Put

$$
U=\{D\in C^{(g)}:H^1(C,\mathcal O_C(D))=0\}.
$$

This is open by the [semicontinuity theorem for coherent cohomology](../../../../../semicontinuity-theorem-for-coherent-cohomology.md). It is nonempty: choose $g$ points successively imposing independent vanishing conditions on $H^0(C,K_C)$, so that $H^0(C,K_C-D)=0$, and use [Serre duality](../../../../../serre-duality.md). The [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives $h^0(\mathcal O_C(D))=1$ on $U$.

For any fixed [line bundle](../../../../../line-bundle.md) $B$ of degree $g-d$, use a copy $U_B$ of $U$ with the universal normalized [line bundle](../../../../../line-bundle.md) $\mathcal O(D)\otimes B^{-1}$. This represents exactly the open subfunctor on which $H^1(\mathcal L_t\otimes B)=0$. Indeed, [cohomology and base change for line bundles on a curve](../../../../../cohomology-and-base-change-for-line-bundles-on-a-curve.md) makes $\pi_*(\mathcal L\otimes B)$ a rank-one [vector bundle](../../../../../vector-bundle.md). The evaluation morphism

$$
\pi^*\pi_*(\mathcal L\otimes B)\longrightarrow\mathcal L\otimes B
$$

has a unique relative zero [Cartier divisor](../../../../../cartier-divisor-split.md) of degree $g$ and recovers the point of $U_B$. No choice of a global generator on $T$ is needed. Conversely that zero [Cartier divisor](../../../../../cartier-divisor-split.md) recovers $\mathcal L$ modulo a bundle from $T$.

These charts cover: given any degree-$d$ [line bundle](../../../../../line-bundle.md) $L$, choose a nonspecial effective degree-$g$ [Cartier divisor](../../../../../cartier-divisor-split.md) $D$ and take $B=\mathcal O(D)\otimes L^{-1}$. On the overlap of $U_B$ and $U_{B'}$, the unique effective representative of $\mathcal O(D)\otimes B^{-1}\otimes B'$ is constructed by the same rank-one evaluation map. It therefore gives a regular transition morphism; uniqueness gives both the inverse and the cocycle identity. Gluing gives a [scheme](../../../../../scheme.md) $J^d$ representing $\mathcal P^d$, with a universal normalized [line bundle](../../../../../line-bundle.md).

The construction is of finite type, not an infinite union of indispensable charts. Choose $m\ge2g-1$ and a fixed [line bundle](../../../../../line-bundle.md) $F$ of degree $m-d$. Every $L\otimes F$ has a nonzero section by the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md), so the universal effective [Cartier divisor](../../../../../cartier-divisor-split.md) gives a surjection $C^{(m)}\to J^d$. The inverse images of the charts cover the projective, hence quasi-compact, [symmetric product of a curve](../../../../../symmetric-product-of-a-curve.md) $C^{(m)}$. A finite subcover gives finitely many charts for $J^d$. This surjection also makes $J^d$ irreducible. The charts show that it is smooth of dimension $g$.

For properness, apply the [valuative criterion for properness](../../../../../valuative-criterion-for-properness.md). Let $R$ be a discrete valuation $k$-algebra with fraction field $K$, and let $L_K$ be a degree-$d$ [line bundle](../../../../../line-bundle.md) on $C_K$. A rational section represents it by a [Cartier divisor](../../../../../cartier-divisor-split.md). Its closure in the regular surface $C_R$ is again a [Cartier divisor](../../../../../cartier-divisor-split.md), since regular local rings are factorial. Thus $L_K$ extends to a [line bundle](../../../../../line-bundle.md) on $C_R$, whose fibre degree remains $d$ by [constancy of line bundle degree in a family](../../../../../constancy-of-line-bundle-degree-in-a-family.md). Two extensions with the same generic class differ by a vertical [Cartier divisor](../../../../../cartier-divisor-split.md). The special fibre is irreducible, so that [Cartier divisor](../../../../../cartier-divisor-split.md) is an integer multiple of the entire fibre, the principal [Cartier divisor](../../../../../cartier-divisor-split.md) of a power of a uniformizer. The extensions therefore give the same normalized Picard class. This proves existence and uniqueness in the valuative criterion, hence separatedness and properness of the finite-type [scheme](../../../../../scheme.md) $J^d$.

Consequently **$\operatorname{Pic}^d_C=\operatorname{Jac}^d_C$ is a smooth proper $k$-variety of dimension $g$**. Tensoring by $\mathcal O_C(-dP_0)$ identifies it with $J^0$. On $J^0$ the [tensor product](../../../../../tensor-product.md) and inverse of [line bundles](../../../../../line-bundle.md) induce the algebraic group operations; it is the [Jacobian variety](../../../../../jacobian-variety.md), an [abelian variety](../../../../../abelian-variety-split.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
