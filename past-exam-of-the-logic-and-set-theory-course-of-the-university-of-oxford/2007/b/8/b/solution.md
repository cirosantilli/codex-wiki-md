<h1 id="b/8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A nonempty [weakly linear function](../../../../../weakly-linear-partial-function.md) has a domain $D$ closed under rational scalars and [addition](../../../../../addition.md), hence a [vector subspace](../../../../../vector-subspace.md) of $\mathbb R$ over $\mathbb Q$. Additivity first gives $f(0)=0$ and $f(-x)=-f(x)$, then $f(nx)=nf(x)$ for [integers](../../../../../integer-split.md) $n$. If $q=m/n$ with $n>0$, rational closure puts $qx$ in $D$ and

$$
n f(qx)=f(nqx)=f(mx)=m f(x).
$$

Thus $f(qx)=qf(x)$: it is a $\mathbb Q$-linear map. The [empty function](../../../../../empty-function.md) is not maximal because it extends to the [function](../../../../../function-split.md) on $\{0\}$ with value [zero](../../../../../zero-of-a-function.md).

Suppose a maximal $f$ had proper domain $D\ne\mathbb R$. Choose $t\notin D$ and any prescribed real value $a$, for instance $a=0$. Every element of $D+\mathbb Qt$ has a unique expression $d+qt$: if two expressions coincide and the coefficients differ, then $t$ would belong to $D$. Define

$$
h(d+qt)=f(d)+qa.
$$

Uniqueness makes this well-defined. The displayed [logical formula](../../../../../logical-formula.md) and the $\mathbb Q$-linearity of $f$ show directly that $h$ is additive and has a domain closed under rational scalars. Hence it is a [weakly linear function](../../../../../weakly-linear-partial-function.md) and extends $f$. It is a proper extension because $t$ is now in its domain, contradicting maximality. Therefore

$$
\boxed{\operatorname{dom}f=\mathbb R\quad\text{for every maximal }f\in\mathcal F.}
$$

Part (a) and [Zorn's lemma](../../../../../zorn-s-lemma.md) guarantee the existence of maximal extensions as well as this description of their domains.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
