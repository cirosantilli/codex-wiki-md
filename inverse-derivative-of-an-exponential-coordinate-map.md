# Inverse derivative of an exponential coordinate map

↑ **Parent:** [Derivative of a local inverse map](derivative-of-a-local-inverse-map.md)

This map is a [diffeomorphism](diffeomorphism.md) from $\mathbb R^2$ onto $V=\{(s,t):s>0,t>0,st>1\}$. Writing $q=e^x$, the inverse problem becomes $(s-q)(t-q)=1$ with $0<q<\min(s,t)$. The left side decreases strictly from $st$ to zero, proving existence and uniqueness exactly on $V$. Its [Jacobian determinant](jacobian-determinant.md) is $-e^x(e^y+e^{-y})\ne0$, so the [inverse function theorem](inverse-function-theorem.md) supplies a differentiable inverse. Along $(x,y)=(c,c)$, applying the inverse Jacobian to $(1/2,1/2)$ gives $(e^{-c}/2,0)$. Establishing the actual image matters before using a global inverse, even when a local inverse already exists at the point of interest.

## ↑ Ancestors (10)

1. [Derivative of a local inverse map](derivative-of-a-local-inverse-map.md)
2. [Inverse function theorem](inverse-function-theorem.md)
3. [Differentiable map](differentiable-map.md)
4. [Multivariable calculus](multivariable-calculus-split.md)
5. [Calculus](calculus-split.md)
6. [Real analysis](real-analysis-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)
