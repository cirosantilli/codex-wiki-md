<h1 id="11f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For rational $q\in(0,1)$ and positive integer $M$, define

$$
U_{q,M}=\bigcup_{m\geq M}
\left\{f\in C^\infty([0,1]):|f^{(m)}(q)|>m!m^m\right\}.
$$

Evaluation of the $m$th derivative at $q$ is continuous in the smooth-function metric, so $U_{q,M}$ is open.

It is also dense. Given $f$ and a metric tolerance $\varepsilon>0$, choose $R\geq1$ so that the contribution of all derivatives of order at least $R$ is below $\varepsilon/2$, and choose $m\geq\max\{M,R\}$. For large $K$, perturb $f$ by

$$
h_K(x)=\delta_K\cos\left(K(x-q)-\frac{m\pi}{2}\right),
\qquad
\delta_K=\frac{\varepsilon}{4R K^{R-1}}.
$$

For every $r<R$, $\|h_K^{(r)}\|_\infty\leq\varepsilon/(4R)$, so $d(f+h_K,f)<\varepsilon$. On the other hand,

$$
h_K^{(m)}(q)=\delta_KK^m
=\frac{\varepsilon}{4R}K^{m-R+1}\longrightarrow\infty.
$$

For sufficiently large $K$, $|f^{(m)}(q)+h_K^{(m)}(q)|>m!m^m$, proving density.

The space is complete by part (b). The [Baire category theorem](../../../../../../baire-category-theorem.md) therefore makes

$$
G=\bigcap_{q\in\mathbb Q\cap(0,1)}
\bigcap_{M=1}^\infty U_{q,M}
$$

dense. Put $E=C^\infty([0,1])\setminus G$. Each complement $U_{q,M}^c$ is closed and nowhere dense, so $E$ is a [meagre set](../../../../../../meagre-set.md), or a set of first category. Every $f\notin E$ has the required derivative growth. This is the [generic superfactorial derivative growth at rational points](../../../../../../generic-superfactorial-derivative-growth-at-rational-points.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
