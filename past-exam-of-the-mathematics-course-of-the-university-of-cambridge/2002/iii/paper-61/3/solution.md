<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The original PDF prints $O(n^\alpha)$, with a positive exponent. **That premise is insufficient; the intended decay rate is $O(n^{-\alpha})$.** Indeed every bounded continuous periodic function has $E_n(f)\le\|f\|_\infty=O(n^\alpha)$. For an explicit counterexample, on $[-\pi,\pi]$ set

$$
h(0)=0,\qquad h(x)=\frac1{\log(e/|x|)}\ (0<|x|\le1),\qquad h(x)=1\ (1\le|x|\le\pi),
$$

and extend periodically. This is continuous, but $\omega(h,\delta)\ge1/\log(e/\delta)$ for $0<\delta<1$, which is not $O(\delta^\alpha)$ for any $\alpha>0$. Thus the sign correction is required in the actual printed question, not just in its converted TeX.

For real continuous $2\pi$-periodic $f$, write $E_n$ for best [uniform approximation](../../../../../uniform-approximation-split.md) by degree-at-most-$n$ [trigonometric polynomials](../../../../../trigonometric-polynomial.md) and $\omega(f,\delta)=\sup_{|h|\le\delta}\|f(\cdot+h)-f\|_\infty$. A quantitative [inverse theorem for trigonometric approximation](../../../../../inverse-theorem-for-trigonometric-approximation.md) is

$$
\boxed{\omega(f,1/n)\le\frac Cn\sum_{\nu=0}^nE_\nu(f),\qquad n\ge1,}
$$

where $C$ is universal. Here is a direct reason for the sum. Choose best approximants $p_j$ and $2^r\le n<2^{r+1}$. Write

$$
p_{2^r}=p_0+(p_1-p_0)+\sum_{j=1}^r(p_{2^j}-p_{2^{j-1}}).
$$

The [Bernstein inequality for trigonometric polynomials](../../../../../bernstein-inequality-for-trigonometric-polynomials.md) gives

$$
\|p_{2^r}'\|_\infty\le2E_0+\sum_{j=1}^r2^{j+1}E_{2^{j-1}}.
$$

For $j\ge2$, monotonicity of best errors bounds $2^{j+1}E_{2^{j-1}}$ by $8\sum_{\nu=2^{j-2}}^{2^{j-1}-1}E_\nu$. The first terms are bounded by a fixed multiple of $E_0$. Also $2E_{2^r}\le4n^{-1}\sum_{\nu=0}^nE_\nu$. Now

$$
\omega(f,1/n)\le2E_{2^r}+\frac1n\|p_{2^r}'\|_\infty
$$

proves the theorem, for example with a sufficiently large absolute constant $C=20$.

Suppose, as intended, $E_\nu(f)\le A\nu^{-\alpha}$ for $\nu\ge1$, after enlarging $A$ to include any finite exceptional indices, where $0<\alpha<1$. Since $\sum_{\nu=1}^n\nu^{-\alpha}\le n^{1-\alpha}/(1-\alpha)$, the inverse theorem gives

$$
\omega(f,1/n)\le C\left(E_0/n+\frac{A}{1-\alpha}n^{-\alpha}\right)\le C_f n^{-\alpha}.
$$

For $0<\delta\le1$ take $n=\lfloor1/\delta\rfloor$. Then $1/(n+1)<\delta\le1/n$, so monotonicity of the [modulus of continuity](../../../../../modulus-of-continuity.md) and $n^{-\alpha}\le2^\alpha\delta^\alpha$ give $\omega(f,\delta)\le2^\alpha C_f\delta^\alpha$. For $\delta>1$, the separate bound $\omega(f,\delta)\le2\|f\|_\infty\le2\|f\|_\infty\delta^\alpha$ covers the remaining scales. Therefore the corrected conclusion is

$$
\boxed{E_n(f)=O(n^{-\alpha})\Longrightarrow\omega(f,\delta)=O(\delta^\alpha),\quad0<\alpha<1.}
$$

Now put $\beta=\log2/\log3$. The given best approximant to the [Weierstrass function](../../../../../weierstrass-function.md) leaves the uniformly convergent tail $\sum_{k=m+1}^\infty2^{-k}\cos(3^kx)$. Its [supremum norm](../../../../../supremum-norm.md) is exactly $2^{-m}$, attained at $x=0$; hence

$$
E_n(g)=2^{-m}\quad(3^m\le n<3^{m+1}),\qquad E_n(g)\asymp n^{-\beta}.
$$

The corrected inverse theorem gives $\omega(g,\delta)=O(\delta^\beta)$. To show that this order is sharp, set $h_m=\pi/3^{m+1}$. Every term of $g(0)-g(h_m)$ is nonnegative, and for $k\ge m+1$ the cosine equals $-1$ because $3^{k-m-1}$ is odd. Thus

$$
g(0)-g(h_m)\ge2\sum_{k=m+1}^\infty2^{-k}=2^{1-m}=4\pi^{-\beta}h_m^\beta.
$$

Given small $\delta>0$, select $m$ with $h_m\le\delta<3h_m$. Then $\omega(g,\delta)\ge4(3\pi)^{-\beta}\delta^\beta$. Combining the estimates gives the precise small-scale order

$$
\boxed{\omega(g,\delta)\asymp\delta^{\log2/\log3}\qquad(\delta\downarrow0).}
$$

The exact approximation error can also be verified independently of the supplied fact: at $x_j=j\pi/3^{m+1}$ the tail has alternating values $(-1)^j2^{-m}$. There are enough such points in one period for the [trigonometric Chebyshev alternation theorem](../../../../../trigonometric-chebyshev-alternation-theorem.md), since $n<3^{m+1}$. This is the [positive lacunary trigonometric series](../../../../../positive-lacunary-trigonometric-series.md) mechanism behind the best partial sums.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
