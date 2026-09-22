<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

There is a minor range issue in the printed bound: **for $\varepsilon>1$ and positive $C$, the upper bound is below one.** We prove the intended result for $0<\varepsilon\leq1$; a valid formulation for every $\varepsilon>0$ replaces the upper bound by $\max\{1,\varepsilon^{-C}\}$. In fact the argument below gives $C=32$. All auxiliary estimates are proved here.

For $0<\varepsilon\leq1/2$, let $m=\lceil\varepsilon^{-2}\rceil$, and use the [Fejér kernel](../../../../../fejer-kernel.md)

$$
F_m(t)=\frac1m\left|\sum_{j=0}^{m-1}e(jt)\right|^2
=\sum_{|k|<m}\left(1-\frac{|k|}{m}\right)e(kt).
$$

Expanding the square proves the identity and nonnegativity. The [finite geometric series](../../../../../finite-geometric-series.md) formula and $|\sin\pi t|\geq2\|t\|$ give $F_m(t)\leq(4m\|t\|^2)^{-1}$ off the [integers](../../../../../integer.md). In particular $F_m(t)\leq1/4$ whenever $\|t\|\geq\varepsilon$.

Suppose, for a contradiction, that no $1\leq n\leq N$ has $\|\alpha n^2\|<\varepsilon$. Summing the [Fejér kernel](../../../../../fejer-kernel.md) along the quadratic sequence and separating its constant term gives

$$
\frac34N\leq\sum_{0<|k|<m}\left(1-\frac{|k|}{m}\right)|S_k|,
\qquad S_k=\sum_{n=1}^N e(k\alpha n^2).
$$

The coefficients on the right sum to $m-1$. Also $|S_{-k}|=|S_k|$. Hence some $1\leq k<m$ has $|S_k|\geq\eta N$, where $\eta=1/(2m)$.

We need only an elementary [Van der Corput inequality for finite scalar sequences](../../../../../van-der-corput-inequality-for-finite-scalar-sequences.md). For $|z_n|\leq1$, extended by zero outside $[N]$, each term of $S=\sum_nz_n$ occurs in exactly $H$ windows of length $H$. Applying the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) to the window sums and expanding their squares gives, for $H\leq N$,

$$
H^2|S|^2\leq(N+H)\left(HN+2\sum_{h=1}^{H-1}(H-h)|C_h|\right),
\qquad C_h=\sum_{n=1}^{N-h}z_{n+h}\overline{z_n}.
$$

Consequently $|S|^2\leq2N^2/H+(4N/H)\sum_{h=1}^{H-1}|C_h|$. Take $H=\lceil8\eta^{-2}\rceil$. If $|S|\geq\eta N$, some $1\leq h<H$ must have $|C_h|\geq\eta^2N/8$; otherwise the displayed upper bound is less than $3\eta^2N^2/4$.

For the large [quadratic exponential sum](../../../../../quadratic-exponential-sum.md) just found, put $z_n=e(k\alpha n^2)$. Its [quadratic exponential sum](../../../../../quadratic-exponential-sum.md) has multiplicative derivative

$$
z_{n+h}\overline{z_n}=e(k\alpha h^2)e(2kh\alpha n).
$$

Thus $C_h$ is a [finite geometric series](../../../../../finite-geometric-series.md). Its absolute value is at most $1/(2\|2kh\alpha\|)$, unless that distance is zero, in which case the desired estimate is automatic. It follows that

$$
\|2kh\alpha\|\leq\frac4{\eta^2N}.
$$

Set $n_*=2kh$. The [distance to the nearest integer](../../../../../distance-to-the-nearest-integer.md) satisfies $\|\ell x\|\leq\ell\|x\|$ for a positive integer $\ell$, by multiplying a nearest integer to $x$. Therefore

$$
1\leq n_*\leq2mH,
\qquad
\|\alpha n_*^2\|\leq\frac{8mH}{\eta^2N}.
$$

This proves the needed [quantitative quadratic recurrence](../../../../../quantitative-quadratic-recurrence.md) once $N$ is chosen polynomially in $\varepsilon^{-1}$.

For explicit bookkeeping, $m\leq2\varepsilon^{-2}$ and $H\leq33m^2$. Choose $N=\lfloor\varepsilon^{-32}\rfloor$. For $0<\varepsilon\leq1/2$ we have $N>33792\varepsilon^{-11}\geq8mH/(\eta^2\varepsilon)$ and $N\geq H$, while $2mH\leq528\varepsilon^{-6}\leq N$. Hence $n_*\leq N$ and $\|\alpha n_*^2\|<\varepsilon$, contradicting our supposition. The estimates have substantial slack even at $\varepsilon=1/2$.

For $1/2<\varepsilon\leq1$, simply take $n=1$, since $\|\alpha\|\leq1/2<\varepsilon$ and $1\leq\varepsilon^{-32}$. **For the intended range, the conclusion is**

$$
\boxed{\exists\,1\leq n\leq\varepsilon^{-32}\text{ with }\|\alpha n^2\|<\varepsilon.}
$$

For $\varepsilon>1$, the same choice $n=1$ proves the corrected all-range version.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 79](../../paper-79-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
