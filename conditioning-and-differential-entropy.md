# Conditioning and differential entropy

↑ **Parent:** [Conditioning reduces entropy](conditioning-reduces-entropy.md)

With appropriate [probability density functions](probability-density-function.md) and finite [differential entropies](differential-entropy.md), $h(X)-h(X\mid Y)=I(X;Y)\geq0$, with equality iff [independence](independent-random-variables.md). [Differential entropy](differential-entropy.md) does not reverse the inequality; infinite or undefined quantities cannot justify subtraction.[Theorem 2.4(3), printed p. 24: density and finiteness hypotheses for the differential-entropy identity](6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others/chapter-2-information-measures-mutual-information.md)

However, [differential entropy](differential-entropy.md) can be negative and depends on the choice of coordinates. For $X$ with a [uniform distribution](continuous-uniform-distribution.md) on an interval of length $a>0$, $h(X)=\log_2a$; in particular $a=1/2$ gives $-1$. Rescaling $X$ by a constant $c>0$ adds $\log_2c$ to both $h(X)$ and $h(X\mid Y)$, whenever they are finite, leaving the [mutual information](mutual-information.md) unchanged.[pp. 37–38: coordinate dependence, negative entropy, and linear rescaling](a-mathematical-theory-of-communication-by-claude-shannon.md)

If a continuously distributed $X$ is revealed exactly, its [conditional distribution](conditional-distribution.md) is a [Dirac measure](dirac-measure.md) with no ordinary [probability density function](probability-density-function.md). The discrete identity $H(X\mid X)=0$ has no finite [differential entropy](differential-entropy.md) counterpart. [Mutual information](mutual-information.md), defined through [relative entropy](kullback-leibler-divergence.md), is infinite here.[Theorem 2.4(1) and its proof, printed p. 24: I(X;X) is infinite for a non-discrete distribution](6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others/chapter-2-information-measures-mutual-information.md)

## ↑ Ancestors (7)

1. [Conditioning reduces entropy](conditioning-reduces-entropy.md)
2. [Conditional entropy](conditional-entropy.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
