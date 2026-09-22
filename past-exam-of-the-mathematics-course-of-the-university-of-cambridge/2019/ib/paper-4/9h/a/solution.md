<h1 id="9h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $R$ be the number of returns to $v$ after time $0$. Since $v$ is a [recurrent state](../../../../../../recurrent-state.md), the probability of another return after each visit is one. By the stated [geometric distribution](../../../../../../geometric-distribution.md) description, $\mathbb P_v(R\geq k)=1$ for every positive integer $k$. Thus $R=\infty$ almost surely and $\mathbb E_vR=\infty$.

On the other hand, writing each visit as an [indicator random variable](../../../../../../indicator-random-variable.md) and applying the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) to the partial sums gives

$$
1+\mathbb E_vR
=\mathbb E_v\left[\sum_{n=0}^{\infty}\boldsymbol1_{\{X_n=v\}}\right]
=\sum_{n=0}^{\infty}\mathbb P_v(X_n=v)
=\sum_{n=0}^{\infty}p_{vv}(n).
$$

The left side is infinite, proving the [recurrence criterion by return probabilities](../../../../../../recurrence-criterion-by-return-probabilities.md) in the required direction:

$$
\boxed{\sum_{n=0}^{\infty}p_{vv}(n)=\infty}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9H](../../9h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
