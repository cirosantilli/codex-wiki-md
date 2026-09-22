# Integration of a series with summable L1 norms

↑ **Parent:** [Summable L1 norms imply almost-everywhere absolute convergence](summable-l1-norms-imply-almost-everywhere-absolute-convergence.md)

Suppose $\sum_n\|a_n\|_1<\infty$. By [summable L1 norms imply almost-everywhere absolute convergence](summable-l1-norms-imply-almost-everywhere-absolute-convergence.md), let $A=\sum_na_n$ where the series converges absolutely, and choose zero on the exceptional [null set](null-set.md). Then $A$ is a [Lebesgue measurable function](lebesgue-measurable-function.md) and $|A|\leq S=\sum_n|a_n|$ almost everywhere. Since $S$ is [Lebesgue integrable](lebesgue-integrable-function.md), so is $A$. The signed partial sums are bounded in absolute value by $S$, so the [dominated convergence theorem](dominated-convergence-theorem.md) proves termwise integration. It also gives the quantitative [L1 norm](l1-norm.md) estimate

$$
\left\|A-\sum_{n=1}^Na_n\right\|_1\leq\sum_{n>N}\|a_n\|_1\longrightarrow0.
$$

The numerical series of integrals is absolutely convergent because $|\int a_n|\leq\int|a_n|$.

For example, on $(0,1)$ take $a_n(x)=(-1)^n n\mathbf1_{(0,2^{-n})}(x)$. Its [L1 norm](l1-norm.md) is $n2^{-n}$, and these norms sum to two. Every positive $x$ lies in only finitely many supports, so the series is pointwise finite, although its terms are not uniformly small. Termwise integration gives $\int_0^1\sum_na_n=\sum_n(-1)^nn2^{-n}=-2/9$, by differentiating the [geometric series](geometric-series.md). This illustrates why a small [L1 norm](l1-norm.md) can permit tall terms on short intervals.

## ↑ Ancestors (9)

1. [Summable L1 norms imply almost-everywhere absolute convergence](summable-l1-norms-imply-almost-everywhere-absolute-convergence.md)
2. [L1 space](l1-space.md)
3. [Lp space](lp-space.md)
4. [Measure theory](measure-theory-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-integration-course-of-the-university-of-oxford/2014/1/b/solution.md)
- [Solution](past-exam-of-the-integration-course-of-the-university-of-oxford/2017/2/b/ii/b/solution.md)
- [Solution](past-exam-of-the-integration-course-of-the-university-of-oxford/2017/2/b/ii/c/solution.md)
- [Solution](past-exam-of-the-integration-course-of-the-university-of-oxford/2017/2/b/iii/solution.md)
