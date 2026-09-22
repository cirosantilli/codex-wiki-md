# Injections between successive kernel quotients

↑ **Parent:** [Kernel of a linear map](kernel-of-a-linear-map-split.md)

For a [linear map](linear-map.md) $T:V\to V$, set $K_i=\ker T^i$ and $K_0=0$. Since $T(K_{i+1})\subseteq K_i$ and $T(K_i)\subseteq K_{i-1}$, the rule $v+K_i\mapsto Tv+K_{i-1}$ defines a [linear map](linear-map.md) $K_{i+1}/K_i\to K_i/K_{i-1}$. It is [injective](injective-function.md): if $Tv\in K_{i-1}$, then $T^iv=0$, so $v\in K_i$. In finite [dimension](dimension-vector-space.md), this proves

$$
\dim K_{i+1}-\dim K_i\leq\dim K_i-\dim K_{i-1}.
$$

The [linear map](linear-map.md) need not be [surjective](surjective-function.md): for $T=0$ on a nonzero [vector space](vector-space-split.md), its $i=1$ instance is $0\to V$. For a [nilpotent linear map](nilpotent-linear-map.md), these [dimensions](dimension-vector-space.md) are the increments in the [kernel dimensions of powers of a nilpotent map](kernel-dimensions-of-powers-of-a-nilpotent-map.md).

## ↑ Ancestors (6)

1. [Kernel of a linear map](kernel-of-a-linear-map-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2021/1/a/iii/solution.md)
