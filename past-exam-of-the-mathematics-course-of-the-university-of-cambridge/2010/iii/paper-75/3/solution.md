<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write a [coalgebra for a comonad](../../../../../coalgebra-for-a-comonad.md) as $(A,a)$ with $a:A\to GA$, $\epsilon_Aa=1_A$ and $\delta_Aa=Ga\,a$. Since the [Cartesian comonad](../../../../../cartesian-comonad.md) $G$ preserves [finite limits](../../../../../finite-limit.md), the [forgetful functor](../../../../../forgetful-functor.md) $U:\mathcal E_G\to\mathcal E$ creates them: for an underlying limit $K$ of coalgebras, the maps $K\to A_i\to GA_i$ induce a unique $K\to GK$ using $GK\cong\lim_iGA_i$. Its counit and coassociativity equations follow after every limiting projection, which jointly detect equality. The same argument makes the limiting cone universal among coalgebra cones. Thus $\mathcal E_G$ is a [Cartesian category](../../../../../cartesian-category.md); in particular, the product structure on $A\times B$ is $a\times b$ followed by the comparison $GA\times GB\cong G(A\times B)$.

An [exponential object](../../../../../exponential-object.md) needs more than the underlying ambient $B^A$. The [cofree coalgebra](../../../../../cofree-coalgebra.md) functor is $R(D)=(GD,\delta_D)$, with [adjunction](../../../../../adjoint-functors.md)

$$
\mathcal E_G((C,c),R(D))\cong\mathcal E(C,D),\qquad
h\longmapsto\widetilde h=Gh\,c.
$$

The inverse sends $\widetilde h$ to $\epsilon_D\widetilde h$; the [comonad](../../../../../comonad.md) laws verify that these are inverse and that $\widetilde h$ is a coalgebra map.

For $(A,a)$ and $(B,b)$, put $D=B^A$ and $W=(GB)^A$ in the ambient [Cartesian closed category](../../../../../cartesian-closed-category.md). Define $p,q:GD\to W$ by

$$
p=b^A\epsilon_D,
$$

and by transposing the composite

$$
GD\times A\xrightarrow{1\times a}GD\times GA
\cong G(D\times A)\xrightarrow{G\operatorname{ev}}GB
$$

to obtain $q$. Their cofree-adjoint transposes are coalgebra maps

$$
p^\sharp=Gp\,\delta_D,\qquad q^\sharp=Gq\,\delta_D:
R(D)\rightrightarrows R(W).
$$

Take their coalgebra [equalizer](../../../../../equaliser.md) $e:H\hookrightarrow R(D)$, which exists by the finite-limit construction.

To verify its universal property, let $h:C\to D$ transpose to $t:C\times A\to B$. Its coalgebra transpose $\widetilde h=Gh\,c$ factors through $H$ exactly when $p^\sharp\widetilde h=q^\sharp\widetilde h$. By the cofree [adjunction](../../../../../adjoint-functors.md), this equality is equivalent to $p\widetilde h=q\widetilde h$. The first side is $b^Ah$, because $\epsilon_DGh\,c=h$; transposing the second side gives $Gt$ composed with the product coalgebra structure on $C\times A$. The equality therefore says exactly

$$
bt=Gt\,(c\times a),
$$

with the canonical product comparison understood: precisely the condition that $t$ is a coalgebra map. Thus

$$
\boxed{\mathcal E_G(C,H)\cong\mathcal E_G(C\times A,B)}
$$

naturally in the coalgebra $C$. Its evaluation is ambient evaluation after $\epsilon_De\times1_A$, and the preceding condition makes it a coalgebra map. **This equalizer is the coalgebra exponential, so the category of coalgebras is cartesian closed.** This [Cartesian closure for a finite-limit-preserving comonad](../../../../../cartesian-closure-for-a-finite-limit-preserving-comonad.md) uses no subobject classifier on $\mathcal E$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
