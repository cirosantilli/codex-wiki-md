# WKB quantization condition for a symmetric double well

↑ **Parent:** [WKB quantization condition](wkb-quantization-condition.md)

For a smooth symmetric confining [potential energy](potential-energy.md) with four separated simple [classical turning points](classical-turning-point.md) $-x_2<-x_1<x_1<x_2$, define

$$
\theta(E)=\frac1\hbar\int_{x_1}^{x_2}\sqrt{2m(E-V)}\,dx,\qquad\phi(E)=\frac1\hbar\int_{-x_1}^{x_1}\sqrt{2m(V-E)}\,dx.
$$

The [Airy turning-point connection formula](airy-turning-point-connection-formula.md) applied to a decaying exterior [wavefunction](wave-function-split.md) gives a central [WKB approximation](wkb-approximation.md) proportional to $\chi^{-1/2}[2\cos\theta\,e^K+\sin\theta\,e^{-K}]$, where $\chi=\sqrt{2m(V-E)}$ and $K(x)=\hbar^{-1}\int_x^{x_1}\chi\,dx$. Since $\chi'(0)=0$ and $2K(0)=\phi$, the even [Neumann boundary condition](neumann-boundary-condition.md) gives $\tan\theta=2e^\phi$, while the odd [Dirichlet boundary condition](dirichlet-boundary-condition.md) gives $\tan\theta=-2e^\phi$. For $\phi\gg1$, $\theta=(n+\tfrac12)\pi\mp\tfrac12e^{-\phi}+O(e^{-3\phi})$, with the minus correction for even [parity](parity.md). Since $\theta'=\mathcal T/(2\hbar)$ for the single-well classical [oscillation period](period-of-an-oscillation.md) $\mathcal T$, the leading [double-well tunneling splitting](double-well-tunneling-splitting.md) is $2\hbar e^{-\phi}/\mathcal T$.

## ↑ Ancestors (6)

1. [WKB quantization condition](wkb-quantization-condition.md)
2. [WKB approximation](wkb-approximation.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-further-quantum-theory-course-of-the-university-of-oxford/2023/3/d/solution.md)
