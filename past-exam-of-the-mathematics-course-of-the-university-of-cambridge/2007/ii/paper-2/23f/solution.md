<h1 id="23f/solution">Solution</h1>

↑ **Parent:** [23F](../23f.md)

Put $b=\operatorname{Im}\tau>0$. On $|\operatorname{Im}z|\le R$, the modulus of the $n$th summand is at most

$$
\exp[-\pi b(n+1/2)^2+2\pi R|n+1/2|].
$$

The resulting Gaussian majorant is summable, independently of the unbounded real part of $z$. The Weierstrass test proves [uniform convergence](../../../../../uniform-convergence.md) on every such strip. Since the summands are entire, locally [uniform convergence](../../../../../uniform-convergence.md) implies **$\psi$ is entire**. It is not identically zero: integrating $\psi(x)e^{-\pi ix}$ over $0\le x\le1$ extracts its nonzero $n=0$ Fourier coefficient.

Logarithmic differentiation of the two supplied transformation laws gives

$$
\boxed{\ell(z+1)=\ell(z),\qquad \ell(z+\tau)=\ell(z)-2\pi i.}
$$

These hold as [meromorphic](../../../../../meromorphic-function.md) identities, with poles at zeros of $\psi$. For a translated fundamental parallelogram with no boundary zeros, opposite edges parallel to $\tau$ cancel by the first identity. The other edge pair contributes $2\pi i$ by the second, so the [argument principle](../../../../../argument-principle.md) counts exactly one zero, including multiplicity, in that parallelogram.

Changing the summation index $n\mapsto-n-1$ shows $\psi(-z)=-\psi(z)$, hence $\psi(0)=0$. Quasiperiodicity makes every lattice point a zero. Every generic fundamental parallelogram contains exactly one lattice point, which already accounts for its one zero; varying its position rules out any additional zeros and proves the lattice zeros are simple. Therefore

$$
\boxed{\{z:\psi(z)=0\}=\Lambda=\mathbb Z+\tau\mathbb Z,\quad\text{all zeros simple}.}
$$

In particular the centred parallelogram in the question has no lattice points on its boundary and its unique zero is zero. Using generic translated contours first avoids assuming this boundary fact before determining the zeros.

For the proposed sum, the first period always holds, while $f(z+\tau)-f(z)=-2\pi i\sum_j\lambda_j$. Thus **it is $\Lambda$-periodic exactly when $\sum_j\lambda_j=0$**. Meromorphicity follows from the [meromorphic](../../../../../meromorphic-function.md) logarithmic derivatives. Finally differentiation removes the additive shift in $\ell$, so **$\frac d{dz}[\psi'(z-a)/\psi(z-a)]$ has both periods** for every $a$.

## ↑ Ancestors (10)

1. [23F](../23f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
