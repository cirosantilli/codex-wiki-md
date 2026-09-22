<h1 id="35a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let the [pair potential](../../../../../../pair-potential.md) be $u(r)$, so that in the dilute limit only one interacting pair need be retained at a time. The leading [Mayer f-function](../../../../../../mayer-f-function.md) expansion is

$$
e^{-U/T}-1\simeq\sum_{1\leq i<j\leq N}
\left(e^{-u(|\mathbf x_i-\mathbf x_j|)/T}-1\right).
$$

For each pair, translation of its center coordinate supplies $V$ and the other $N-2$ particles supply $V^{N-2}$. Neglecting boundary corrections,

$$
\frac1{V^N}\int(e^{-U/T}-1)\,d^{3N}x
\simeq \frac{N(N-1)}{2V}\int_{\mathbb R^3}(e^{-u(r)/T}-1)\,d^3r.
$$

The [Taylor expansion](../../../../../../taylor-expansion.md) $\log(1+x)=x+O(x^2)$ and $N(N-1)\simeq N^2$ in the [thermodynamic limit](../../../../../../thermodynamic-limit.md) give

$$
\boxed{F=F_{\rm ideal}+\frac{N^2T}{V}B(T)},
\qquad
\boxed{B(T)=\frac12\int_{\mathbb R^3}\left(1-e^{-u(r)/T}\right)d^3r
=2\pi\int_0^\infty\left(1-e^{-u(r)/T}\right)r^2\,dr}.
$$

Using $P=-(\partial F/\partial V)_{T,N}$ and the [ideal gas free energy](../../../../../../ideal-gas-free-energy.md),

$$
\boxed{P=\frac{NT}{V}+\frac{N^2T}{V^2}B(T)}.
$$

With [number density](../../../../../../number-density.md) $n=N/V$, this is $P/(nT)=1+B(T)n+O(n^2)$, so $B(T)$ is precisely the [second virial coefficient](../../../../../../second-virial-coefficient.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [35A](../../35a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
