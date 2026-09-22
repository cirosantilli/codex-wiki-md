<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The stated $M$ is specifically the transfer from the external input to the internal field $b_1$. Combining $b_1=Gb_0$ with $b_0=\beta b_{
m in}-\alpha b_1$ gives

$$
\boxed{\frac{\widetilde b_1}{\widetilde b_{
m in}}=M(s)=\frac{\beta G(s)}{1+\alpha G(s)}
=\frac\beta{1+\alpha}\frac{s-\gamma/2}{s+\gamma_{
m eff}/2}.}
$$

For $\gamma>0$ and a nondegenerate [beam splitter](../../../../../../beam-splitter.md) $|\alpha|<1$, the closed-loop pole is $-\gamma_{
m eff}/2<0$. The return ratio for the [Nyquist stability criterion](../../../../../../nyquist-stability-criterion.md) is $L=\alpha G$. Its frequency locus is a circle of radius $|\alpha|<1$, so it cannot reach or encircle $-1$. The open cavity has no unstable poles; hence the closed loop has none. This agrees with the directly derived state damping rate.

The externally accessible output is different. From $b_2=\alpha b_{
m in}+\beta b_1$,

$$
\boxed{\frac{\widetilde b_2}{\widetilde b_{
m in}}
=\alpha+\beta M=\frac{\alpha+G}{1+\alpha G}
=\frac{s-\gamma_{
m eff}/2}{s+\gamma_{
m eff}/2}.}
$$

It is again an all-pass cavity response. Confusing $b_1$ and $b_2$ would give the wrong output steady state.

For a constant coherent input mean $B=\langle b_{
m in}\rangle$, the steady mean cavity amplitude follows by setting its [derivative](../../../../../../derivative.md) to zero:

$$
\boxed{\langle a\rangle_{
m ss}=-\frac{2\beta}{\sqrt\gamma(1-\alpha)}B,
\quad\langle b_0\rangle_{
m ss}=\frac\beta{1-\alpha}B,
\quad\langle b_1\rangle_{
m ss}=-\frac\beta{1-\alpha}B,
\quad\langle b_2\rangle_{
m ss}=-B.}
$$

The input-output values also follow from $G(0)=-1$ and $M(0)=-\beta/(1-\alpha)$. For any initial mean amplitude, its difference from the stationary mean decays as $e^{-\gamma_{
m eff}t/2}$.

The stability statement needs endpoint qualifications. At $\alpha=1$, normalization forces $\beta=0$, and the cavity obeys $\dot a=0$: it is isolated and undamped, not asymptotically stable. Its external output is nevertheless the decoupled input. At $\alpha=-1$, the algebraic elimination divides by zero; the instantaneous feedback connection is singular and is not a well-posed instance of these reduced equations. Thus strict cavity stability holds for $|\alpha|<1$, not for every real pair satisfying only $\alpha^2+\beta^2=1$.

Finally, $b_{
m in}(t)$ is a quantum stochastic field, so arbitrary inputs do not approach a literal time-independent operator amplitude. The stationary expressions above describe a constant coherent drive's means, or the formal zero-frequency response. The full solution contains the filtered input-noise convolution

$$
a(t)=e^{-\gamma_{
m eff}t/2}a(0)-c\int_0^te^{-\gamma_{
m eff}(t-s)/2}b_{
m in}(s)\,ds.
$$

The stationary cavity [density operator](../../../../../../density-matrix.md) also depends on the input noise statistics. For this ideal passive cavity with a coherent drive and vacuum noise, it is the coherent state with the amplitude just calculated; without such input statistics, the gain function alone does not specify a complete stationary [quantum state](../../../../../../quantum-state.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
