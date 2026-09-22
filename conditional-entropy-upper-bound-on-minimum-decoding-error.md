# Conditional entropy upper bound on minimum decoding error

↑ **Parent:** [Maximum a posteriori decoding](maximum-a-posteriori-decoding.md)

For finite random variables $X,Y$, let $P_e$ be the error probability of [maximum a posteriori decoding](maximum-a-posteriori-decoding.md) of $X$ from $Y$. Then $P_e\leq H(X\mid Y)/2$ when [conditional entropy](conditional-entropy.md) is measured in bits. At each positive-probability output $y$, the optimum success probability is the largest posterior atom $\Pi_y$, so its conditional error is $1-\Pi_y$. Apply the [entropy lower bound from the largest atom](entropy-lower-bound-from-the-largest-atom.md) to that posterior to get $2(1-\Pi_y)\leq H(X\mid Y=y)$, then average over $Y$. An arbitrary decoder need not satisfy this bound; it uses the optimum conditional decision rule.

## ↑ Ancestors (6)

1. [Maximum a posteriori decoding](maximum-a-posteriori-decoding.md)
2. [Coding theory](coding-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2010/2/c/solution.md)
