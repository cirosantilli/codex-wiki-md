# Eigenvalue lower bound for total variation mixing

↑ **Parent:** [Mixing time of a Markov chain](mixing-time-of-a-markov-chain.md)

If $r=\max_{j\geq2}|\lambda_j|$ for a finite [irreducible Markov chain](irreducible-markov-chain.md) with at least two states, then its worst-case [total variation distance](total-variation-distance.md) from its [stationary distribution](stationary-distribution.md) satisfies $d(t)\geq r^t/2$. Choose a possibly complex [eigenfunction](eigenfunction.md) $f$ for an [eigenvalue](eigenvalue.md) of modulus $r$, normalize $\max_x|f(x)|=1$, and start where the maximum is attained. Since $\pi(f)=0$, $|P^tf(x)-\pi(f)|=r^t$; the defining sum for [total variation distance](total-variation-distance.md) bounds this difference by $2d(t)$. For $0<r<1$, this yields $t_{\mathrm{mix}}(\varepsilon)\geq(r/(1-r))\log(1/(2\varepsilon))$ for $0<\varepsilon<1/2$, because $-r\log r\leq1-r$.

## ↑ Ancestors (8)

1. [Mixing time of a Markov chain](mixing-time-of-a-markov-chain.md)
2. [Markov chain](markov-chain.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/2/d/solution.md)
- [Peres product condition](peres-product-condition.md)
