<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The partial sums $S_n$ are a [martingale](../../../../../../martingale-split.md), as are $S_n^2-n$. Since the increment has mean zero and nonzero variance, there are $\delta_+,\delta_->0$ with $\mathbb P(X_1\geq\delta_+)>0$ and $\mathbb P(X_1\leq-\delta_-)>0$. From any point in $(-a,b)$, a sufficiently long run of either kind exits the interval. Independence in consecutive blocks therefore bounds $\mathbb P(T>km)$ by a geometric sequence. In particular, $T<\infty$ almost surely and $\mathbb ET<\infty$.

Apply the [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) first to $T\wedge n$. Since the increments are bounded and $\mathbb ET<\infty$, the stopped variables are uniformly integrable and passage to the limit gives

$$
\mathbb E S_T=0.
$$

Applying the same argument to $S_n^2-n$, using $|S_T|\leq\max\{a,b\}+c$, gives

$$
\boxed{\mathbb E(S_T^2-T)=0,
\qquad
\mathbb E S_T^2=\mathbb ET.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
