# Laplace solution of a first-order equation with exponential memory

↑ **Parent:** [Volterra integral equation](volterra-integral-equation.md)

The [derivative](derivative.md) and [convolution theorem for Laplace transforms](convolution-theorem-for-laplace-transforms.md) give $[p+1/(p+2)]\bar x=1/p$. Partial fractions yield $\bar x=2/p-2/(p+1)-1/(p+1)^2$, so $x(t)=2-(2+t)e^{-t}$ tends to two. A direct check gives $x'=(1+t)e^{-t}$ and $(e^{-2t}*x)(t)=1-(1+t)e^{-t}$. Introducing the memory variable $w=e^{-2t}*x$ gives the equivalent local system $x'+w=1$, $w'=x-2w$, $w(0)=0$, explaining why the transform denominator has a repeated pole at $p=-1$.

## ↑ Ancestors (6)

1. [Volterra integral equation](volterra-integral-equation.md)
2. [Integral equation](integral-equation.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
