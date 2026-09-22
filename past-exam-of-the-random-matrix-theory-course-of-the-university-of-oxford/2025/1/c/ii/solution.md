<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $g_i=(X_{i1},\ldots,X_{in})$ be row $i$ of $X$, viewed as a real [vector](../../../../../vector.md). These are [independent](../../../../../independent-random-variables.md) standard [Gaussian](../../../../../normal-distribution.md) [random vectors](../../../../../random-vector.md), and $(XX^T)_{ij}=g_i\cdot g_j$. The [trace](../../../../../matrix-trace.md) expression for the [empirical spectral measure](../../../../../empirical-spectral-measure.md) gives

$$
\widetilde m_k(n)
=n^{-k-1}\sum_{i_1,\ldots,i_k}
(g_{i_1}\cdot g_{i_2})\cdots(g_{i_k}\cdot g_{i_1}).
$$

We need the norm [moments](../../../../../moment.md)

$$
\mathbb E\lVert g_i\rVert^2=n,\qquad
\mathbb E\lVert g_i\rVert^4=n(n+2),\qquad
\mathbb E\lVert g_i\rVert^6=n(n+2)(n+4).
$$

For completeness, $S=\lVert g_i\rVert^2$ has the [chi-squared distribution](../../../../../chi-squared-distribution.md) with $n$ degrees of freedom. By [independence](../../../../../independent-random-variables.md) and the [Gaussian integral](../../../../../gaussian-integral.md), its [moment-generating function](../../../../../moment-generating-function.md) is $\mathbb E e^{sS}=(1-2s)^{-n/2}$ for $s<1/2$. Differentiating at zero once, twice and three times proves these three identities.

For the first [moment](../../../../../moment.md),

$$
\boxed{\mathbb E[\widetilde m_1(n)]
=n^{-2}\sum_i\mathbb E\lVert g_i\rVert^2=1.}
$$

For the second [moment](../../../../../moment.md), if $i\ne j$, [conditional expectation](../../../../../conditional-expectation.md) given $g_i$ gives $\mathbb E[(g_i\cdot g_j)^2\mid g_i]=\lVert g_i\rVert^2$, hence an unconditional value $n$. Separating equal and unequal row indices yields

$$
\boxed{\mathbb E[\widetilde m_2(n)]
=n^{-3}\{n\,n(n+2)+n(n-1)n\}=2+\frac1n.}
$$

For the third [moment](../../../../../moment.md), the summand is $(g_i\cdot g_j)(g_j\cdot g_k)(g_k\cdot g_i)$. There are three disjoint cases.

- If $i,j,k$ are all different, average over $g_k$ first. Its [covariance matrix](../../../../../covariance-matrix.md) is the identity, so the [conditional expectation](../../../../../conditional-expectation.md) of the last two factors is $g_j\cdot g_i$. The summand's [expectation](../../../../../expected-value-split.md) is therefore $\mathbb E(g_i\cdot g_j)^2=n$. There are $n(n-1)(n-2)$ such triples.
- If exactly two indices agree, cyclic symmetry reduces the calculation to $i=j\ne k$. The product is $\lVert g_i\rVert^2(g_i\cdot g_k)^2$, whose [conditional expectation](../../../../../conditional-expectation.md) given $g_i$ is $\lVert g_i\rVert^4$. Its [expectation](../../../../../expected-value-split.md) is $n(n+2)$, and there are $3n(n-1)$ such triples.
- If all three indices agree, the product is $\lVert g_i\rVert^6$, with [expectation](../../../../../expected-value-split.md) $n(n+2)(n+4)$. There are $n$ choices.

Consequently

$$
\begin{aligned}
\mathbb E[\widetilde m_3(n)]
&=n^{-4}\{n^2(n-1)(n-2)
+3n^2(n-1)(n+2)+n^2(n+2)(n+4)\}\\
&=5+\frac6n+\frac4{n^2}.
\end{aligned}
$$

The three limiting [expected values](../../../../../expected-value-split.md) are therefore

$$
\boxed{\lim_{n\to\infty}\mathbb E[\widetilde m_k(n)]
=\begin{cases}1,&k=1,\\2,&k=2,\\5,&k=3.\end{cases}}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the random matrix theory course of the University of Oxford](../../../../split.md)
6. [Random matrix theory course of the University of Oxford](../../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
