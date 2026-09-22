<h1 id="27k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put

$$
H(u)=\frac{4\sin^2(u/2)}{u^2},
\qquad H(0)=1.
$$

This function is bounded near zero and is $O(u^{-2})$ at infinity, so $H\in L^1(\mathbb R)$ and the defining integral for $g$ converges absolutely.

For the [triangular function](../../../../../../triangular-function.md)

$$
h(x)=(1-|x|)\mathbf1_{[-1,1]}(x),
$$

direct integration gives

$$
\begin{aligned}
\widehat h(u)
&=\int_{-1}^1(1-|x|)e^{iux}\,dx\\
&=2\int_0^1(1-x)\cos(ux)\,dx\\
&=\frac{2(1-\cos u)}{u^2}
=\frac{4\sin^2(u/2)}{u^2}=H(u).
\end{aligned}
$$

The [Fourier inversion theorem](../../../../../../fourier-inversion-theorem.md), or equivalently the [Fourier transform of a triangular function](../../../../../../fourier-transform-of-a-triangular-function.md), therefore yields

$$
\boxed{g(x)=(1-|x|)\mathbf1_{[-1,1]}(x).}
$$

In particular $g(x)=0$ whenever $|x|>1$. Finally,

$$
\boxed{\|g\|_2^2
=2\int_0^1(1-x)^2\,dx
=\frac23.}
$$

This also agrees with the [Plancherel theorem](../../../../../../plancherel-theorem.md) applied to $h$ and $H$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [27K](../../27k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
