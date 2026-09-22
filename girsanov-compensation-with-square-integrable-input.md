# Girsanov compensation with square-integrable input

↑ **Parent:** [Girsanov theorem](girsanov-theorem.md)

Let $Z=\exp(X-\langle X\rangle/2)$ and $dQ=Z_TdP$. The [Girsanov theorem](girsanov-theorem.md) first makes $N=M-\langle M,X\rangle$ a continuous local Q-martingale. Boundedness of $Y$ gives $\langle X\rangle_T\leq C^2T$ and $\mathbb E_PZ_T^2\leq e^{C^2T}$: write $Z_T^2=\mathcal E(2X)_T e^{\langle X\rangle_T}$ and apply [Novikov's condition](novikov-s-condition.md) to $2X$.

The [quadratic covariation](quadratic-covariation.md) bound gives $\sup_{s\leq T}|\langle M,X\rangle_s|\leq C\sqrt T\langle M\rangle_T^{1/2}$. For a square-integrable [martingale](martingale-split.md) $M$, both its maximal square moment and its expected terminal bracket are finite. [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) with the density $Z_T$ therefore yields $\mathbb E_Q\sup_{s\leq T}|N_s|<\infty$. The dominated limit of its stopped conditional identities proves the true martingale property. Mere P-integrability of $M_T$ does not suffice.

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

## ← Incoming links (2)

- [Bounded Girsanov drift does not preserve true martingales under compensation](bounded-girsanov-drift-does-not-preserve-true-martingales-under-compensation.md)
- [Solution](past-exam-of-the-stochastic-differential-equations-course-of-the-university-of-oxford/2011/3/d/solution.md)
