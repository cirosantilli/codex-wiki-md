<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [connection on a vector bundle](../../../../../../connection-vector-bundle.md) is an $\mathbb R$-linear map

$$
\nabla:\Gamma(E)\longrightarrow\Omega^1(M;E)
$$

which satisfies $\nabla(fs)=df\otimes s+f\nabla s$ for every [smooth function](../../../../../../smooth-function.md) $f$ and section $s$. Here $\Omega^1(M;E)=\Gamma(T^*M\otimes E)$. Equivalently, writing $\nabla_Xs=(\nabla s)(X)$, it is linear over [smooth functions](../../../../../../smooth-function.md) in $X$, linear over $\mathbb R$ in $s$, and obeys

$$
\nabla_X(fs)=X(f)s+f\nabla_Xs.
$$

Choose a trivializing [open cover](../../../../../../open-cover.md) and a [local frame](../../../../../../frame-of-a-vector-bundle.md) $e_{i1},\ldots,e_{ir}$ on each $U_i$. Differentiating the coefficient functions gives a local [connection on a vector bundle](../../../../../../connection-vector-bundle.md):

$$
\nabla^i_X\left(\sum_a s^a e_{ia}\right)=\sum_a X(s^a)e_{ia}.
$$

No compatibility of these local connections is assumed. Choose a smooth locally finite [partition of unity](../../../../../../partition-of-unity.md) $\{\phi_i\}$ subordinate to the cover and define

$$
\boxed{\nabla_Xs=\sum_i\phi_i\nabla^i_X(s|_{U_i}),}
$$

extending each weighted term by zero outside $U_i$. Its support lies inside $U_i$, so each extension is smooth, and local finiteness makes the whole sum smooth. The operation is linear over [smooth functions](../../../../../../smooth-function.md) in $X$. For the Leibniz rule,

$$
\nabla_X(fs)=\sum_i\phi_i\bigl(X(f)s+f\nabla^i_Xs\bigr)
=X(f)s+f\nabla_Xs,
$$

using $\sum_i\phi_i=1$. This proves **every smooth [vector bundle](../../../../../../vector-bundle.md) admits a connection** by the [construction of a vector bundle connection by a partition of unity](../../../../../../construction-of-a-vector-bundle-connection-by-a-partition-of-unity.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
