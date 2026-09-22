# Dyadic conditional averages recover integrable functions

↑ **Parent:** [Conditional expectation](conditional-expectation.md)

For an integrable [function](function-split.md) on $[0,1]$, average $f$ on each [dyadic interval](dyadic-interval.md) of length $2^{-n}$. The resulting [step function](step-function.md) $f_n$ converges to $f$ [almost everywhere](almost-everywhere.md) and in the [L1 norm](l1-norm.md). If $U$ has the [uniform distribution](continuous-uniform-distribution.md) on $[0,1]$, then $f_n(U)=\mathbb E[f(U)\mid\sigma(b_n(U))]$, where $b_n$ rounds down to a dyadic endpoint. Refinement makes these [conditional expectations](conditional-expectation.md) a [uniformly integrable](uniform-integrability.md) [martingale](martingale-split.md). The [uniformly integrable martingale convergence theorem](uniformly-integrable-martingale-convergence-theorem.md) gives almost-sure and [convergence in L1](convergence-in-l1.md) to a limit $Y$.

Since $b_n(U)\to U$, the generated limiting [sigma-algebra](sigma-algebra.md) contains $U$ up to null sets. For every [event](event.md) $A$ in any finite-stage [sigma-algebra](sigma-algebra.md), convergence in the [L1 norm](l1-norm.md) gives $\mathbb E[Y\mathbf1_A]=\mathbb E[f(U)\mathbf1_A]$. The [pi-lambda theorem](pi-lambda-theorem.md) extends this equality to the limiting [sigma-algebra](sigma-algebra.md), identifying $Y=f(U)$. The [uniform distribution](continuous-uniform-distribution.md) of $U$ translates the two convergence conclusions into the assertions for $f_n$. Choosing a Borel representative of $f$ and assigning arbitrary values at the endpoint one makes all random variables well defined without changing either conclusion.

## ↑ Ancestors (7)

1. [Conditional expectation](conditional-expectation.md)
2. [Measure theory](measure-theory-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34/5/b/solution.md)
