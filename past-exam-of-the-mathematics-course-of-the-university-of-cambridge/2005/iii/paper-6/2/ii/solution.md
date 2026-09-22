<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We prove the extension by [Zorn's lemma](../../../../../../zorn-s-lemma.md), retaining the full domination condition. Consider all pairs $(Y,S)$ extending $(Y_0,T_0)$, with $Y$ a subspace and $S$ linear, satisfying $S(y)\leq p(x+y)-q(x)$ for every $x\in X,y\in Y$. Order these pairs by extension. A chain has an upper bound: take the union of its subspaces and maps. The union is a subspace, and its map is well defined and linear because any finitely many vectors lie together in one member of the chain. Its domination is inherited there. Thus a maximal extension exists.

Suppose its domain $Y$ is proper, and choose $z\notin Y$. A linear extension to $Y+\mathbb Rz$ has the form $S_a(y+tz)=S(y)+ta$. Define the [admissible values for a sandwich extension](../../../../../../admissible-values-for-a-sandwich-extension.md) by

$$
A=\sup_{x',y'}\{S(y')-p(x'+y'-z)+q(x')\},
$$



$$
B=\inf_{x,y}\{-S(y)+p(x+y+z)-q(x)\},
$$

with $x,x'\in X$ and $y,y'\in Y$. Part (i) shows every quantity in the [supremum](../../../../../../supremum.md) is at most every quantity in the [infimum](../../../../../../infimum.md), hence $A\leq B$. Both bounds are real and finite: choosing zero vectors provides $A\geq-p(-z)$ and $B\leq p(z)$, and the pairwise comparison then bounds them from the other sides. Choose $a\in[A,B]$.

For $t>0$, [positive homogeneity](../../../../../../positively-homogeneous-function-degree-one.md) and the upper bound on $a$, used with $x/t,y/t$, give

$$
S(y)+ta\leq t\big[p(x/t+y/t+z)-q(x/t)\big]
=p(x+y+tz)-q(x).
$$

For $t=-s<0$, the lower bound on $a$ applied to $x/s,y/s$ gives

$$
a\geq S(y/s)-p(x/s+y/s-z)+q(x/s),
$$

which rearranges to $S(y)-sa\leq p(x+y-sz)-q(x)$. For $t=0$ this is the existing domination. Thus $S_a$ is a legitimate larger extension, contradicting maximality. The maximal domain is therefore all of $X$; call its map $T$.

Setting the first vector in the domination to zero yields $T(v)\leq p(v)$. Setting it to $v$ and the domain vector to $-v$ yields $-T(v)\leq-q(v)$. Consequently

$$
\boxed{T|_{Y_0}=T_0,\qquad T(y)\leq p(x+y)-q(x),\qquad q(v)\leq T(v)\leq p(v).}
$$

The one-dimensional extension has checked both signs of its coefficient; [positive homogeneity](../../../../../../positively-homogeneous-function-degree-one.md) alone does not permit treating negative coefficients as positive ones.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
