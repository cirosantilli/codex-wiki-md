<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The set $\widetilde P$ contains zero. It is closed under negatives because $-f\in P$ whenever $f\in P$. If $f,g\in P$ and $n,m>0$, then

$$
\frac fn+\frac gm=\frac{mf+ng}{nm}\in\widetilde P,
$$

since $P$ is an [ideal](../../../../ideal.md) of $\mathbb Z[t]$. Also, any $q\in\mathbb Q[t]$ can be written $q=h/d$ with $h\in\mathbb Z[t]$ and $d>0$, giving

$$
q\frac fn=\frac{hf}{dn}\in\widetilde P.
$$

This proves that $\widetilde P$ is an [ideal](../../../../ideal.md) of $\mathbb Q[t]$.

Clearly $P\subseteq\widetilde P\cap\mathbb Z[t]$, by taking denominator one. Conversely, if $h\in\widetilde P\cap\mathbb Z[t]$, then $nh\in P$ for some positive [integer](../../../../integer-split.md) $n$. The condition $P\cap\mathbb Z=\{0\}$ implies $n\notin P$. Since $P$ is a [prime ideal](../../../../prime-ideal.md), $nh\in P$ forces $h\in P$. Hence

$$
\boxed{\widetilde P\cap\mathbb Z[t]=P.}
$$

In particular, $\widetilde P$ is nonzero because it contains the nonzero [ideal](../../../../ideal.md) $P$, and it is proper: otherwise its intersection with $\mathbb Z[t]$ would contain $1$. This is the concrete [extension of an ideal](../../../../extension-of-an-ideal.md) and [contraction of an ideal](../../../../contraction-of-an-ideal.md) calculation for the [localization](../../../../localization-of-a-ring.md) that inverts nonzero [integers](../../../../integer-split.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the algebra 2 course of the University of Oxford](../../../split.md)
5. [Algebra 2 course of the University of Oxford](../../../../algebra-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
