<h1 id="38e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $\hat u^n(\theta)=\sum_m u_m^ne^{-im\theta}$, initially for finite-support sequences and then by [Plancherel theorem](../../../../../../plancherel-theorem.md) for $\ell^2$. A shift by $k$ multiplies the transform by $e^{ik\theta}$. Hence the recurrence gives

$$
A(\theta)\hat u^{n+1}=B(\theta)\hat u^n,\qquad \boxed{\hat u^{n+1}=H(\theta)\hat u^n=H(\theta)^{n+1}\hat u^0.}
$$

Here the last equality is understood with time-zero data, and the scheme is assumed well-defined, so the denominator is nonzero or any removable singularity is filled continuously.

If $|H|\leq1$, Plancherel gives $\|u^n\|_2\leq\|u^0\|_2$ for every $n$. Conversely, if the continuous amplification factor has $|H(\theta_0)|>1$, it exceeds $1+\delta$ on an interval of positive length. Choose a nonzero initial Fourier transform supported in that interval. Then $\|u^n\|_2\geq(1+\delta)^n\|u^0\|_2$, contradicting a uniform stability bound. Therefore **uniform power stability holds exactly when**

$$
\boxed{|H(\theta)|\leq1\quad(-\pi\leq\theta\leq\pi).}
$$

Without continuity the exact condition is an essential-supremum bound, since isolated Fourier frequencies have zero measure. The fixed recurrence here uses a bound uniform over all time steps; mesh-dependent finite-time growth bounds are a different stability convention.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38E](../../38e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
