# Kernel dimensions of powers of a nilpotent map

↑ **Parent:** [Nilpotent linear map](nilpotent-linear-map.md)

For a [nilpotent linear map](nilpotent-linear-map.md) with [minimal polynomial](minimal-polynomial.md) $x^m$, set $K_i=\ker T^i$ and $d_i=\dim K_i$, with $d_0=0$. Then

$$
\boxed{0=d_0<d_1<\cdots<d_m=\dim V,\qquad d_{i+1}-d_i\leq d_i-d_{i-1}}.
$$

For strictness, choose $w$ with $T^{m-1}w\ne0$. The [vector](vector.md) $T^{m-1-i}w$ belongs to $K_{i+1}\setminus K_i$ for $0\leq i<m$. For the second inequality, the [rank-nullity theorem](rank-nullity-theorem.md) gives

$$
\dim T^i(K_{i+1})=d_{i+1}-d_i,\qquad
\dim T^{i-1}(K_i)=d_i-d_{i-1}.
$$

The first image is contained in the second because $T(K_{i+1})\subseteq K_i$.

If the [Nilpotent Jordan block](nilpotent-jordan-block.md) sizes are $s_1,\ldots,s_r$, then

$$
d_i=\sum_{j=1}^r\min(i,s_j),\qquad d_i-d_{i-1}=\#\{j:s_j\geq i\}.
$$

Thus successive increments count the [Jordan blocks](jordan-block.md) reaching a given size, and $(d_i-d_{i-1})-(d_{i+1}-d_i)$ counts blocks of size exactly $i$, with $d_{m+1}=d_m$. The [nullities](nullity-of-a-linear-map.md) determine the entire [Jordan normal form](jordan-normal-form.md). Conversely any positive nonincreasing integer increments summing to $\dim V$ are realized by taking the corresponding numbers of each [Nilpotent Jordan block](nilpotent-jordan-block.md).

## ↑ Ancestors (7)

1. [Nilpotent linear map](nilpotent-linear-map.md)
2. [Operator theory](linear-operator-theory-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Injections between successive kernel quotients](injections-between-successive-kernel-quotients.md)
- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2023/2/a/i/solution.md)
- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2023/2/a/ii/solution.md)
