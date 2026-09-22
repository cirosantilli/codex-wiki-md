<h1 id="11g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $X\sim\operatorname{Bin}(n,t)$ and $Y\sim\operatorname{Bin}(n,s)$ be independent. The displayed [Bernstein polynomial](../../../../../../bernstein-polynomial.md) is

$$
B_nf(t,s)=\mathbb E f(X/n,Y/n).
$$

Given $\varepsilon>0$, [uniform continuity](../../../../../../uniform-continuity.md) of $f$ supplies $\delta>0$ such that changing both coordinates by less than $\delta$ changes $f$ by less than $\varepsilon$. If $M=\lVert f\rVert_\infty$, then [Chebyshev inequality](../../../../../../chebyshev-inequality.md) and  
$\operatorname{Var}(X/n),\operatorname{Var}(Y/n)\leq1/(4n)$ give, uniformly in $(t,s)$,

$$
|B_nf(t,s)-f(t,s)|
\leq\varepsilon+2M\,
\mathbb P\!\left(|X/n-t|\geq\delta
\ \hbox{or}\ |Y/n-s|\geq\delta\right)
\leq\varepsilon+\frac{M}{n\delta^2}.
$$

Thus $B_nf\to f$ uniformly.

Each $B_nf$ is a polynomial, whose iterated integrals may be interchanged term by term. Uniform convergence permits passage to the limit in both iterated integrals, proving the asserted continuous-function form of [Fubini's theorem](../../../../../../fubini-s-theorem.md).

Now suppose every monomial moment of $f$ vanishes. By linearity,  
$\int\!\!\int p f=0$ for every two-variable polynomial $p$. The just-proved Bernstein approximation gives polynomials $p_n\to f$ uniformly. Therefore

$$
\int_{[0,1]^2}f^2
=\lim_n\int_{[0,1]^2}f p_n=0,
$$

so $\boxed{f=0}$. Statement (i) is true.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11G](../../11g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
