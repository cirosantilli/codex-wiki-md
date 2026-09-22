<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the standard definition of a [partition regular matrix](../../../../../../partition-regular-matrix.md): for every [finite coloring](../../../../../../finite-coloring.md) of the [positive integers](../../../../../../positive-integer.md), there is a positive solution whose coordinates all have one color. Coordinates may repeat. Clearing denominators lets us assume $a_i\in\mathbb Z\setminus\{0\}$; multiplication of the row by a nonzero [rational number](../../../../../../rational-number.md) changes neither its zero-sum [subsets](../../../../../../subset.md) nor its solutions. We prove both directions of the [Rado theorem for one equation](../../../../../../rado-theorem-for-one-equation.md) directly, without invoking any form of [Rado's theorem](../../../../../../rado-s-theorem.md).

For necessity, choose a [prime number](../../../../../../prime-number.md) $p>\sum_i|a_i|$ and use the [last nonzero digit coloring](../../../../../../last-nonzero-digit-coloring.md): write $x=p^{v_p(x)}u$, with $p\nmid u$, and assign color $u\bmod p$. Given a [monochromatic](../../../../../../monochromatic-set.md) solution, let $v=\min_i v_p(x_i)$, let $I=\{i:v_p(x_i)=v\}$, and let $r\ne0$ be the common color. Divide $\sum_i a_i x_i=0$ by $p^v$ and reduce modulo $p$. Terms outside $I$ vanish; the others give

$$
r\sum_{i\in I}a_i\equiv0\pmod p.
$$

The nonzero residue $r$ is invertible modulo the [prime number](../../../../../../prime-number.md) $p$, so $p$ divides $\sum_{i\in I}a_i$. This sum has absolute value less than $p$, forcing it to be zero. The set $I$ is nonempty by its definition.

For sufficiency we first derive the needed [Brauer progression theorem](../../../../../../brauer-progression-theorem.md) from the permitted [Van der Waerden theorem](../../../../../../van-der-waerden-theorem.md). Fix [positive integers](../../../../../../positive-integer.md) $s,\ell$. We claim that for every number of colors $r$, a finite [integer interval](../../../../../../integer-interval.md) $[B(r,s,\ell)]$ forces a [monochromatic](../../../../../../monochromatic-set.md) set

$$
\{sd,\ a,a+d,\ldots,a+(\ell-1)d\},\qquad a,d>0.
$$

The case $\ell=1$ is immediate by taking $a=s$ and $d=1$. For $r=1$ and $\ell\geq2$, take $a=d=1$ in an interval of length at least $\max(s,\ell)$. Suppose the claim holds for $r-1$ and write $M=B(r-1,s,\ell)$. By the [Van der Waerden theorem](../../../../../../van-der-waerden-theorem.md), some $R$ forces an [arithmetic progression](../../../../../../arithmetic-progression.md) of length $(\ell-1)M+1$ in $[R]$ with one color $q$. Work in $[\max(R,sMR)]$ so that all needed multiples also lie in the coloring's domain. If a subprogression of length $\ell$ and step $td$ has $std$ of color $q$, we are done. Otherwise, for every $1\leq t\leq M$, the initial long [arithmetic progression](../../../../../../arithmetic-progression.md) contains such a subprogression, and $std$ avoids color $q$. The induced [finite coloring](../../../../../../finite-coloring.md) $t\mapsto\chi(sdt)$ of $[M]$ therefore uses at most $r-1$ colors. The induction hypothesis gives a [monochromatic](../../../../../../monochromatic-set.md) set $\{se,b,b+e,\ldots,b+(\ell-1)e\}$ for this induced [finite coloring](../../../../../../finite-coloring.md). Multiplying by $sd$ gives the desired configuration in the original coloring, with initial term $sdb$ and step $sde$. This proves the claim for $\ell\geq2$; the only use below has $\ell\geq3$.

Now suppose $\sum_{i\in I}a_i=0$ for a nonempty $I$. Choose $i_0\in I$, put $B=\sum_{i\notin I}a_i$, and put $s=|a_{i_0}|$. If $B=0$, then $\sum_i a_i=0$ and any constant positive vector is already a [monochromatic](../../../../../../monochromatic-set.md) solution. Otherwise take $L=|B|$ and apply the proved [Brauer progression theorem](../../../../../../brauer-progression-theorem.md) with $\ell=2L+1$. All of $sd$ and $a+jd$ for $0\leq j\leq2L$ have one color. Define

$$
x_i=\begin{cases}
sd,&i\notin I,\\
a+Ld,&i\in I\setminus\{i_0\},\\
a+\bigl(L-\operatorname{sgn}(a_{i_0})B\bigr)d,&i=i_0.
\end{cases}
$$

Every coordinate is a [positive integer](../../../../../../positive-integer.md) in that [monochromatic](../../../../../../monochromatic-set.md) set, since $L-\operatorname{sgn}(a_{i_0})B$ is either $0$ or $2L$. Using the zero sum on $I$ gives

$$
\sum_i a_i x_i=sBd-a_{i_0}\operatorname{sgn}(a_{i_0})Bd=0.
$$

Thus both directions are proved:

$$
\boxed{(a_1,\ldots,a_n)\text{ is partition regular}\iff
\exists\,\varnothing\ne I\subseteq[n]:\ \sum_{i\in I}a_i=0.}
$$

For $n=1$ the right side is impossible, agreeing with the absence of positive solutions for a single nonzero coefficient.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
