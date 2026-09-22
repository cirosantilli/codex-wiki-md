# Necessity of the root condition for multistep convergence

↑ **Parent:** [Dahlquist equivalence theorem](dahlquist-equivalence-theorem.md)

For a [linear multistep method](linear-multistep-method.md), convergence for every set of consistent starting values requires the [root condition for a multistep method](root-condition-for-a-multistep-method.md). Apply the recurrence to $y'=0$ over $N$ steps. A root $\xi$ with $|\xi|>1$ gives the error mode $e_n=|\xi|^{-N}\xi^n$: its fixed-index starting errors vanish as $N\to\infty$, but $|e_N|=1$. A unit-modulus root of multiplicity $m\geq2$ instead gives $e_n=N^{-(m-1)}n^{m-1}\xi^n$, with the same failure. Repeated roots inside the unit disk are harmless because their polynomial growth is dominated by exponential decay.

## ↑ Ancestors (7)

1. [Dahlquist equivalence theorem](dahlquist-equivalence-theorem.md)
2. [Linear multistep method](linear-multistep-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/1/a/solution.md)
