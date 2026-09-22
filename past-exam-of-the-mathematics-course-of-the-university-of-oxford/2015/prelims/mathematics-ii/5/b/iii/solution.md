<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For real-valued [functions](../../../../../../../function-split.md), the [Uniform Cauchy criterion](../../../../../../../uniform-cauchy-criterion.md) applied to [partial sums](../../../../../../../partial-sum.md) says that $\sum u_n$ has [uniform convergence](../../../../../../../uniform-convergence.md) exactly when

$$
\forall\varepsilon>0\ \exists N\ \forall q>p\geq N\ \forall x\in E:\quad\left|\sum_{n=p+1}^q u_n(x)\right|<\varepsilon.
$$

Sufficiency uses [completeness of the real numbers](../../../../../../../completeness-of-the-real-numbers.md).

Let $M$ be a common bound for the [uniformly bounded family of functions](../../../../../../../uniformly-bounded-family-of-functions.md) $(g_n)$; increase it if necessary so that $M>0$. The assumed [uniform absolute convergence](../../../../../../../uniform-absolute-convergence.md) of $\sum f_n$ gives $N$ such that

$$
\sum_{n=p+1}^q|f_n(x)|<\frac{\varepsilon}{M+1}
\qquad(q>p\geq N,\ x\in E).
$$

The [triangle inequality](../../../../../../../triangle-inequality.md) now yields

$$
\boxed{\left|\sum_{n=p+1}^q f_n(x)g_n(x)\right|\leq M\sum_{n=p+1}^q|f_n(x)|<\varepsilon.}
$$

The [Uniform Cauchy criterion](../../../../../../../uniform-cauchy-criterion.md) therefore proves **[uniform convergence](../../../../../../../uniform-convergence.md) of $\sum f_ng_n$.** The same estimate with $|f_ng_n|$ proves [uniform absolute convergence](../../../../../../../uniform-absolute-convergence.md) as well.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
