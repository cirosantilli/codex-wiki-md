<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First take the usual endpoint-regular interpretation $f\in C([-1,1])$. Integrating the divergence form shows that $F=(1-x^2)y'$ has finite endpoint limits. A nonzero limit would make $y'$ proportional to $1/(1\mp x)$ near that endpoint, forcing a logarithmically unbounded $y$. Thus boundedness requires $F(-1)=F(1)=0$, and consequently

$$
\boxed{\int_{-1}^1f(x)\,dx=0}.
$$

This is [orthogonality](../../../../../orthogonal-vectors.md) to the constant [eigenfunction](../../../../../eigenfunction.md) $P_0$, hence the [Fredholm alternative](../../../../../fredholm-alternative.md) condition. It is also sufficient under the stated endpoint regularity: put

$$
F(x)=\int_{-1}^xf(t)\,dt,\qquad
y(x)=C+\int_0^x\frac{F(s)}{1-s^2}\,ds.
$$

If $M=\max|f|$, the zero-mean condition gives $|F(s)|\leq M\min(1+s,1-s)$. Hence the last integrand is bounded, so $y$ extends continuously to both endpoints. Any two bounded solutions differ by a constant: their difference solves $((1-x^2)z')'=0$, whose other solution is $\tfrac12\log((1+x)/(1-x))$.

For the requested [eigenfunction expansion](../../../../../eigenfunction-expansion.md), set

$$
N_k=\int_{-1}^1P_k(t)^2\,dt,\qquad
f_k=\frac{\int_{-1}^1f(t)P_k(t)\,dt}{N_k}.
$$

The [Legendre polynomials](../../../../../legendre-polynomial.md) span all [polynomials](../../../../../polynomial-split.md), so their completeness follows from the [Weierstrass approximation theorem](../../../../../weierstrass-approximation-theorem.md). Projecting $\mathcal Ly=f$ onto each [eigenfunction](../../../../../eigenfunction.md) gives $-k(k+1)y_k=f_k$ for $k\geq1$. The zero mode is free, while $f_0=0$. Thus the full family is

$$
\boxed{y(x)=C-\sum_{k=1}^\infty
\frac{P_k(x)}{k(k+1)}
\frac{\int_{-1}^1f(t)P_k(t)\,dt}{\int_{-1}^1P_k(t)^2\,dt},\qquad C\in\mathbb R}.
$$

The formula is unchanged by rescaling any $P_k$. For the usual normalization $P_k(1)=1$, the facts $|P_k(x)|\leq1$ on $[-1,1]$ and $N_k=2/(2k+1)$, together with the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), bound each summand by a constant times $k^{-3/2}$. The series therefore converges absolutely and uniformly. Its identification with the preceding integral solution avoids unjustified termwise second [differentiation](../../../../../differentiation.md).

There is a source ambiguity: continuity only on $(-1,1)$ does not supply the endpoint control used above. Even for integrable forcing, zero mean alone is insufficient. For example, let

$$
H(x)=\log\frac{e}{1-x^2},\qquad
F(x)=\frac1{H(x)},\qquad
f(x)=F'(x)=\frac{-2x}{(1-x^2)H(x)^2}.
$$

This $f$ is continuous in the interior, absolutely integrable, and has zero mean because $F(\pm1)=0$. Yet every candidate with zero endpoint values of $(1-x^2)y'$ has

$$
y'(x)=\frac1{(1-x^2)H(x)},
$$

whose [integral](../../../../../integral-split.md) diverges logarithmically in $H$ at each endpoint. Thus no bounded solution exists. For a merely interior-continuous $f$, the exact criterion is that some constant $B$ makes

$$
\int_0^x\frac{B+\int_0^sf(t)\,dt}{1-s^2}\,ds
$$

bounded as $x$ approaches both endpoints. The [Bounded solvability for the Legendre operator](../../../../../bounded-solvability-for-the-legendre-operator.md) criterion above covers the intended regular forcing and makes this endpoint limitation explicit.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
