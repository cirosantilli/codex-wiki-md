<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Multiplying the vertical induction equation by $B$ and averaging eliminates advection and gives

$$
\frac12\frac{d}{dt}\langle B^2\rangle=\langle B(A_yU_x-A_xU_y)\rangle-\eta\langle|\nabla B|^2\rangle.
$$

Integrate the derivatives of $A$ by parts. Mixed derivatives of $U$ cancel, leaving

$$
\langle B(A_yU_x-A_xU_y)\rangle=\langle A(B_xU_y-B_yU_x)\rangle.
$$

The pointwise cross-product bound and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) bound its absolute value by $Q\sqrt{\langle A^2\rangle\langle|\nabla B|^2\rangle}$, where $Q=\|\nabla U\|_\infty$. Hence

$$
\boxed{\frac12\frac{d}{dt}\langle B^2\rangle\leq Q\sqrt{\langle A^2\rangle\langle|\nabla B|^2\rangle}-\eta\langle|\nabla B|^2\rangle.}
$$

For $J=\langle|\nabla B|^2\rangle$ and $X=\langle A^2\rangle$, completing the square gives

$$
Q\sqrt{XJ}-\eta J=-\eta\left(\sqrt J-\frac{Q\sqrt X}{2\eta}\right)^2+\frac{Q^2X}{4\eta}.
$$

Apply part (i) and integrate, obtaining the [periodic two-coordinate anti-dynamo energy bound](../../../../../../periodic-two-coordinate-anti-dynamo-energy-bound.md)

$$
\boxed{\langle B^2(t)\rangle-\langle B^2(0)\rangle
\leq\frac{Q^2A_0^2}{4\eta^2k^2}(1-e^{-2\eta k^2t})
\leq\frac{Q^2A_0^2}{4\eta^2k^2}.}
$$

**The printed bound has only one power of diffusivity and is false as written.** Both powers above are needed: one comes from maximizing against diffusion and the other from integrating the decay time of $A$.

For an explicit counterexample in a nondimensional $2\pi$-periodic box, take $u=(0,0,\sin y)$, $A(x,y,0)=\cos x$, $B(x,y,0)=0$, $k=1$. All means vanish and the velocity is solenoidal. The exact solution is

$$
A=e^{-\eta t}\cos x,\qquad
B=\frac1\eta(e^{-\eta t}-e^{-2\eta t})\sin x\cos y.
$$

Indeed $B_h\cdot\nabla U=e^{-\eta t}\sin x\cos y$ and this mode's Laplacian is $-2B$. Here $A_0^2=1/2$, $Q=1$, and at $t=(\log2)/\eta$,

$$
\langle B^2\rangle=\frac1{64\eta^2}.
$$

For $\eta=0.01$ this is $156.25$, exceeding the printed $1/(8\eta)=12.5$. The corrected bound is valid and finite.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
