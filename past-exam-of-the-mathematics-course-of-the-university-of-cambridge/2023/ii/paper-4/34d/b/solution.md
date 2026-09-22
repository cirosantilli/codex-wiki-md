<h1 id="34d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume $eB>0$; reversing the sign only exchanges the spin labels. Since $\mathbf B\mathbin{\cdot}\boldsymbol\sigma=B\sigma_3$, the Pauli term shifts the spinless energies by $\pm\hbar\omega_c/2$. Thus

$$
E_{n,\sigma}
=\hbar\omega_c\left(n+\frac12+\frac\sigma2\right),
\qquad \sigma=\pm1.
$$

After collecting equal energies, the [spin splitting of Landau levels](../../../../../../spin-splitting-of-landau-levels.md) is

$$
\boxed{E_\ell=\ell\hbar\omega_c},
\qquad \ell=0,1,2,\ldots.
$$

The level $\ell=0$ contains only $(n,sigma)=(0,-1)$ and has degeneracy $D$. Every level $\ell\geq1$ contains $(\ell,-1)$ and $(\ell-1,+1)$ and has degeneracy $2D$.

For $N$ noninteracting electrons, the [Pauli exclusion principle](../../../../../../pauli-exclusion-principle.md) fills these states from the bottom. If $0\leq N\leq D$, every electron fits in the zero-energy level and

$$
E_{\mathrm{gs}}(N)=0.
$$

For $N>D$, write

$$
N-D=2Dk+r,
\qquad k\in\mathbb Z_{\geq0},
\qquad 0\leq r<2D.
$$

Then the first $k$ positive levels are full and $r$ states in level $k+1$ are occupied. The [ground-state](../../../../../../ground-state.md) energy is

$$
\boxed{
E_{\mathrm{gs}}(N)
=\hbar\omega_c\left[Dk(k+1)+(k+1)r\right].
}
$$

Equivalently, on

$$
D(2k+1)\leq N\leq D(2k+3),
$$



$$
E_{\mathrm{gs}}(N)
=D\hbar\omega_c k(k+1)
+(k+1)\hbar\omega_c\,[N-D(2k+1)].
$$

The graph is continuous and piecewise linear: it is flat up to $N=D$, then has slopes $\hbar\omega_c,2\hbar\omega_c,3\hbar\omega_c,\ldots$, with kinks at

$$
\boxed{N=D,3D,5D,\ldots.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [34D](../../34d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
