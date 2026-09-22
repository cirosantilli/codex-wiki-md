# Continuous functions preserve convergent sequences

↑ **Parent:** [Continuous function](continuous-function.md)

For $f:D\to\mathbb R$ and $a\in D$, [continuity](continuous-function.md) at $a$ is equivalent to the following condition: every [sequence](sequence.md) $(x_n)$ in $D$ with $x_n\to a$ satisfies $f(x_n)\to f(a)$. This is useful when a [numerical method](numerical-method.md) or a [proof](mathematical-proof.md) approaches a point through successively refined [function inputs](function-input.md): applying a [continuous function](continuous-function.md) preserves the intended [limit](limit-of-a-function.md).

For the forward direction, choose $\delta$ from the [epsilon-delta definition of continuity](epsilon-delta-definition-of-continuity.md). A [convergent sequence](convergent-sequence.md) eventually lies in that input window, so its [function outputs](function-output.md) eventually lie in the requested output band. Conversely, if [continuity](continuous-function.md) fails, there is some $\varepsilon_0>0$ for which every input window contains an allowed $x$ with $|f(x)-f(a)|\geq\varepsilon_0$. Choosing such an $x_n$ within $1/n$ of $a$ gives $x_n\to a$ while $f(x_n)$ does not tend to $f(a)$. This converse relies on the countable shrinking windows available in [metric spaces](metric-space.md); a general [topological space](topological-space.md) needs a different formulation.

## ↑ Ancestors (8)

1. [Continuous function](continuous-function.md)
2. [Limit of a function](limit-of-a-function.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
