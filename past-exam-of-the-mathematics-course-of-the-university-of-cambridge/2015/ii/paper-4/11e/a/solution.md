<h1 id="11e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a smooth test function $f$, integration by parts in the [Fokker-Planck equation](../../../../../../fokker-planck-equation.md) gives

$$
\frac d{dt}\mathbb E f(x)=\mathbb E\left[A_i\partial_i f+\tfrac12B_{ij}\partial_i\partial_j f\right].
$$

We use the decay and absence of boundary flux intended in the question, sufficiently strong to remove the moment-weighted boundary terms. For $f=x_k$, only $\partial_i f=\delta_{ik}$ survives, giving $d\langle x_k\rangle/dt=\langle A_k\rangle$. For $f=x_kx_l$, the first derivative is $\delta_{ik}x_l+\delta_{il}x_k$ and the second is $\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}$. The [Fokker-Planck diffusion matrix](../../../../../../fokker-planck-diffusion-matrix.md) is symmetric, so

$$
\boxed{\frac d{dt}\langle x_kx_l\rangle=\langle x_lA_k+x_kA_l+B_{kl}\rangle.}
$$

The factor one-half cancels the two equal diffusion contributions, including when $k=l$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11E](../../11e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
