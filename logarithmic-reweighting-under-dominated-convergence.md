# Logarithmic reweighting under dominated convergence

↑ **Parent:** [Dominated convergence theorem](dominated-convergence-theorem.md)

Suppose $u$ and $\log(1+x)u$ are [Lebesgue integrable functions](lebesgue-integrable-function.md) on $(0,\infty)$. For integers $n\geq1$, $x+n\leq n(1+x)$ gives the displayed [L1 norm](l1-norm.md) bound. It tends to zero because $\log n/n\to0$, proving [L1 convergence](convergence-in-l1.md) of the logarithmically weighted [functions](function-split.md) to zero. Alternatively, $|\log(n+x)u(x)/n|\leq(1+\log(1+x))|u(x)|$ and pointwise convergence permit the [dominated convergence theorem](dominated-convergence-theorem.md).

For $u(x)=\sin x/x^q$ with $1<q<2$, both integrability conditions hold. Near zero, $|\sin x|\leq x$ and $\log(1+x)\leq x$ give integrable bounds by powers. At infinity, $|\sin x|\leq1$ and $\log(1+x)\leq\log2+\log x$, with $\int_1^\infty x^{-q}\log x\,dx=(q-1)^{-2}$. The [L1 norm](l1-norm.md) consequently decays as $O(\log n/n)$ in [Big O notation](big-o-notation.md).

## ↑ Ancestors (7)

1. [Dominated convergence theorem](dominated-convergence-theorem.md)
2. [Measure theory](measure-theory-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-integration-course-of-the-university-of-oxford/2015/2/c/solution.md)
