# Coarse embedding

↑ **Parent:** [Metric embedding](metric-embedding.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coarse_embedding)

A map $f:X\to Y$ between [metric spaces](metric-space.md) is a [coarse embedding](coarse-embedding.md) when nondecreasing control functions $\rho_-,\rho_+:[0,\infty)\to[0,\infty)$ satisfy

$$
\rho_-(d_X(x,y))\leq d_Y(f(x),f(y))\leq\rho_+(d_X(x,y)),
\qquad \rho_-(t)\longrightarrow\infty.
$$

The last condition means that distances tending to infinity in the source must also tend to infinity in the target. The upper control prevents bounded source distances from having unbounded image distances. Unlike a [metric embedding](metric-embedding.md) as defined here, a [coarse embedding](coarse-embedding.md) need not be [injective](injective-function.md): its lower control may vanish at small distances. Finite [bi-Lipschitz distortion](bi-lipschitz-distortion.md) implies a [coarse embedding](coarse-embedding.md) by taking $\rho_-(t)=at$ and $\rho_+(t)=bt$, but nonlinear controls such as $\sqrt t$ allow much more compression.

**Table of contents**

- [Uniform coarse embedding of a family of metric spaces](uniform-coarse-embedding-of-a-family-of-metric-spaces.md)

## ↑ Ancestors (6)

1. [Metric embedding](metric-embedding.md)
2. [Functional analysis](functional-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Coarse embedding](coarse-embedding.md)
- [Metric embedding](metric-embedding.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-155/1/solution.md)
- [Uniform coarse embedding of a family of metric spaces](uniform-coarse-embedding-of-a-family-of-metric-spaces.md)
