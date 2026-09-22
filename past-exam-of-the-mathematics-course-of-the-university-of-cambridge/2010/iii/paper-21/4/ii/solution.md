<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $\mathcal C_0=\mathbf{Set}$. The initial free construction $L_0:\mathbf{Set}\to\mathcal C_1$ sends $A$ to $A\times\mathbb N$ with $\alpha_1(a,k)=(a,k+1)$. A [function](../../../../../../function-split.md) $f:A\to UB$ extends uniquely by $(a,k)\mapsto\beta_1^k(f(a))$. Its induced [monad](../../../../../../monad.md) is $T_0A=A\times\mathbb N$, with unit $a\mapsto(a,0)$ and multiplication $(a,k,l)\mapsto(a,k+l)$. An [algebra for a monad](../../../../../../algebra-for-a-monad.md) is determined by the action of $1\in\mathbb N$, so its [Eilenberg-Moore category](../../../../../../eilenberg-moore-category.md) is $\mathcal C_1$. Thus this first free–forgetful adjunction is a [monadic adjunction](../../../../../../monadic-adjunction.md) without needing the given assumption for $n=0$.

The [monadic length](../../../../../../monadic-length.md) counts successive [Eilenberg-Moore comparison functor](../../../../../../eilenberg-moore-comparison-functor.md) steps until the comparison becomes an equivalence. Fix $0\leq m<n$. For $m\geq1$, the free construction in the preceding part adds the $(m+1)$st operation with no fixed points. For $m=0$, the free first operation also has no fixed points. Consequently the [left adjoint](../../../../../../adjoint-functors.md) $F_{n,m}$ to the composite forgetful functor $U_{n,m}:\mathcal C_n\to\mathcal C_m$ is obtained by the one-step free construction, followed by empty higher operations. In particular, its underlying object of $\mathcal C_m$, unit and multiplication are exactly those of the one-step adjunction:

$$
U_{n,m}F_{n,m}=U_mL_m=T_m
$$

as [monads](../../../../../../monad.md), not merely as object functions. The multiplication agrees because both counits evaluate the same first new operation and the same chains; no later operation has a value on a free object.

By the assumed one-step [monadic adjunction](../../../../../../monadic-adjunction.md) property, or the explicit argument above when $m=0$, the [Eilenberg-Moore category](../../../../../../eilenberg-moore-category.md) $\mathcal C_m^{T_m}$ is equivalent to $\mathcal C_{m+1}$. Under this equivalence the comparison $\mathcal C_n\to\mathcal C_m^{T_m}$ is precisely $U_{n,m+1}$. Indeed, its algebra action evaluates each newly adjoined chain using $\alpha_1$, and evaluates the first new value using $\alpha_{m+1}$; it retains that operation and ignores all higher ones. The comparison has a left adjoint by the same explicit free extension. Thus the whole [monadic tower for nested partial unary operations](../../../../../../monadic-tower-for-nested-partial-unary-operations.md) is

$$
\mathbf{Set}=\mathcal C_0,\quad\mathcal C_1,\quad\ldots,\quad\mathcal C_n,
$$

with the remaining comparison at stage $m$ equal to $U_{n,m}$, and stage $n$ the identity.

It does not terminate earlier. If $m<n$, take the same underlying two-element [set](../../../../../../set-split.md) in two objects of $\mathcal C_n$, making every operation up to $m$ the identity. In the first object make all remaining operations identities; in the second make $\alpha_{m+1}$ exchange the two elements, and leave all subsequent operations undefined. Both satisfy the nesting rule. The identity function is a morphism after forgetting to $\mathcal C_m$, but is not a morphism between the original objects. Thus $U_{n,m}$ is not a [full functor](../../../../../../full-functor.md), and cannot be an equivalence. Therefore

$$
\boxed{\operatorname{monadic\ length}(\mathcal C_n\to\mathbf{Set})=n.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
