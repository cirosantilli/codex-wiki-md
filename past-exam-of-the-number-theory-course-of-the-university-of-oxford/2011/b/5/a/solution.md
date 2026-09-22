<h1 id="b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Kummer-Dedekind theorem](../../../../../kummer-dedekind-theorem.md) states the following. If $K=\mathbb Q(\theta)$ with $\theta$ integral and $p\nmid[\mathcal O_K:\mathbb Z[\theta]]$, factor the [minimal polynomial](../../../../../minimal-polynomial.md) modulo $p$ as $\bar f=\prod_i\bar g_i^{e_i}$ into distinct monic irreducible factors. Then

$$
p\mathcal O_K=\prod_i\mathfrak p_i^{e_i},\qquad
\mathfrak p_i=(p,g_i(\theta)),\qquad
N(\mathfrak p_i)=p^{\deg g_i}.
$$

The index restriction is essential.

For the proposed [ideal](../../../../../ideal.md) relation, reflexivity uses $\alpha=\beta=1$ and symmetry interchanges $\alpha,\beta$. If $(\alpha)I_1=(\beta)I_2$ and $(\gamma)I_2=(\delta)I_3$, multiplication gives $(\alpha\gamma)I_1=(\beta\delta)I_3$. All multipliers remain nonzero. Thus it is an [equivalence relation](../../../../../equivalence-relation.md), namely equality of [ideal classes](../../../../../ideal-class.md).

Put $s=\sqrt{-2}$. The [minimal polynomial](../../../../../minimal-polynomial.md) is $x^2+2$ and the given full power [basis](../../../../../basis.md) makes every prime eligible for the theorem. Modulo $3$ its roots are $\pm1$; modulo $5$ and $7$ it is irreducible; modulo $17$ its roots are $\pm7$. Consequently

$$
\boxed{\begin{aligned}
(3)&=(3,s-1)(3,s+1),\\
(5)&\text{ is prime},\\
(7)&\text{ is prime},\\
(17)&=(17,s-7)(17,s+7).
\end{aligned}}
$$

The two inert ideals have norms $25$ and $49$; each split factor has [norm](../../../../../norm.md) equal to its rational prime.

For $p_1\equiv1\pmod8$, [quadratic reciprocity](../../../../../quadratic-reciprocity.md) and its supplementary laws give $(-2/p_1)=1$. Thus $x^2+2$ has two distinct roots modulo $p_1$, giving distinct prime ideals $P,P'$ with

$$
(p_1)=PP',\qquad N(P)=N(P')=p_1.
$$

The given [principal ideal domain](../../../../../principal-ideal-domain.md) property makes $P=(x+ys)$ for some integers $x,y$. Taking norms, which are positive here, gives $p_1=N(P)=x^2+2y^2$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the number theory course of the University of Oxford](../../../../split.md)
6. [Number theory course of the University of Oxford](../../../../../number-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
