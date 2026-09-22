# Clark-Ocone formula for a smooth Brownian terminal payoff

↑ **Parent:** [Brownian martingale representation theorem](brownian-martingale-representation-theorem.md)

In the completed natural [Brownian filtration](brownian-filtration.md), a bounded continuously differentiable $\phi$ with bounded derivative satisfies

$$
\phi(W_T)=\mathbb E\phi(W_T)+\int_0^T\mathbb E[\phi'(W_T)\mid\mathcal F_t]\,dW_t.
$$

The integrand is unique up to $d\mathbb P\,dt$-almost everywhere equality. [Gaussian integration by parts](stein-s-lemma-probability.md) first gives the duality between the payoff and every square-integrable [Itô integral](ito-integral.md). The [Brownian martingale representation theorem](brownian-martingale-representation-theorem.md) then identifies the integrand as the projection of $\phi'(W_T)\mathbf1_{\{t\le T\}}$ onto the [predictable processes](predictable-process.md) in the product $L^2$ space. This explains the [conditional expectation](conditional-expectation.md) in the formula, rather than a nonadapted terminal derivative.

## ↑ Ancestors (9)

1. [Brownian martingale representation theorem](brownian-martingale-representation-theorem.md)
2. [Martingale representation theorem](martingale-representation-theorem.md)
3. [Brownian motion](brownian-motion-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-25/2/e/solution.md)
