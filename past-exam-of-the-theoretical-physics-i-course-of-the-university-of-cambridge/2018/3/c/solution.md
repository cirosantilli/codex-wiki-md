<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $R=h_t-\nu\nabla^2h$, where the [diffusion coefficient](../../../../diffusion-coefficient.md) $\nu$ is constant. Then

$$
\delta S=2\int R(\partial_t\delta h-\nu\nabla^2\delta h)\,d^2x\,dt.
$$

One temporal and two spatial [integrations by parts](../../../../integration-by-parts.md) give

$$
\delta S=-2\int(\partial_tR+\nu\nabla^2R)\delta h\,d^2x\,dt,
$$

with compactly supported variations. Hence

$$
\boxed{(\partial_t+\nu\nabla^2)(\partial_t-\nu\nabla^2)h=0,
\qquad h_{tt}-\nu^2\nabla^4h=0.}
$$

Here $\nabla^4=(\nabla^2)^2$ is the [biharmonic operator](../../../../biharmonic-operator.md). The cross terms cancel because $\nu$ is constant and spatial and temporal derivatives commute. Equivalently, $P^0=2R$ and $Q^{ij}=-2\nu R\delta^{ij}$ in part (b), producing $-2\partial_tR-2\nu\nabla^2R=0$.

This [squared diffusion-residual action](../../../../squared-diffusion-residual-action.md) does not have only the first-order [diffusion equation](../../../../diffusion-equation-split.md) as its stationary equation. The zero-residual paths $h_t=\nu\nabla^2h$ have $S=0$ and are certainly solutions, but the variational equation is the higher-order one above. For a spatial [Fourier mode](../../../../fourier-mode.md) with nonzero [wavevector](../../../../wavevector.md) $\mathbf k$, it gives

$$
\ddot h_{\mathbf k}-\nu^2|\mathbf k|^4h_{\mathbf k}=0,\qquad
h_{\mathbf k}(t)=A_{\mathbf k}e^{-\nu|\mathbf k|^2t}+B_{\mathbf k}e^{+\nu|\mathbf k|^2t}.
$$

Boundary data or an additional physical selection principle are needed to retain only the decaying diffusion branch. The spatially uniform mode instead has $h_0(t)=A_0+B_0t$ in the stationary equation.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics I course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics I course of the University of Cambridge](../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
