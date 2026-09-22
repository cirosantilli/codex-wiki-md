<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $v=t(1-t)$. The assertion is trivial when $v=0$. Otherwise suppose it fails and set $L=\log n$, $\lambda=vL$, $\gamma=3\log L/L$, $\delta=1-\gamma$, $p=2-\gamma$ and $b=L/3$, with natural logarithms. For large $n$ these parameters lie in their required ranges. The high-level [Fourier weight](../../../../../../fourier-weight.md) is

$$
\sum_{|S|\geq b}\alpha_S^2\leq\frac1b\sum_S|S|\alpha_S^2<\frac\lambda{4b}=\frac34v.
$$

For $1\leq s<b$, let $M_n=\max[s\delta^{s-1}]^{-1}$. The logarithm of this expression is a convex function of real $s$, so its maximum on $[1,b]$ is at an endpoint. Also $\delta^{1-b}/b\to3$, since $-(b-1)\log(1-\gamma)=\log L+o(1)$. Hence $M_n$ is bounded. The stronger inequality in part (ii) gives

$$
\sum_{1\leq|S|<b}\alpha_S^2\leq\frac{M_n}4(vL)^{2/p}n^{1-2/p}.
$$

Divide by $v$. Because $0<v\leq1/4$ and $2/p>1$, the factor $v^{2/p-1}$ is at most one. The remaining factor is $L^{2/p}e^{-\gamma L/p}=L^{-1/2+o(1)}\to0$. Thus the low-level weight is $o(v)$ uniformly in $t$. Adding both parts contradicts $\sum_{S\ne\varnothing}\alpha_S^2=v$ for sufficiently large $n$. This proves the [squared-influence logarithmic lower bound](../../../../../../squared-influence-logarithmic-lower-bound.md)

$$
\boxed{\sum_i\beta_i^2\geq\frac{t^2(1-t)^2(\log n)^2}{n}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
