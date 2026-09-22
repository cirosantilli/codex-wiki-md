# Capacity after independent output erasure

↑ **Parent:** [Channel capacity](channel-capacity.md)

Pass the output of a [discrete memoryless channel](discrete-memoryless-channel.md) of [channel capacity](channel-capacity.md) $C$ through an independent [finite-alphabet erasure channel](finite-alphabet-erasure-channel.md) with erasure probability $p$. Its capacity becomes $(1-p)C$.

To prove it, let $X$ be the original input, $Y$ the original output, $E$ the erasure indicator, and $Z$ the final output. Since the erasure marker is distinguishable, $E$ is determined by $Z$. It is independent of $X,Y$, so the [chain rule for mutual information](chain-rule-for-mutual-information.md) gives $I(X;Z)=I(X;E,Z)=I(X;Z\mid E)=(1-p)I(X;Y)$. Maximization over the same input distributions proves the formula. For $p<1$ the maximizing distributions are exactly the original channel's maximizers. For $p=1$, every input distribution attains the zero capacity. Input-dependent erasure need not satisfy this scaling identity.

## ↑ Ancestors (6)

1. [Channel capacity](channel-capacity.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2009/3/c/solution.md)
