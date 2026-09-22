# Trivial kernel

↑ **Parent:** [Kernel of a linear map](kernel-of-a-linear-map.md)

A [linear map](linear-map.md) $T:V\to W$ has a trivial [kernel](kernel-of-a-linear-map.md) when $\ker T=\{0_V\}$: the [zero vector](zero-vector.md) is the only input producing the zero output. The [kernel](kernel-of-a-linear-map.md) is a [singleton set](singleton-mathematics.md), not the [empty set](empty-set.md), because every [linear map](linear-map.md) sends zero to zero. Equivalently, its [nullity](nullity-of-a-linear-map.md) is zero and $T$ is [injective](injective-function.md). This holds even without a finite-dimensional hypothesis; see [Linear Algebra Done Right by Sheldon Axler (4th edition)](linear-algebra-done-right-by-sheldon-axler-4th-edition.md).

The reason this zero-output test controls all outputs is [linearity](linearity.md):

$$
T(v)=T(w)\iff T(v-w)=0\iff v-w\in\ker T.
$$

With a [trivial kernel](trivial-kernel.md), equal outputs force equal inputs. Therefore every equation $T(x)=b$ has at most one solution. Existence is a separate question: $b$ must belong to the [image of a linear map](image-of-a-linear-map.md). In the [fiber](fiber-of-a-function.md) description under [nullity](nullity-of-a-linear-map.md), $x_0+\{0\}$ is just the single point $x_0$.

For example, the [linear map](linear-map.md) $J:\mathbb R^2\to\mathbb R^3$, $J(x,y)=(x,y,0)$, has [trivial kernel](trivial-kernel.md) and [full column rank](full-column-rank.md):

$$
J=\begin{pmatrix}1&0\\0&1\\0&0\end{pmatrix},\qquad
\ker J=\{0\},\qquad\operatorname{rank}J=2.
$$

The output $(3,4,0)$ comes from exactly $(3,4)$, while $(3,4,1)$ is unreachable. Conversely, $P:\mathbb R^3\to\mathbb R^2$, $P(x,y,z)=(x,y)$, is [surjective](surjective-function.md) and has [full row rank](full-row-rank.md), but its [kernel](kernel-of-a-linear-map.md) is $\operatorname{span}\{(0,0,1)\}$: every output $(a,b)$ comes from the solution [straight line](straight-line.md) $(a,b,s)$.

For an $m\times n$ [matrix](matrix.md), a [trivial kernel](trivial-kernel.md) is equivalent to [matrix rank](matrix-rank.md) $n$ and [linear independence](linear-independence.md) of its columns. It can therefore occur only if $n\leq m$. If $m=n$, the [rank-nullity theorem](rank-nullity-theorem.md) also forces [surjectivity](surjective-function.md), giving an [invertible matrix](invertible-matrix.md); if $m>n$, the example $J$ shows why unique recovery of reachable inputs does not imply that every output is reachable. Finally, a [trivial kernel](trivial-kernel.md) guarantees exact uniqueness without guaranteeing numerical stability: the [singular matrix](singular-matrix.md) example $A(t)$ has [trivial kernel](trivial-kernel.md) for every $t\ne0$, even as its [condition number](condition-number.md) grows without bound when $t$ approaches zero.

## ↑ Ancestors (6)

1. [Kernel of a linear map](kernel-of-a-linear-map.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Invertible matrix](invertible-matrix.md)
- [Matrix inverse](matrix-inverse.md)
- [Noninjective linear measurement](noninjective-linear-measurement.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-326/1/c/iv/solution.md)
- [Trivial kernel](trivial-kernel.md)
