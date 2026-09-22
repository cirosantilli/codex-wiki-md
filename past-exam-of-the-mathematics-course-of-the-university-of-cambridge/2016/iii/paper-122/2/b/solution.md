<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [opmonoidal monad](../../../../../../opmonoidal-monad.md) on a [monoidal category](../../../../../../monoidal-category.md) is a [monad](../../../../../../monad.md) $(T,\eta,\mu)$ whose endofunctor is an [opmonoidal functor](../../../../../../opmonoidal-functor.md) and whose [unit and multiplication of a monad](../../../../../../unit-and-multiplication-of-a-monad.md) are [opmonoidal natural transformations](../../../../../../opmonoidal-natural-transformation.md). Suppress only the canonical parentheses. Explicitly,

$$
T_2\eta_{X\otimes Y}=\eta_X\otimes\eta_Y,\qquad T_0\eta_I=1_I,
$$



$$
T_2(X,Y)\mu_{X\otimes Y}=(\mu_X\otimes\mu_Y)T_2(TX,TY)T(T_2(X,Y)),\qquad T_0\mu_I=T_0T(T_0).
$$

The composite [opmonoidal functor](../../../../../../opmonoidal-functor.md) $T^2$ has tensor comparison $T_2(TX,TY)T(T_2(X,Y))$ and unit comparison $T_0T(T_0)$, explaining the last two equations.

For two [algebras for a monad](../../../../../../algebra-for-a-monad.md) $(X,a)$ and $(Y,b)$, define

$$
\boxed{(X,a)\otimes(Y,b)=\bigl(X\otimes Y,(a\otimes b)T_2(X,Y)\bigr),\qquad\mathbf I=(I,T_0).}
$$

Let $c=(a\otimes b)T_2(X,Y)$. The [unit law for a monad algebra](../../../../../../unit-law-for-a-monad-algebra.md) follows at once from the opmonoidality of $\eta$:

$$
c\eta_{X\otimes Y}=(a\eta_X)\otimes(b\eta_Y)=1.
$$

For the multiplication law, [naturality](../../../../../../naturality.md) of $T_2$, the algebra laws, and the opmonoidality of $\mu$ give

$$
\begin{aligned}
cT(c)&=(a\otimes b)(Ta\otimes Tb)T_2(TX,TY)T(T_2(X,Y))\\
&=(a\mu_X\otimes b\mu_Y)T_2(TX,TY)T(T_2(X,Y))\\
&=(a\otimes b)T_2(X,Y)\mu_{X\otimes Y}=c\mu_{X\otimes Y}.
\end{aligned}
$$

The two unit-comparison equations above similarly make $(I,T_0)$ a [algebra for a monad](../../../../../../algebra-for-a-monad.md). If $f,g$ are [morphisms of algebras for a monad](../../../../../../morphism-of-algebras-for-a-monad.md), [naturality](../../../../../../naturality.md) of $T_2$ shows that $f\otimes g$ is an algebra morphism.

For a third algebra $(Z,d)$, the base [associator](../../../../../../associator.md) is also an algebra morphism: its intertwining equation is precisely the opmonoidal associativity axiom, followed by $a\otimes b\otimes d$. The two base [unitors](../../../../../../unitor.md) are algebra morphisms by the opmonoidal unit axioms. Their pentagon and triangle commute because they commute after the faithful [forgetful functor](../../../../../../forgetful-functor.md), and the lifted maps have exactly the same underlying [morphisms](../../../../../../morphism.md).

**The [Eilenberg-Moore category](../../../../../../eilenberg-moore-category.md) is therefore monoidal**, with these lifted constraints. Its [forgetful functor](../../../../../../forgetful-functor.md) $U:\mathcal C^T\to\mathcal C$ preserves the tensor product, unit object and constraints exactly, so it is a [strict monoidal functor](../../../../../../strict-monoidal-functor.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
