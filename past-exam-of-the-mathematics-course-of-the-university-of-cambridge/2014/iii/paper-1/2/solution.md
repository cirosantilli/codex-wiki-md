<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [prime ideal](../../../../../prime-ideal.md) $\mathfrak p$ is minimal over $I$ if $I\subseteq\mathfrak p$ and no strictly smaller prime contains $I$. An [associated prime of a module](../../../../../associated-prime-of-a-module.md) is an [annihilator](../../../../../annihilator-ring-theory.md) of an individual nonzero element which happens to be prime. For the quotient [module](../../../../../module-mathematics.md) this reads

$$
\boxed{\operatorname{Ass}_R(R/I)=\{\operatorname{Ann}_R(\bar a):0\neq\bar a\in R/I,\ \operatorname{Ann}_R(\bar a)\text{ prime}\},}
$$

where $\operatorname{Ann}_R(\bar a)=(I:a)=\{r\in R:ra\in I\}$. This is the [annihilator](../../../../../annihilator-ring-theory.md) of an individual element, rather than necessarily the [annihilator](../../../../../annihilator-ring-theory.md) of the whole quotient.

Minimal primes exist because $I$ is proper. First choose a [maximal ideal](../../../../../maximal-ideal.md) containing $I$. Within the primes contained in it and containing $I$, an intersection of any decreasing chain is again prime. Indeed, if $ab$ is in the intersection and $a$ is absent from one member, then $b$ belongs to that member and to every smaller member; it also belongs to every larger member. The intersection is still proper and contains $I$. [Zorn's lemma](../../../../../zorn-s-lemma.md), applied with reverse inclusion, produces a minimal prime. This proves [existence of minimal primes over a proper ideal](../../../../../existence-of-minimal-primes-over-a-proper-ideal.md), even without the [Noetherian](../../../../../noetherian-ring.md) hypothesis.

Now fix a minimal prime $\mathfrak p$ and put $A=R/I$. The [localization at a prime ideal](../../../../../localization-at-a-prime-ideal.md) $A_{\mathfrak p}$ is nonzero and is a [Noetherian local ring](../../../../../noetherian-local-ring.md). By [prime ideal correspondence for localization](../../../../../prime-ideal-correspondence-for-localization.md), its only prime is $\mathfrak pR_{\mathfrak p}/IR_{\mathfrak p}$. Write this [maximal ideal](../../../../../maximal-ideal.md) as $\mathfrak n$. It is the [nilradical](../../../../../nilradical.md); since it is finitely generated and each generator is nilpotent, some power of $\mathfrak n$ is zero. Explicitly, if its generators have nilpotence exponents $e_1,\ldots,e_r$, every product of degree $1+\sum_i(e_i-1)$ vanishes.

Choose the smallest $s\geq1$ such that $\mathfrak n^s=0$, and choose a nonzero element in $\mathfrak n^{s-1}$; when $\mathfrak n=0$, choose $1$. Its [annihilator](../../../../../annihilator-ring-theory.md) over $R_{\mathfrak p}$ is exactly $\mathfrak pR_{\mathfrak p}$. Represent it as $a/u$ with $u\notin\mathfrak p$. Multiplication by the unit $u$ shows that $a/1$ has the same [annihilator](../../../../../annihilator-ring-theory.md) and remains nonzero.

Let $p_1,\ldots,p_r$ generate $\mathfrak p$ in $R$. For each $i$, the equality $p_i a/1=0$ supplies $u_i\notin\mathfrak p$ such that $u_i p_i\bar a=0$ in $A$. Put $u=\prod_i u_i$ and $\bar b=u\bar a$. Its localization is nonzero, so $\bar b\neq0$, and every element of $\mathfrak p$ kills it. Conversely, an element outside $\mathfrak p$ becomes a unit and cannot kill the nonzero element $\bar b/1$. Therefore

$$
\operatorname{Ann}_R(\bar b)=\mathfrak p,\qquad\boxed{\varnothing\neq\operatorname{Min}_R(I)\subseteq\operatorname{Ass}_R(R/I).}
$$

The key step in [minimal primes are associated primes](../../../../../minimal-primes-are-associated-primes.md) is clearing denominators for a finite generating set of $\mathfrak p$; that is where [Noetherianity](../../../../../noetherian-ring.md) is used.

For an [embedded associated prime](../../../../../embedded-associated-prime.md), take $R=k[x,y]$ and $I=(x^2,xy)$. Its radical is $(x)$, so $(x)$ is its unique minimal prime. The nonzero class of $x$ satisfies

$$
\operatorname{Ann}_R(\bar x)=(I:x)=(x,y).
$$

Indeed, $rx\in x(x,y)$ is equivalent to $r\in(x,y)$ by cancellation in the polynomial domain. Thus **$(x,y)$ is associated but is not minimal**, since $(x)\subsetneq(x,y)$. For comparison, $\operatorname{Ann}_R(\bar y)=(x)$, exhibiting the minimal associated prime as well.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
