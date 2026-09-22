# Weighted binary counter cost

↑ **Parent:** [Amortized analysis](amortized-analysis.md)

For an initially zero $k$-bit [binary counter](binary-counter.md), suppose changing [bit](bit.md) $i$ costs $2^i$. It changes exactly $\lfloor n/2^i\rfloor$ times in $n$ increments. Consequently the total is $\Theta(n\min\{k,1+\log_2 n\})$ for $n,k\geq1$. The upper bound counts at most $n$ cost at each active position; the lower bound uses $\lfloor x\rfloor\geq x/2$ for $x\geq1$. This shows why exponential position costs cancel the decreasing carry frequencies that make the ordinary [binary counter](binary-counter.md) have constant [amortized cost](amortized-cost.md).

## ↑ Ancestors (7)

1. [Amortized analysis](amortized-analysis.md)
2. [Time complexity](time-complexity.md)
3. [Complexity class](complexity-class.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)
