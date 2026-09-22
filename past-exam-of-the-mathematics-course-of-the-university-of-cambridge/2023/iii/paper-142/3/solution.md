<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [splitting principle for complex vector bundles](../../../../../splitting-principle-for-complex-vector-bundles.md) says that for every complex vector bundle $E\to X$ there is a map $p:F(E)\to X$ such that $p^*$ is injective on cohomology and

$$
p^*E=L_1\oplus\cdots\oplus L_r
$$

splits into complex line bundles. Write $x_i=c_1(L_i)$ for the formal [Chern roots](../../../../../chern-root.md).

Define the [Chern character](../../../../../chern-character.md) after this injective pullback by

$$
\operatorname{ch}(E)=\sum_{i=1}^r e^{x_i}.
$$

Each homogeneous component is a symmetric polynomial in the $x_i$ with rational coefficients, hence a polynomial in the elementary symmetric functions $c_j(E)$. It therefore descends uniquely to $H^{\mathrm{ev}}(X;\mathbb Q)$ and depends only on $E$. Set

$$
\operatorname{ch}(E-F)=\operatorname{ch}(E)-\operatorname{ch}(F)
$$

on the [Grothendieck group](../../../../../grothendieck-group.md) $K^0(X)$; additivity under direct sums makes this well defined.

If $E$ has roots $x_i$ and $F$ has roots $y_j$, then $E\otimes F$ has roots $x_i+y_j$. Consequently

$$
\begin{aligned}
\operatorname{ch}(E\oplus F)
&=\sum_i e^{x_i}+\sum_j e^{y_j}
=\operatorname{ch}(E)+\operatorname{ch}(F),\\
\operatorname{ch}(E\otimes F)
&=\sum_{i,j}e^{x_i+y_j}
=\left(\sum_i e^{x_i}\right)
\left(\sum_j e^{y_j}\right)
=\operatorname{ch}(E)\operatorname{ch}(F).
\end{aligned}
$$

It also sends the trivial line to $1$, so it is a unital ring homomorphism.

For $S^{2n}$, a generator of $\widetilde K^0(S^{2n})$ is the $n$-fold exterior product of the degree-two [Bott element](../../../../../bott-element.md). The Chern character respects exterior products, and the degree-two Bott element has Chern character equal, up to sign, to the integral generator of $\widetilde H^2(S^2;\mathbb Z)$. Its $n$-fold product maps to the integral top-dimensional generator. Hence the [Chern character on an even-dimensional sphere is integral](../../../../../chern-character-on-an-even-dimensional-sphere-is-integral.md).

Let the formal Chern roots of $E\to S^{2n}$ be $x_1,\ldots,x_r$ and write $p_n=\sum_i x_i^n$. Since

$$
H^{2j}(S^{2n};\mathbb Z)=0
\qquad(0<j<n),
$$

all lower Chern classes $c_1(E),\ldots,c_{n-1}(E)$ vanish. The [Newton identities](../../../../../newton-s-identities.md) then reduce to

$$
p_n=(-1)^{n+1}n\,c_n(E).
$$

The degree-$2n$ term of the Chern character is therefore

$$
\operatorname{ch}_n(E)
=\frac{p_n}{n!}
=(-1)^{n+1}\frac{c_n(E)}{(n-1)!}.
$$

Its evaluation on the [fundamental class](../../../../../fundamental-class.md) is an integer by integrality of the reduced Chern character. Thus

$$
\left\langle c_n(E),[S^{2n}]\right\rangle
$$

is divisible by $(n-1)!$, proving the [Divisibility of the top Chern number on an even-dimensional sphere](../../../../../divisibility-of-the-top-chern-number-on-an-even-dimensional-sphere.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 142](../../paper-142-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
