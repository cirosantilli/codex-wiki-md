<h1 id="algebra/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Every $g_i\in U^0$ vanishes on $U$, so $U\subseteq\bigcap_i\ker g_i$. Conversely, suppose $v\in\bigcap_i\ker g_i$. Every $f\in U^0$ is a [linear combination](../../../../../linear-combination.md) $\sum_i a_ig_i$, giving $f(v)=0$. If $v\notin U$, part (b) supplies a functional in $U^0$ with $f(v)\neq0$, a contradiction. Therefore

$$
\boxed{U=\bigcap_{i=1}^k\ker g_i.}
$$

For the dimension statement, take a [basis](../../../../../basis.md) $u_1,\ldots,u_m$ of $U$ and extend it to a [basis](../../../../../basis.md) $u_1,\ldots,u_n$ of $V$. Relative to the corresponding [dual basis](../../../../../dual-basis.md), a functional belongs to $U^0$ precisely when its first $m$ coefficients are zero. Thus

$$
\boxed{k=\dim U^0=n-m=\dim V-\dim U.}
$$

If $U=V$, this says $k=0$ and the empty intersection is understood to be $V$.

In the coordinate example choose the [linear functionals](../../../../../linear-functional.md) $g_1(x,y,z)=y$ and $g_2(x,y,z)=z$. Their [kernels](../../../../../kernel-of-a-linear-map-split.md) are the two coordinate planes

$$
\boxed{W_1=\{(x,0,z):x,z\in\mathbb R\},\qquad
W_2=\{(x,y,0):x,y\in\mathbb R\}.}
$$

Their intersection is the stated axis, and $k=2=3-1$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Algebra](../../../algebra.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
