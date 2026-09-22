<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In the [truncated tensor algebra](../../../../../../truncated-tensor-algebra.md), let $\mathfrak g^N(V)$ be the linear span of all iterated [Lie brackets](../../../../../../lie-bracket.md) of elements of $V$ of length at most $N$, with bracket $[a,b]=a\otimes b-b\otimes a$. Brackets of length greater than $N$ vanish. The [free step-N nilpotent Lie group](../../../../../../free-step-n-nilpotent-lie-group.md) is

$$
G^N(V)=\exp\mathfrak g^N(V)\subseteq1+\bigoplus_{k=1}^N V^{\otimes k}.
$$

The exponential and logarithm are the finite series

$$
\exp(\ell)=\sum_{j=0}^N\frac{\ell^{\otimes j}}{j!},\qquad
\log(1+a)=\sum_{j=1}^N\frac{(-1)^{j+1}a^{\otimes j}}j.
$$

Its multiplication is the tensor multiplication above, its identity is $e=(1,0,\ldots,0)$, and its inverse is

$$
(1+a)^{-1}=\sum_{j=0}^N(-a)^{\otimes j},\qquad
(\exp\ell)^{-1}=\exp(-\ell).
$$

The truncated [Baker--Campbell--Hausdorff formula](../../../../../../baker-campbell-hausdorff-formula.md) shows that this multiplication stays in the exponential of the [Lie algebra](../../../../../../lie-algebra-split.md). This is the connected simply connected [Lie group](../../../../../../lie-group.md) of the free step-$N$ nilpotent [Lie algebra](../../../../../../lie-algebra-split.md), rather than a discrete free nilpotent group.

Give the first layer $V$ its usual [Euclidean norm](../../../../../../euclidean-norm.md). An absolutely continuous curve $\gamma$ in $G^N(V)$ is horizontal if

$$
\dot\gamma_t=(L_{\gamma_t})_*\dot x_t,
$$

for an absolutely continuous control $x$ in $V$. In the [truncated tensor algebra](../../../../../../truncated-tensor-algebra.md) this equation is $\dot\gamma_t=\gamma_t\otimes\dot x_t$, truncated at degree $N$. Its horizontal length is $\int|\dot x_t|\,dt$. The [Carnot-Carathéodory distance](../../../../../../carnot-caratheodory-distance.md) is

$$
\boxed{d_{CC}(g,h)=\inf_{\gamma_0=g,\,\gamma_1=h\atop\gamma\ \mathrm{horizontal}}\int_0^1|\dot x_t|\,dt.}
$$

The first-layer [Lie brackets](../../../../../../lie-bracket.md) span the full [Lie algebra](../../../../../../lie-algebra-split.md), so horizontal curves reach every endpoint. Thus this infimum is finite; it is a left-invariant distance inducing the usual manifold topology. Dilations $\delta_\lambda(a)^{(k)}=\lambda^k a^{(k)}$ give $d_{CC}(\delta_\lambda g,\delta_\lambda h)=\lambda d_{CC}(g,h)$ for $\lambda>0$. Equivalently $d_{CC}(e,g)$ is the least length of a [bounded variation](../../../../../../total-variation-of-a-function.md) control whose step-$N$ [path signature](../../../../../../signature-of-a-bounded-variation-path.md) is $g$.

For $p\ge1$ set $N=\lfloor p\rfloor$. A [weak geometric p-rough path](../../../../../../weak-geometric-p-rough-path.md) is a continuous path $\mathbf X:[0,T]\to G^N(V)$, usually based at $e$, with

$$
\boxed{\sup_D\sum_{[u,v]\in D}d_{CC}(\mathbf X_u,\mathbf X_v)^p<\infty.}
$$

Its increments $\mathbf X_{s,t}=\mathbf X_s^{-1}\otimes\mathbf X_t$ obey $\mathbf X_{s,u}=\mathbf X_{s,t}\otimes\mathbf X_{t,u}$. Equivalently their degree-$k$ tensor components have finite $p/k$-variation and satisfy the [path signature](../../../../../../signature-of-a-bounded-variation-path.md) algebraic constraints. This is a group-valued definition; being a limit of smooth [path signatures](../../../../../../signature-of-a-bounded-variation-path.md) in the same $p$-variation topology is the stronger definition of a [geometric p-rough path](../../../../../../geometric-p-rough-path.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
