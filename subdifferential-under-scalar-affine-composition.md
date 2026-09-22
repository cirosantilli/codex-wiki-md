# Subdifferential under scalar affine composition

↑ **Parent:** [Subdifferential](subdifferential.md)

For a finite [convex function](convex-function.md) $h:\mathbb R\to\mathbb R$, the [function](function-split.md) $f(x)=h(c^Tx+b)$ is [convex](convex-function.md). The [subgradient inequality](subgradient-inequality.md) gives $c\partial h(u)\subseteq\partial f(x)$, where $u=c^Tx+b$. Conversely, every [subgradient](subgradient.md) $g$ of $f$ annihilates $\ker c^T$, because $f$ is constant on lines in those directions. For $c\ne0$, write $g=cv$ and test the subgradient inequality at $y=x+(t-u)c/\|c\|_2^2$; this proves $v\in\partial h(u)$. For $c=0$, $f$ is constant and both sides are $\{0\}$ since a finite [convex](convex-function.md) [function](function-split.md) on the real line has a nonempty [subdifferential](subdifferential.md) everywhere.

## ↑ Ancestors (6)

1. [Subdifferential](subdifferential.md)
2. [Convex optimization](convex-optimization-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205/5/solution.md)
