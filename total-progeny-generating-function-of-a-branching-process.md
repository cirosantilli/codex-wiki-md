# Total progeny generating function of a branching process

↑ **Parent:** [Total progeny of a branching process](total-progeny-of-a-branching-process.md)

For an almost surely finite [total progeny of a branching process](total-progeny-of-a-branching-process.md), let $F$ be the offspring [probability generating function](probability-generating-function.md) and $g$ that of the total, including one ancestor. Conditional on $k$ children, the total is one plus the sum of $k$ independent descendant totals. Independence and the [law of total expectation](law-of-total-expectation.md) give $g(s)=sF(g(s))$ for $|s|\leq1$, including the empty-product case $k=0$. If the offspring [expected value](expected-value-split.md) is $m=F'(1-)<1$, differentiation for $0<s<1$ gives $g'(s)=F(g(s))/(1-sF'(g(s)))$. The denominator is positive because $F'(g(s))\leq m$. Letting $s\uparrow1$ and using the [monotone convergence theorem](monotone-convergence-theorem.md) on the derivative series proves $\mathbb ET=1/(1-m)$, establishing finiteness rather than assuming it. For [Poisson branching process](poisson-branching-process.md) offspring, $F(z)=e^{m(z-1)}$.

## ↑ Ancestors (6)

1. [Total progeny of a branching process](total-progeny-of-a-branching-process.md)
2. [Galton-Watson process](galton-watson-process-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-options-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford/2013/n2/e/ii/solution.md)
