# Legendre polynomial kernel construction

↑ **Parent:** [Kernel of order ell](kernel-of-order-ell.md)

For normalized [Legendre polynomials](legendre-polynomial.md), this [kernel for density estimation](kernel-for-density-estimation.md) reproduces evaluation at zero on every [polynomial](polynomial-split.md) of degree below $\ell$: expand $p$ in the [orthonormal basis](orthonormal-basis.md) to obtain $\int K_\ell p=p(0)$. Taking monomials proves integral one and zero moments of orders $1,\ldots,\ell-1$; [compact support](compact-support.md) gives finite absolute moments. If exact order requires a nonzero moment of order $\ell$, add $(\phi_\ell(0)+1)\phi_\ell\mathbf1_{[-1,1]}$. Lower moments remain unchanged. Writing $a_\ell=\langle u^\ell,\phi_\ell\rangle\ne0$ and evaluating the full expansion of $u^\ell$ at zero shows that the new moment is $a_\ell$. A useful three-derivative example is $K_3=(9-15u^2)\mathbf1_{[-1,1]}/8$, whose first two moments vanish and whose squared [L2 norm](l2-norm.md) is $9/8$.

## ↑ Ancestors (9)

1. [Kernel of order ell](kernel-of-order-ell.md)
2. [Kernel for density estimation](kernel-for-density-estimation.md)
3. [Density estimation](density-estimation.md)
4. [Nonparametric statistics](nonparametric-statistics-split.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31/2/solution.md)
