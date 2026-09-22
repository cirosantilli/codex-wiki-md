<h1 id="32d/solution">Solution</h1>

↑ **Parent:** [32D](../32d.md)

Expand a perturbed eigenvector and energy as $\psi=\psi_0+\lambda\psi_1+O(\lambda^2)$ and $E(\lambda)=E+\lambda\delta+O(\lambda^2)$. At first order, $(H-E)\psi_1+(V-\delta)\psi_0=0$. Projecting onto the $E$ eigenspace eliminates the first term and gives $P_EVP_E\psi_0=\delta\psi_0$. Thus [degenerate perturbation theory](../../../../../degenerate-perturbation-theory.md) diagonalizes the restriction of $V$ to that eigenspace; in the nondegenerate case this reduces to its expectation value.

For the specified two-dimensional eigenspace, the restricted matrix is $\begin{pmatrix}\alpha&\beta\\\beta&\alpha\end{pmatrix}$. Its eigenvectors are $(|1\rangle\pm|2\rangle)/\sqrt2$ and its eigenvalues $\alpha\pm\beta$. Hence the perturbed energies are $E+\lambda(\alpha\pm\beta)+O(\lambda^2)$.

The square-box unperturbed energies are $E_{pq}=\pi^2\hbar^2(p^2+q^2)/(2ma^2)$. Every diagonal matrix element of $xy/a^2$ is $1/4$, because each coordinate has mean $a/2$. The [ground state](../../../../../ground-state.md) is $(p,q)=(1,1)$, giving $E_{11}+\lambda/4$. The first excited eigenspace is spanned by $(1,2)$ and $(2,1)$. Its off-diagonal entry factors into the square of

$$
\int_0^1 2s\sin(\pi s)\sin(2\pi s)\,ds=\int_0^1s[\cos(\pi s)-\cos(3\pi s)]ds=-\frac{16}{9\pi^2}.
$$

Thus that entry is $256/(81\pi^4)=(4/(3\pi))^4$, and the three levels are

$$
\boxed{\frac{\pi^2\hbar^2}{ma^2}+\frac\lambda4,\qquad\frac{5\pi^2\hbar^2}{2ma^2}+\lambda\left[\frac14\pm\left(\frac4{3\pi}\right)^4\right].}
$$

The neglected energy corrections are $O(\lambda^2ma^2/\hbar^2)$ in the given weak-field regime.

## ↑ Ancestors (10)

1. [32D](../32d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
