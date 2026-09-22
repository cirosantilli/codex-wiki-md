<h1 id="positivity-of-the-limiting-polya-urn-proportion">Positivity of the limiting Pólya urn proportion</h1>

↑ **Parent:** [Pólya urn model](polya-urn-model.md)

Both colour counts tend to infinity almost surely. For example, $X_n\geq B_0/(m+n)$, and independent events $U_{n+1}\leq B_0/[2(n+1)]$ occur infinitely often by the [Borel-Cantelli second lemma](borel-cantelli-second-lemma.md), forcing infinitely many blue additions.

The martingale increment formula gives $\mathbb E[(X_{k+1}-X_k)^2\mid\mathcal F_k]\leq X_k/(m+k+1)^2$. Conditional orthogonality of later increments and $\mathbb E[X_k\mid\mathcal F_n]=X_n$ imply

$$
\mathbb E[(X_\infty-X_n)^2\mid\mathcal F_n]\leq X_n\sum_{j=m+n+1}^\infty j^{-2}\leq\frac{X_n}{m+n}.
$$

On $X_\infty=0$ the squared difference is $X_n^2$, so its conditional probability is at most $1/[(m+n)X_n]=1/B_n\to0$. Dominated convergence proves zero probability of that endpoint. The symmetric argument for red excludes $X_\infty=1$. No explicit beta law is needed for this proof.

## ↑ Ancestors (7)

1. [Pólya urn model](polya-urn-model.md)
2. [Stochastic process](stochastic-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2010/a/3/b/iii/solution.md)
