# Mixed-point norm identity for alternating updates

↑ **Parent:** [Alternating proximal-gradient operator](alternating-proximal-gradient-operator.md)

For two mixed points with difference $(p,q)$ and gradient difference $(a,b)$, the input difference is $(p,q+\tau b)$ and the output difference is $(p-\tau a,q)$. Their squared-norm difference is $-2\tau(\langle p,a\rangle+\langle q,b\rangle)+\tau^2(\|a\|^2-\|b\|^2)$. This exact identity is a reusable way to prove averagedness without assuming the two block maps are individually nonexpansive.

## ↑ Ancestors (8)

1. [Alternating proximal-gradient operator](alternating-proximal-gradient-operator.md)
2. [Proximal gradient method](proximal-gradient-method.md)
3. [Proximal operator](proximal-operator.md)
4. [Convex optimization](convex-optimization-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
