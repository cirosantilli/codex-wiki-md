# Convolution of Sobolev distributions

↑ **Parent:** [Sobolev space](sobolev-space-split.md)

For arbitrary real $s,t$, the [convolution](convolution.md) of $u\in H^s(\mathbb R)$ and $v\in H^t(\mathbb R)$ has a canonical definition as a [tempered distribution](tempered-distribution.md). With $\langle\xi\rangle=(1+\xi^2)^{1/2}$, write $A=\langle\xi\rangle^s\widehat u$ and $B=\langle\xi\rangle^t\widehat v$, both in the [L2 space](l2-space-is-a-hilbert-space.md). Then $AB\in L^1$ by [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md), and

$$
|\langle\widehat u\widehat v,\phi\rangle|
\leq\|u\|_{H^s}\|v\|_{H^t}\sup_\xi\langle\xi\rangle^{-s-t}|\phi(\xi)|.
$$

Thus the product defines a [tempered distribution](tempered-distribution.md), and the displayed [inverse Fourier transform](inverse-fourier-transform.md) defines $u*v$. This extends ordinary [convolution](convolution.md) of [Schwartz functions](schwartz-function.md) by the [convolution theorem](convolution-theorem.md) and density in the [Sobolev norm](sobolev-norm.md).

The result need not belong to any [Sobolev space](sobolev-space-split.md), even when both inputs belong to every [Sobolev space](sobolev-space-split.md). For $\widehat u=\widehat v=\xi^{-1/3}\mathbf1_{(0,1)}(\xi)$, each weighted squared input is integrable, but the squared product is $\xi^{-4/3}\mathbf1_{(0,1)}(\xi)$, which is not locally integrable at zero. Every weight $(1+\xi^2)^r$ is bounded above and below there, proving the failure for all real $r$.

## ↑ Ancestors (6)

1. [Sobolev space](sobolev-space-split.md)
2. [Functional analysis](functional-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-fourier-analysis-course-of-the-university-of-oxford/2023/2/b/iii/solution.md)
