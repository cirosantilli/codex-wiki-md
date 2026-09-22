<h1 id="11f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every summand is at most $2^{-r}$, and $\sum_{r\geq0}2^{-r}=2$, so $d(f,g)$ is finite and well defined. Nonnegativity and symmetry follow from the uniform norm. If $d(f,g)=0$, its $r=0$ summand gives $\|f-g\|_\infty=0$, hence $f=g$. Finally,

$$
\min\{1,a+b\}\leq\min\{1,a\}+\min\{1,b\}
$$

and the triangle inequality for each uniform norm give the triangle inequality for $d$. Thus $d$ is a metric.

Let $(f_n)$ be $d$-Cauchy. For fixed $r$ and $0<\varepsilon<1$, sufficiently large $m,n$ satisfy

$$
d(f_m,f_n)<2^{-r}\varepsilon,
$$

which forces $\|f_m^{(r)}-f_n^{(r)}\|_\infty<\varepsilon$. Hence, for every $r$, the continuous functions $f_n^{(r)}$ converge uniformly to some continuous $g_r$. The fundamental theorem of calculus gives

$$
f_n^{(r)}(x)-f_n^{(r)}(0)
=\int_0^x f_n^{(r+1)}(t)\,dt.
$$

Uniform convergence permits passage to the limit, yielding

$$
g_r(x)-g_r(0)=\int_0^xg_{r+1}(t)\,dt.
$$

Therefore $g_r'=g_{r+1}$ for every $r$, so $g_0\in C^\infty([0,1])$ and $g_0^{(r)}=g_r$.

To prove convergence in $d$, first choose $R$ so that $\sum_{r\geq R}2^{-r}$ is small, then use uniform convergence for the finitely many derivatives $r<R$. Thus $d(f_n,g_0)\to0$. This proves the [completeness of the smooth-function metric](../../../../../../completeness-of-the-smooth-function-metric.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
