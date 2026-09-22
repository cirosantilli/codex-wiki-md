<h1 id="contour-shift-proof-of-the-paley-wiener-schwartz-theorem">Contour-shift proof of the Paley–Wiener–Schwartz theorem</h1>

↑ **Parent:** [Paley–Wiener–Schwartz theorem](paley-wiener-schwartz-theorem.md)

For the forward implication, finite [order of a distribution](order-of-a-distribution.md) makes $F(\zeta)=\langle u,e^{-ix\cdot\zeta}\rangle$ entire. Use a smooth cutoff in an $\varepsilon$-neighborhood of the support set, with derivatives of order $j$ bounded by $C_j\varepsilon^{-j}$. Taking $\varepsilon=(1+|\zeta|)^{-1}$ in the finite-order estimate gives the polynomial factor and adds at most $e$ to the desired exponential bound. This shrinking cutoff recovers the exact support indicator, instead of an arbitrarily enlarged one.

For the converse, the real restriction of $F$ has [polynomial growth](polynomial-growth.md) and defines an inverse [tempered distribution](tempered-distribution.md). If a [test function](test-function.md) $\varphi$ is supported in $x\cdot\omega\geq R+\eta$ for a unit vector $\omega$ and $\eta>0$, [contour shifting](contour-shifting.md) gives

$$
\langle u,\varphi\rangle=(2\pi)^{-n}\int F(\xi+it\omega)\widehat\varphi(-\xi-it\omega)\,d\xi.
$$

Repeated [integration by parts](integration-by-parts.md) gives, for every integer $M$,

$$
|\widehat\varphi(-\xi-it\omega)|
\leq C_M(1+t)^{2M}e^{-(R+\eta)t}(1+|\xi|^2)^{-M}.
$$

Choosing $2M>N+n$ justifies the shift by [Cauchy integral theorem](cauchy-s-integral-theorem.md) and bounds the pairing by $C'(1+t)^{N+2M}e^{-\eta t}$, which tends to zero. Half-spaces of this form cover the complement of the ball, and a [partition of unity](partition-of-unity.md) proves the support inclusion. For general compact convex $K$, replace $R$ by $H_K(\omega)$ in each separating direction. [Fourier inversion](fourier-inversion-theorem.md) gives uniqueness. A related proof outline appears in [Richard Melrose's distribution-theory problem set](https://math.mit.edu/~rbm/Problems4.pdf).

**Table of contents**

- [Mollifier regularization for contour recovery of support](mollifier-regularization-for-contour-recovery-of-support.md)

## ↑ Ancestors (7)

1. [Paley–Wiener–Schwartz theorem](paley-wiener-schwartz-theorem.md)
2. [Paley–Wiener theorem](paley-wiener-theorem.md)
3. [Distribution theory](distribution-theory-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-327/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-327/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-327/3/solution.md)
