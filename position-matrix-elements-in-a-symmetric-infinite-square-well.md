# Position matrix elements in a symmetric infinite square well

↑ **Parent:** [Infinite square well](infinite-square-well.md)

For a well $-a<x<a$, choose normalized [energy eigenstates](energy-eigenstate.md) $\phi_n=a^{-1/2}\sin[(n+1)\pi(x+a)/(2a)]$, $n=0,1,\ldots$. The diagonal position [matrix elements](matrix-element.md) vanish by the [parity operator](parity-operator.md). For $k\ne n$,

$$
\langle\phi_k|x|\phi_n\rangle=
\frac{8a(k+1)(n+1)[(-1)^{k+n}-1]}{\pi^2[(k+1)^2-(n+1)^2]^2}.
$$

To derive it, set $y=x+a$ and use $2\sin Ay\sin By=\cos[(A-B)y]-\cos[(A+B)y]$. For unequal positive integer indices $r,s$, the constant part of $x=y-a$ integrates to zero by [orthogonality](orthogonal-vectors.md), while

$$
\int_0^{2a}(y-a)\cos\left(\frac{j\pi y}{2a}\right)dy
=\frac{4a^2[(-1)^j-1]}{j^2\pi^2}\quad(j\ne0).
$$

Taking the difference for $j=r-s$ and $j=r+s$ yields the formula after setting $r=k+1,s=n+1$. It vanishes for equal parity and gives $x_{01}=-32a/(9\pi^2)$ for this phase convention.

## ↑ Ancestors (5)

1. [Infinite square well](infinite-square-well.md)
2. [Quantum mechanics](quantum-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Degenerate orbital exchange splitting from a product perturbation](degenerate-orbital-exchange-splitting-from-a-product-perturbation.md)
- [First-order parity selection in an infinite well](first-order-parity-selection-in-an-infinite-well.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2021/section-b/6/c/solution.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2022/section-b/5/b/solution.md)
