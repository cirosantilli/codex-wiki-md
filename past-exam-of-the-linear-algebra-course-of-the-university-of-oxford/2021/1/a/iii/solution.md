<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [iii](../iii.md)

Write $K_j=\ker T^j$, where $T^0=I$ and $K_0=\{0\}$. These [kernels](../../../../../kernel-of-a-linear-map-split.md) satisfy $K_j\subseteq K_{j+1}$. Also $T(K_{i+1})\subseteq K_i$ and $T(K_i)\subseteq K_{i-1}$: for example, $T^i(Tv)=T^{i+1}v=0$ when $v\in K_{i+1}$. Thus the proposed [linear map](../../../../../linear-map.md) between [quotient vector spaces](../../../../../quotient-vector-space.md) is well-defined and has the formula

$$
\overline T:K_{i+1}/K_i\longrightarrow K_i/K_{i-1},\qquad
v+K_i\longmapsto Tv+K_{i-1}.
$$

If $v+K_i$ belongs to its [kernel](../../../../../kernel-of-a-linear-map-split.md), then $Tv\in K_{i-1}$. Therefore $T^iv=T^{i-1}(Tv)=0$, so $v\in K_i$ and $v+K_i$ is zero. We have proved

$$
\boxed{\overline T\text{ is injective for every }i\geq1.}
$$

These are the [injections between successive kernel quotients](../../../../../injections-between-successive-kernel-quotients.md). In finite [dimension](../../../../../dimension-vector-space.md), they imply $\dim K_{i+1}-\dim K_i\leq\dim K_i-\dim K_{i-1}$.

**Surjectivity need not hold.** Take a nonzero [vector space](../../../../../vector-space-split.md) $V$ and the zero [linear map](../../../../../linear-map.md) $T=0$. At $i=1$, we have $K_2=K_1=V$ and $K_0=0$, so

$$
\boxed{\overline T:V/V\longrightarrow V/0\text{ is the map }0\longrightarrow V,\text{ which is not surjective}.}
$$

## ↑ Ancestors (13)

1. [iii](../iii.md)
2. [a](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
