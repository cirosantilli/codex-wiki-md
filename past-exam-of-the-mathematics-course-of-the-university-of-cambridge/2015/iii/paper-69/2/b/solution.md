<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the unnormalized [Fourier transform](../../../../../../fourier-transform.md) in the question and the [Plancherel theorem](../../../../../../plancherel-theorem.md), with inverse factor $1/(2\pi)$. For a general $L^2$ [scaling function](../../../../../../scaling-function.md), the transform is interpreted in the $L^2$ sense; the printed integral need not be absolutely convergent. All frequency identities are almost-everywhere statements.

Changing variables in the [Fourier transform](../../../../../../fourier-transform.md) gives

$$
\widehat{\phi(2\cdot-n)}(\xi)=\frac12e^{-in\xi/2}f(\xi/2).
$$

Thus taking the transform of the [scaling refinement equation](../../../../../../scaling-refinement-equation.md) gives $f(\xi)=m(\xi/2)f(\xi/2)$, or

$$
\boxed{f(2t)=m(t)f(t),\qquad m(t)=\frac12\sum_na_ne^{-int}.}
$$

Conversely the same calculation and injectivity of the [Fourier transform](../../../../../../fourier-transform.md) recover refinement, with convergence understood in $L^2$.

To justify both the [orthogonality](../../../../../../orthogonal-vectors.md) assertion and this convergence precisely, put $P(t)=\sum_{k\in\mathbb Z}|f(t+2\pi k)|^2$. It belongs to $L^1[-\pi,\pi]$ by monotone integration. The [Plancherel theorem](../../../../../../plancherel-theorem.md) gives

$$
\langle\phi,\phi(\cdot-j)\rangle
=\frac1{2\pi}\int_{-\pi}^{\pi}P(t)e^{-ijt}\,dt.
$$

Hence orthonormality of all integer translates is equivalent, by [uniqueness of Fourier coefficients in L1](../../../../../../uniqueness-of-fourier-coefficients-in-l1.md), to **the periodized-energy condition**

$$
\boxed{P(t)=1\quad\text{almost everywhere}.}
$$

When this holds, the squared norm of $\sum_na_n\phi(2\cdot-n)$ is $\tfrac12\sum_n|a_n|^2$, so square-summable coefficient series converge in $L^2$. In the converse direction the refinement identity and $P=1$ give, by splitting the periodization of $|f(2t)|^2$ into even and odd translates,

$$
1=|m(t)|^2+|m(t+\pi)|^2.
$$

Thus $m$ is bounded and its [Fourier coefficients](../../../../../../fourier-coefficient.md) $a_n/2$ are square summable. If $m_N$ are its [Fourier partial sum](../../../../../../fourier-partial-sum.md), then

$$
\int_{\mathbb R}|m_N(\xi/2)-m(\xi/2)|^2|f(\xi/2)|^2\,d\xi
=2\int_{-\pi}^{\pi}|m_N(t)-m(t)|^2P(t)\,dt\longrightarrow0.
$$

This verifies the transformed refinement series converges to $f$, completing the equivalence of the two pairs of conditions without imposing an unnecessary $L^1$ assumption on $\phi$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
