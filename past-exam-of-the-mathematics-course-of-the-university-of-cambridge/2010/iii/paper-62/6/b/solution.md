<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Fourier transform](../../../../../../fourier-transform.md) convention $f(t)=\widehat\phi(t)=\int\phi(x)e^{-ixt}\,dx$ and the [Plancherel theorem](../../../../../../plancherel-theorem.md) normalization $\|\phi\|_2^2=(2\pi)^{-1}\|f\|_2^2$. For a general $L_2$ [scaling function](../../../../../../scaling-function.md), the transform means its $L_2$ extension; an ordinary absolutely convergent integral is not required.

A change of variables gives $\widehat{\phi(2\cdot-n)}(t)=\tfrac12e^{-int/2}f(t/2)$. Thus the [scaling refinement equation](../../../../../../scaling-refinement-equation.md) transforms to $f(t)=m(t/2)f(t/2)$, or **$f(2t)=m(t)f(t)$**, with the $2\pi$-periodic [MRA low-pass filter](../../../../../../low-pass-filter-of-a-multiresolution-analysis.md) $m(t)=\tfrac12\sum_na_ne^{-int}$. The periodicity is necessary; allowing an arbitrary quotient $f(2t)/f(t)$ would not express refinement by integer translates.

For orthonormality, let $P(t)=\sum_{k\in\mathbb Z}|f(t+2\pi k)|^2$. This is a $2\pi$-periodic $L_1$ function, since $f\in L_2$. The [Plancherel theorem](../../../../../../plancherel-theorem.md) gives

$$
\langle\phi(\cdot-j),\phi(\cdot-\ell)\rangle=\frac1{2\pi}\int_{\mathbb R}|f(t)|^2e^{i(\ell-j)t}\,dt=\frac1{2\pi}\int_0^{2\pi}P(t)e^{i(\ell-j)t}\,dt.
$$

These inner products equal $\delta_{j\ell}$ precisely when the [Fourier coefficients](../../../../../../fourier-coefficient.md) of $P$ agree with those of one. The [uniqueness of Fourier coefficients in L1](../../../../../../uniqueness-of-fourier-coefficients-in-l1.md) proves the equivalence

$$
\boxed{\{\phi(\cdot-n)\}\text{ orthonormal}\quad\Longleftrightarrow\quad\sum_k|f(t+2\pi k)|^2=1\ \text{a.e.}}
$$

For completeness, the converse refinement implication is also valid with the natural $L_2$ series interpretation. Suppose this periodization identity and $f(2t)=m(t)f(t)$ hold for a measurable $2\pi$-periodic $m$. Splitting the periodization at $2t$ into even and odd translates gives

$$
\begin{aligned}
1&=\sum_k|f(2t+2\pi k)|^2\\
&=|m(t)|^2\sum_r|f(t+2\pi r)|^2+|m(t+\pi)|^2\sum_r|f(t+\pi+2\pi r)|^2\\
&=|m(t)|^2+|m(t+\pi)|^2.
\end{aligned}
$$

Hence $m$ is bounded and belongs to $L_2$ of a period. Write $m=\tfrac12\sum_na_ne^{-int}$ in $L_2$ and let $m_N$ denote the symmetric partial sums. Since $P=1$,

$$
\int_{\mathbb R}|(m_N(t)-m(t))f(t)|^2\,dt=\int_0^{2\pi}|m_N(t)-m(t)|^2P(t)\,dt\longrightarrow0.
$$

After substituting $t/2$, this proves convergence of the transformed refinement sums to $f$ in $L_2$. Inverting the [Fourier transform](../../../../../../fourier-transform.md) proves $\phi=\sum_na_n\phi(2\cdot-n)$ in $L_2$. Thus **the two spatial conditions and the two Fourier conditions are equivalent**, with the periodic mask and convergence conventions made explicit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
