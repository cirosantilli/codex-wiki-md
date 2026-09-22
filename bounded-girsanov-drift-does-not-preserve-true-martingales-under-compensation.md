# Bounded Girsanov drift does not preserve true martingales under compensation

↑ **Parent:** [Girsanov theorem](girsanov-theorem.md)

Let $W$ be a P-Brownian motion on $[0,1]$ and tilt by the bounded constant drift integrand one, so $dQ=e^{W_1-1/2}dP$. Then $W_s^Q=W_s-s$ is Q-Brownian motion, either by [Girsanov theorem](girsanov-theorem.md) or direct Gaussian exponential tilting. Set $a=1/2$,

$$
H=\frac{e^{W_a^2}}{1+W_a^2},\qquad M_s=H(W_s-W_a)\mathbf1_{\{s>a\}}.
$$

The density of $W_a$ under P is $\pi^{-1/2}e^{-x^2}$, so $\mathbb E_PH=\pi^{-1/2}\int(1+x^2)^{-1}dx<\infty$. Independence of future Brownian increments makes $M$ a continuous true P-martingale. Under Q, that density is multiplied by $e^{x-1/4}$, so $\mathbb E_QH=\infty$.

For $s>a$, its compensated local martingale is

$$
M_s-\langle M,W\rangle_s=H(W_s^Q-W_a^Q).
$$

The future Q-Brownian increment is independent of the positive variable $H$ and has positive finite mean absolute value. Hence the displayed variable has infinite expected absolute value under Q and is not a true martingale. This shows why the general [Girsanov theorem](girsanov-theorem.md) promises a local martingale, while a true-martingale conclusion needs an additional integrability condition such as [Girsanov compensation with square-integrable input](girsanov-compensation-with-square-integrable-input.md).

## ↑ Ancestors (9)

1. [Girsanov theorem](girsanov-theorem.md)
2. [Doléans-Dade exponential](doleans-dade-exponential.md)
3. [Stochastic calculus](stochastic-calculus-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-stochastic-differential-equations-course-of-the-university-of-oxford/2011/3/d/solution.md)
