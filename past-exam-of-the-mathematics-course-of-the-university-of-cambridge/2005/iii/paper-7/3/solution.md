<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

First, a [maximal left ideal](../../../../../maximal-left-ideal.md) $L$ is [closed](../../../../../closed-set.md). Its [norm](../../../../../norm.md) closure is again a [left ideal](../../../../../left-ideal.md), since multiplication is [continuous](../../../../../continuous-function.md). If that closure were all of $A$, some $\ell\in L$ would satisfy $\|1-\ell\|<1$ and would be invertible by the [Neumann series](../../../../../neumann-series.md). But a proper [left ideal](../../../../../left-ideal.md) cannot contain an invertible element: $\ell^{-1}\ell=1$ would put $1$ in $L$. Maximality therefore forces $\overline L=L$.

Consequently $X=A/L$ is a nonzero [quotient Banach space](../../../../../quotient-banach-space.md). It is a [simple module](../../../../../irreducible-module.md) for left multiplication by $A$, because the inverse image of any [submodule](../../../../../submodule.md) under $A\to A/L$ is a [left ideal](../../../../../left-ideal.md) containing $L$, and hence is either $L$ or $A$. Since $La\subseteq L$, right multiplication defines a well-defined bounded [module endomorphism](../../../../../module-endomorphism.md)

$$
T:X\longrightarrow X,\qquad T(u+L)=ua+L,\qquad\|T\|\le\|a\|.
$$

Indeed, changing $u$ by an element of $L$ changes $ua$ by an element of $L$, and taking the infimum over representatives proves the [quotient norm](../../../../../quotient-norm.md) bound. Right multiplication commutes with the left action by [associativity](../../../../../associative-property.md).

Choose $\lambda$ in the nonempty [spectrum of an element](../../../../../spectrum-of-an-element.md) of $T$ in the [Banach algebra](../../../../../banach-algebra-split.md) $\mathcal B(X)$. Both the [kernel](../../../../../kernel-of-a-linear-map.md) and range of $T-\lambda I$ are [submodules](../../../../../submodule.md). If this [module endomorphism](../../../../../module-endomorphism.md) were nonzero, simplicity would force its [kernel](../../../../../kernel-of-a-linear-map.md) to be zero and its range to be all of $X$. It would be a bounded bijection of [Banach spaces](../../../../../banach-space-split.md), with bounded inverse by the [bounded inverse theorem](../../../../../bounded-inverse-theorem.md), contradicting the choice of $\lambda$. Thus $T=\lambda I$. Applying this identity to $1+L$ yields $a-\lambda1\in L$. If also $a-\mu1\in L$, then $(\lambda-\mu)1\in L$; since $1\notin L$, $\lambda=\mu$. Therefore

$$
\boxed{\text{There is exactly one }\lambda\in\mathbb C\text{ with }a-\lambda1\in L.}
$$

This is the [scalar right action on a maximal-left-ideal quotient](../../../../../scalar-right-action-on-a-maximal-left-ideal-quotient.md); it does not assume that $L$ is a two-sided ideal or that $A/L$ is an algebra.

Now consider the [center of an associative algebra](../../../../../center-of-an-associative-algebra.md) $Z$. For each $u\in A$, the map $z\mapsto zu-uz$ is a [continuous](../../../../../continuous-function.md) [linear map](../../../../../linear-map.md), so its [kernel](../../../../../kernel-of-a-linear-map.md) is [closed](../../../../../closed-set.md). Their intersection $Z$ is therefore [closed](../../../../../closed-set.md). The identity belongs to $Z$, as do sums and scalar multiples of its elements. If $z,w\in Z$, then for every $u\in A$,

$$
(zw)u=z(wu)=z(uw)=(zu)w=(uz)w=u(zw).
$$

Thus $zw\in Z$. Also $zw=wz$, since $z$ commutes with every element of $A$, including $w$. Hence **the center is a [closed](../../../../../closed-set.md) [commutative](../../../../../commutativity.md) unital [subalgebra](../../../../../subalgebra.md)**, and is a [Banach algebra](../../../../../banach-algebra-split.md) in the inherited [norm](../../../../../norm.md).

For every $z\in Z$, the inclusion $Lz=zL\subseteq L$ allows the first argument to apply. Let $\chi(z)$ be the unique scalar for which $z-\chi(z)1\in L$. Equivalently, the induced right multiplication on $A/L$ is $T_z=\chi(z)I$. Since

$$
T_{z+w}=T_z+T_w,\qquad T_{\alpha z}=\alpha T_z,\qquad T_{zw}=T_wT_z,\qquad T_1=I,
$$

the map $\chi:Z\to\mathbb C$ is a complex-linear unital [character of an algebra](../../../../../character-of-an-algebra.md). It is surjective because $\chi(\alpha1)=\alpha$, and its [kernel](../../../../../kernel-of-a-linear-map.md) is precisely $L\cap Z$. Consequently

$$
\boxed{Z/(L\cap Z)\cong\mathbb C,\qquad L\cap Z\text{ is a maximal ideal of }Z.}
$$

Indeed any ideal properly containing the [kernel](../../../../../kernel-of-a-linear-map.md) would have a nonzero image in the [field](../../../../../field.md) $\mathbb C$ and thus would be all of $Z$. The [algebra character](../../../../../character-of-an-algebra.md) is also [continuous](../../../../../continuous-function.md): $|\chi(z)|=\|\chi(z)I\|=\|T_z\|\le\|z\|$, although [continuity](../../../../../continuous-function.md) is not needed for maximality.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
