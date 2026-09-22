<h1 id="a/1/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $U$ have the [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $(0,1)$, set $Y=1/U$, and take $X_n=Y/n$. The variable $Y$ is finite almost surely, so $X_n\to0$ almost surely. For any $\epsilon>0$ and all sufficiently large $n$,

$$
\mathbb P(|X_n|>\epsilon)=\mathbb P(U<1/(n\epsilon))=\frac1{n\epsilon}.
$$

The [harmonic series](../../../../../../harmonic-series.md) diverges, so

$$
\boxed{\sum_n\mathbb P(|X_n|>\epsilon)=\infty.}
$$

This dependent sequence fails [complete convergence](../../../../../../complete-convergence-of-random-variables.md). All its members are scalar multiples of the same nonconstant [random variable](../../../../../../random-variable-split.md), which explains why the independence hypothesis cannot be dropped.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
