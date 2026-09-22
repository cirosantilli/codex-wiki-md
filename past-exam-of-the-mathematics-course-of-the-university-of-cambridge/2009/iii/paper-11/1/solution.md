<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

On any [compact set](../../../../../compact-space.md) avoiding the integers, write

$$
\frac1{z-n}+\frac1n=\frac{z}{n(z-n)}.
$$

For all sufficiently large $|n|$, uniformly on that [compact set](../../../../../compact-space.md) this is $O(|n|^{-2})$. The summands in the higher series are $O(|n|^{-k})$ for $k\ge2$. The [Weierstrass M-test](../../../../../weierstrass-m-test.md) therefore gives [locally uniform convergence](../../../../../locally-uniform-convergence.md) away from the integer [poles](../../../../../pole.md) and permits termwise differentiation. Near an integer $m$, isolate its singular summand; all the others converge uniformly on a small [neighborhood](../../../../../neighbourhood-mathematics.md). Thus **the first function has a simple [pole](../../../../../pole.md) of [residue](../../../../../residue.md) one at each integer, and the $k$th function has a [pole](../../../../../pole.md) of order $k$ there with principal part $(z-m)^{-k}$**. There are no other singularities, so all are [meromorphic functions](../../../../../meromorphic-function.md).

Pairing positive and negative indices is legitimate because the regularized first series converges absolutely. It becomes

$$
\varepsilon_1(z)=\frac1z+\sum_{n=1}^{\infty}\frac{2z}{z^2-n^2}.
$$

Here is a direct derivation of its [cotangent partial-fraction expansion](../../../../../cotangent-partial-fraction-expansion.md). Fix $z\notin\mathbb Z$ and integrate $F(\zeta)=\pi\cot(\pi\zeta)/(\zeta^2-z^2)$ around the square with real and imaginary coordinates $\pm R$, $R=N+1/2$, taking $N$ large enough to enclose $\pm z$. On the vertical sides $|\cot\pi\zeta|\le1$, and on the horizontal sides it is at most $\coth(\pi R)$. Thus the [cotangent](../../../../../cotangent.md) is uniformly bounded and $|\zeta^2-z^2|\ge R^2-|z|^2$, so the contour integral is $O(R^{-1})\to0$.

The [residues](../../../../../residue.md) at integers are $1/(n^2-z^2)$; the two [residues](../../../../../residue.md) at $z$ and $-z$ sum to $\pi\cot(\pi z)/z$. The [residue theorem](../../../../../residue-theorem.md) and [absolute convergence](../../../../../absolute-convergence.md) of the integer [residue](../../../../../residue.md) sum consequently give

$$
0=\frac{\pi\cot\pi z}{z}+\sum_{n\in\mathbb Z}\frac1{n^2-z^2},
\qquad\varepsilon_1(z)=\pi\cot\pi z.
$$

Using the exponential definitions of [sine](../../../../../sine.md) and [cosine](../../../../../cosine.md) now yields, for $w=e^{2\pi iz}$,

$$
\boxed{\varphi_1(w)=\pi i\frac{w+1}{w-1},\qquad
\varepsilon_1(z)=\varphi_1(e^{2\pi iz}).}
$$

The same [locally uniform convergence](../../../../../locally-uniform-convergence.md) gives $\varepsilon_k'=-k\varepsilon_{k+1}$, including $k=1$. Hence if $\varepsilon_k(z)=\varphi_k(e^{2\pi iz})$, the [chain rule](../../../../../chain-rule.md) gives

$$
\boxed{\varphi_{k+1}(w)=-\frac{2\pi i}{k}\,w\varphi_k'(w).}
$$

This is a [rational function](../../../../../rational-function.md) whenever $\varphi_k$ is, proving the requested descent for every $k$ by induction, with

$$
\boxed{\varphi_2(w)=-\frac{4\pi^2w}{(w-1)^2}.}
$$

In particular periodicity is a consequence of the explicit descent, rather than an assumption about the summation order.

Finally, for $|z|<1$ expand each paired summand as a [geometric series](../../../../../geometric-series.md):

$$
\frac{2z}{z^2-n^2}=-2\sum_{j=0}^{\infty}\frac{z^{2j+1}}{n^{2j+2}}.
$$

On $|z|\le r<1$ the double series converges absolutely, since its absolute sum is at most $2r\sum_{n\ge1}n^{-2}/(1-r^2)$. Interchanging the sums and using the [Riemann zeta function](../../../../../riemann-zeta-function.md) gives the [Laurent series](../../../../../laurent-series.md)

$$
\boxed{\varepsilon_1(z)=\frac1z-2\sum_{j=0}^{\infty}\zeta(2j+2)z^{2j+1},\qquad0<|z|<1.}
$$

Thus the $z^{-1}$ coefficient is one; the positive odd coefficients are $-2\zeta(2j+2)$, and all other coefficients vanish.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
