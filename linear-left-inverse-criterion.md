# Linear left inverse criterion

↑ **Parent:** [Linear map](linear-map.md)

A [linear map](linear-map.md) $T:V\to W$ between [finite-dimensional vector spaces](finite-dimensional-vector-space.md) admits a linear [left inverse](left-inverse.md) $S:W\to V$ if and only if its [kernel of a linear map](kernel-of-a-linear-map-split.md) is $\{0\}$, equivalently if and only if it is [injective](injective-function.md).

Necessity follows from $Tv=0\Longrightarrow v=STv=0$. For sufficiency, choose a [basis](basis.md) $v_1,\ldots,v_n$ of $V$. Triviality of the [kernel of a linear map](kernel-of-a-linear-map-split.md) implies that $Tv_1,\ldots,Tv_n$ are [linearly independent](linear-independence.md). By [basis extension](basis-extension.md), they extend to a [basis](basis.md) $Tv_1,\ldots,Tv_n,w_{n+1},\ldots,w_m$ of $W$. Define $S(Tv_i)=v_i$ and $S(w_j)=0$, and extend by [linearity](linearity.md). Then $STv_i=v_i$ on a [basis](basis.md), proving $ST=I_V$.

The freedom in $S$ lies in its values on a [direct-sum complement](direct-sum-complement.md) of the [image of a linear map](image-of-a-linear-map.md). For example, for $T(x,y)=(x,y,0)$, every [linear map](linear-map.md) $S(u,v,w)=(u+aw,v+bw)$ is a [left inverse](left-inverse.md), with arbitrary [scalars](scalar.md) $a,b$. A [right inverse](right-inverse.md) instead requires $T$ to be a [surjective linear map](surjective-linear-map.md).

## ↑ Ancestors (7)

1. [Linear map](linear-map.md)
2. [Vector space](vector-space-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-i/1/c/iii/solution.md)
