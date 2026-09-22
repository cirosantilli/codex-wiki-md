# Symmetric node pairing bound for interpolation on the unit interval

↑ **Parent:** [Polynomial interpolation](polynomial-interpolation.md)

Suppose $m$ interpolation nodes in $[0,1]$ occur in pairs $a,1-a$, with the middle node $1/2$ if $m$ is odd. For each pair,

$$
|(x-a)(x-(1-a))|=|(x-1/2)^2-(a-1/2)^2|\le1/4,
$$

because both squared quantities lie between zero and one quarter. An unpaired middle factor has magnitude at most one half. Multiplication gives the displayed bound on the nodal [polynomial](polynomial-split.md).

The [polynomial interpolation](polynomial-interpolation.md) remainder therefore satisfies $\|f-p_{m-1}\|_\infty\le\|f^{(m)}\|_\infty/[2^m m!]$ for $f\in C^m[0,1]$. For $f(x)=\sin2x$, the [derivative](derivative.md) bound $\|f^{(m)}\|_\infty\le2^m$ gives the particularly simple error bound $1/m!$. This proves [uniform convergence](uniform-convergence.md) for these symmetric-node interpolants of that function. It is not a general convergence theorem for arbitrary [continuous](continuous-function.md) interpolation data.

## ↑ Ancestors (7)

1. [Polynomial interpolation](polynomial-interpolation.md)
2. [Interpolation](interpolation-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-statistics-and-options-ii-course-of-the-university-of-oxford/2009/p/p3/d/solution.md)
