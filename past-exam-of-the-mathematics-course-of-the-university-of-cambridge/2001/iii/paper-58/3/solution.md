<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Korovkin theorem](../../../../../korovkin-theorem.md) says that a sequence of [positive linear operators on continuous functions](../../../../../positive-linear-operator-on-continuous-functions.md) on $[0,1]$ converges uniformly to the identity on every [continuous function](../../../../../continuous-function.md) if it does so on $1$, $x$ and $x^2$. Necessity is immediate; the quadratic barrier argument establishing sufficiency is given in Solution 6.

There is an endpoint misprint in the original PDF: the repeated knots at the right end must equal $1$, not $0$. Otherwise the advertised nondecreasing [spline knot sequence](../../../../../spline-knot-sequence.md) on $[0,1]$ does not exist. Use the corrected clamped [spline knot sequences](../../../../../spline-knot-sequence.md), with fixed order $k$ and maximum gap $h_n\to0$. Let $m_n$ denote the number of [B-splines](../../../../../b-spline.md) for the $n$th sequence. Nonnegativity and partition of unity show that the [Schoenberg spline operator](../../../../../schoenberg-spline-operator.md) $V_n$ is positive and $V_n1=1$.

The [monomial B-spline coefficients](../../../../../monomial-b-spline-coefficients.md) reproduce the first two nonconstant test [polynomials](../../../../../polynomial-split.md). Put

$$
a_{1,j}=\frac1{k-1}\sum_{r=j+1}^{j+k-1}t_r,\qquad
a_{2,j}=\binom{k-1}{2}^{-1}\sum_{j+1\le r<s\le j+k-1}t_rt_s.
$$

The pair sum uses $r<s$, as in the PDF; the converted TeX incorrectly includes $r=s$. Every sampling point $\tau_j$ and every knot entering these [coefficients](../../../../../coefficient.md) lie in $[t_j,t_{j+k}]$, whose length is at most $kh_n$. Thus $|\tau_j-a_{1,j}|\le kh_n$. Also all these numbers belong to $[0,1]$, so

$$
|\tau_j^2-t_rt_s|\le|\tau_j(\tau_j-t_r)|+|t_r(\tau_j-t_s)|\le2kh_n,
\qquad |\tau_j^2-a_{2,j}|\le2kh_n.
$$

The positive [B-spline](../../../../../b-spline.md) weights give

$$
\|V_nx-x\|_\infty\le kh_n,\qquad\|V_nx^2-x^2\|_\infty\le2kh_n.
$$

Together with $V_n1=1$, the three limits prove

$$
\boxed{\|V_ng-g\|_\infty\longrightarrow0\quad\text{for every }g\in C[0,1].}
$$

Under the usual interior knot multiplicities at most $k-1$, the [splines](../../../../../spline-mathematics.md) are continuous and the quoted form of the [Korovkin theorem](../../../../../korovkin-theorem.md) applies directly. If full interior multiplicity is allowed, the output can be discontinuous. The same positive-operator quadratic barrier proof still works with bounded output [functions](../../../../../function-split.md) and the [supremum norm](../../../../../supremum-norm.md), and proves exactly the stated uniform error limit without asserting continuity of each output. Indeed the stronger [local-support error bound for a Schoenberg spline operator](../../../../../local-support-error-bound-for-a-schoenberg-spline-operator.md), $\|V_ng-g\|_\infty\le\omega(g,kh_n)$, follows by comparing $g(x)$ with each active sample value. The restriction $k\ge3$ is needed for the displayed quadratic reproduction argument, not for this direct support estimate.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
