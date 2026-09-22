<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

Work with $x$ modulo $p-1$ and $u$ modulo $p$. By [Fermat's little theorem](../../../../../fermat-little-theorem.md), $a^{p-1}=1$ in $\mathbb F_p$, so the factor $a^y$ is independent of the chosen representative of $y$. The proposed multiplication is therefore well defined on the stated [Cartesian product](../../../../../cartesian-product.md). Its two associative bracketings have the same second component:

$$
a^z(a^yu+v)+w=a^{y+z}u+a^zv+w,
$$

and both have first component $x+y+z$. The [identity element](../../../../../identity-element.md) is $(0,0)$, and the two-sided [inverse element](../../../../../inverse-element.md) is

$$
\boxed{(x,u)^{-1}=(-x,-a^{-x}u)}.
$$

Thus the multiplication defines the [twisted cyclic pair group](../../../../../twisted-cyclic-pair-group.md), of order $p(p-1)$.

If $a=1$, multiplication is coordinatewise addition, so the [group](../../../../../group-split.md) is abelian. If $a\ne1$, then $p>2$ and both $(1,0)$ and $(0,1)$ are available; their products in opposite orders are $(1,1)$ and $(1,a)$. They differ. Hence

$$
\boxed{G\text{ is abelian}\iff a=1.}
$$

Both $H$ and $K$ contain the [identity element](../../../../../identity-element.md) and are closed under the multiplication and inverses: they are the [cyclic groups](../../../../../cyclic-group.md) of orders $p-1$ and $p$ respectively. Conjugation gives, with all coordinates reduced in the appropriate modulus,

$$
(x,u)(0,v)(x,u)^{-1}=(0,a^{-x}v),
$$

so $K$ is a [normal subgroup](../../../../../normal-subgroup.md). For $H$, the corresponding calculation is

$$
(x,u)(y,0)(x,u)^{-1}=(y,a^{-x}(a^y-1)u).
$$

When $a=1$ this lies in $H$. Conversely, for $a\ne1$, take $x=0$, $u=1$, $y=1$: the second coordinate is $a-1\ne0$, so $H$ is not normal. Thus **$H$ is normal precisely when $a=1$**.

Finally, the projection

$$
\boxed{\pi:G\longrightarrow\mathbb Z/(p-1)\mathbb Z,\qquad\pi(x,u)=x}
$$

is a surjective [group homomorphism](../../../../../group-homomorphism.md) because the first coordinates add. Its [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) is exactly $K$. At $p=2$, $a=1$ is the only possibility and the first factor is trivial, consistent with every conclusion. No assumption that $a$ generates the multiplicative [group](../../../../../group-split.md) of the [finite field](../../../../../finite-field.md) is needed.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
