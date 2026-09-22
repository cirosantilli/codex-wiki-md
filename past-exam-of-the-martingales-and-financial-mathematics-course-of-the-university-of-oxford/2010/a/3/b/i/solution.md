<h1 id="a/3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The printed update needs a one-step index correction to match its filtration: the draw for the transition from $n$ to $n+1$ must be the fresh variable $U_{n+1}$. Also the trivial initial sigma-algebra is $\{\varnothing,\Omega\}$, rather than the printed $\{\varnothing,\mathcal F\}$. With literal $U_n$, the next increment is already known at time $n$, so $\mathbb E[X_{n+1}\mid\mathcal F_n]=X_{n+1}$; the nontrivial update differs from $X_n$. Thus the stated martingale claim is false with that indexing. The following uses the standard [Pólya urn](../../../../../../polya-urn-model.md) described in words.

Put $m=B_0+R_0$, so the total count is $m+n$. Conditional on $\mathcal F_n$, the next blue indicator $I_{n+1}$ has expectation $X_n$. Hence

$$
\mathbb E[X_{n+1}\mid\mathcal F_n]
=\frac{B_n+\mathbb E[I_{n+1}\mid\mathcal F_n]}{m+n+1}
=\frac{B_n+B_n/(m+n)}{m+n+1}=X_n.
$$

Adaptedness and integrability follow from the recursive construction and $0\leq X_n\leq1$. Thus $X_n$ is a bounded [martingale](../../../../../../martingale-split.md). The [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) gives an almost-sure limit $X_\infty\in[0,1]$. Boundedness and the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) then give $\mathbb E|X_n-X_\infty|^2\to0$, establishing convergence in $L^2$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
