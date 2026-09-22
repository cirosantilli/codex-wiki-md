<h1 id="4/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A point is in the [closure](../../../../../../../closure-topology.md) $\overline E$ exactly when every [neighbourhood](../../../../../../../neighbourhood-mathematics.md) meets $E$. This is equivalent to belonging to $E$ or being a [limit point](../../../../../../../limit-point.md) of $E$.

If $p\notin\overline E$, choose $\varepsilon>0$ with $(p-\varepsilon,p+\varepsilon)\cap E=\varnothing$. Every $q$ with $|q-p|<\varepsilon/2$ has a smaller [neighbourhood](../../../../../../../neighbourhood-mathematics.md) contained in this interval and disjoint from $E$. Thus $(p-\varepsilon/2,p+\varepsilon/2)$ misses $\overline E$, and the complement of $\overline E$ is [open](../../../../../../../open-set.md). Hence $\overline E$ is [closed](../../../../../../../closed-set.md).

Every [closed set](../../../../../../../closed-set.md) $F$ containing $E$ contains all [limit points](../../../../../../../limit-point.md) of $E$: a [limit point](../../../../../../../limit-point.md) outside $F$ would have a [neighbourhood](../../../../../../../neighbourhood-mathematics.md) missing $F$, and hence missing $E$. Therefore $\overline E\subseteq F$. Since $\overline E$ is itself one of these [closed sets](../../../../../../../closed-set.md),

$$
\boxed{\overline E=\bigcap\{F:E\subseteq F,\ F\text{ closed in }\mathbb R\}.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
