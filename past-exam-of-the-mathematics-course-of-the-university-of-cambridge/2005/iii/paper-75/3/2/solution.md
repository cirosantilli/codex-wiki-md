<h1 id="3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For isotropic initial statistics, isotropic noise preserves $P=P(B,t)$. Isotropy of the noise alone does not turn an arbitrary anisotropic initial vector distribution into an isotropic one; alternatively take the angularly averaged magnitude distribution. The radial gradient satisfies $\partial_jP=P_BB_j/B$, so the diffusion-vector contraction in the preceding equation is $BB_iP_B/2$. Its divergence gives

$$
P_t=\frac{\kappa_2}{4}(B^2P_{BB}+4BP_B)=\frac{\kappa_2}{4B^2}\partial_B(B^4P_B).
$$

Now $F=4\pi B^2P$ is the magnitude [probability density function](../../../../../../probability-density-function.md), normalized by $\int_0^\infty F\,dB=1$. Since

$$
4\pi B^4P_B=B^2F_B-2BF,
$$

we obtain the [radial magnetic-field Fokker-Planck equation](../../../../../../radial-magnetic-field-fokker-planck-equation.md)

$$
\boxed{F_t=D\partial_B(B^2F_B-2BF),\qquad D=\frac{\kappa_2}{4}=\frac\gamma5.}
$$

The outward [Fokker-Planck probability current](../../../../../../fokker-planck-probability-current.md) is $J=-D(B^2F_B-2BF)$. Zero probability flux at zero and infinity preserves normalization. For positive initial magnitude the solution below remains on $B>0$; an atom initially at $B=0$ instead remains an absorbing zero-field component.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
