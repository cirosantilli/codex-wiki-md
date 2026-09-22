<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Here $\phi$ is a finite real [convex function](../../../../../convex-function.md) on the whole real [vector space](../../../../../vector-space-split.md); no topology or continuity is required. We prove the [convex domination form of the Hahn-Banach theorem](../../../../../convex-domination-form-of-the-hahn-banach-theorem.md) by extending across one vector. Suppose a [linear functional](../../../../../linear-functional.md) $f$ is already dominated on a [vector subspace](../../../../../vector-subspace.md) $W$ and choose $v\notin W$. For $w\in W$ and positive $t,s$, the proposed extension $g(w+\tau v)=f(w)+\tau c$ must satisfy the bounds

$$
L=\sup_{w\in W,\ t>0}\frac{f(w)-\phi(w-tv)}{t}\le c\le
U=\inf_{w\in W,\ s>0}\frac{\phi(w+sv)-f(w)}{s}.
$$

To prove compatibility, take $w_1,w_2\in W$ and $t,s>0$. The [convex combination](../../../../../convex-combination.md) of $w_1-tv$ and $w_2+sv$ with weights $s/(s+t)$ and $t/(s+t)$ lies in $W$. Domination there and [convexity](../../../../../convex-function.md) give

$$
sf(w_1)+tf(w_2)\le s\phi(w_1-tv)+t\phi(w_2+sv).
$$

Rearranging proves every lower candidate is at most every upper candidate. Also the candidates $w=0,t=s=1$ show

$$
-\phi(-v)\le L\le U\le\phi(v).
$$

Thus both endpoints are finite, and some $c\in[L,U]$ exists. For $\tau>0$ the upper bound gives domination of $f(w)+\tau c$; for $\tau<0$ the lower bound gives it; and for $\tau=0$ domination was assumed. This defines a dominated [linear functional](../../../../../linear-functional.md) on $W+\mathbb Rv$ extending $f$.

Order all dominated extensions by inclusion of their domains and agreement of values. A chain has the union extension, still linear and dominated. By [Zorn's lemma](../../../../../zorn-s-lemma.md) there is a maximal extension. The one-vector construction would enlarge any proper domain, so its domain is $V$. Hence **there is a full linear extension with $\boxed{g|_W=f,\quad g\le\phi}$**. A [convex function](../../../../../convex-function.md) here need not be positively homogeneous; this is why the bounds included all positive $s,t$.

Now fix $y\in V$. The translated [convex function](../../../../../convex-function.md) $\varphi_y(z)=\phi(y+z)-\phi(y)$ vanishes at zero. Apply the just-proved extension theorem to the zero [linear functional](../../../../../linear-functional.md) on $\{0\}$ to obtain a [linear functional](../../../../../linear-functional.md) $\ell_y$ with $\ell_y(z)\le\varphi_y(z)$ for every $z$. Set

$$
a_y(x)=\phi(y)+\ell_y(x-y).
$$

This is an [affine function](../../../../../affine-function.md), satisfies $a_y(x)\le\phi(x)$ for every $x$, and has $a_y(y)=\phi(y)$. Let $A=\{a_y:y\in V\}$. Every member is an affine minorant, while the member indexed by $x$ attains $\phi(x)$ at $x$. Thus **the exact representation is**

$$
\boxed{\phi(x)=\sup_{a\in A}a(x)\quad(x\in V).}
$$

This is the [finite convex function as supremum of affine minorants](../../../../../finite-convex-function-as-supremum-of-affine-minorants.md) property. The [linear functionals](../../../../../linear-functional.md) are algebraic; without a topology no assertion of continuous affine minorants is intended.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
