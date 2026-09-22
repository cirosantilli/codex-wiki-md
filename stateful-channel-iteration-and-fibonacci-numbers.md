# Stateful channel iteration and Fibonacci numbers

↑ **Parent:** [Fibonacci number](fibonacci-number.md)

Consider a component that remembers its previous input $p$ and maps input $x$ to $x+p$, then sets $p:=x$. Feeding each output back into the same component gives state transition $(x,p)\mapsto(x+p,x)$. Starting at $(1,0)$, the successive outputs are $1,2,3,5,\ldots$, the [Fibonacci numbers](fibonacci-number.md) $F_{k+1}$ after $k\geq1$ calls. The state transition, rather than a memoryless [function](function-split.md) on one [integer](integer-split.md), explains the recurrence. Replacing the component between calls or repeatedly feeding a fixed external input gives different behavior.

## ↑ Ancestors (7)

1. [Fibonacci number](fibonacci-number.md)
2. [Sequence and series](sequence-and-series-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
