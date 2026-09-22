<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With the convention $Lu\geq0$ for a classical subsolution, the [weak maximum principle for elliptic operators](../../../../../../weak-maximum-principle-for-elliptic-operators.md) is

$$
\boxed{\sup_\Omega u\leq\max_{\partial\Omega}u,\qquad u\in C^2(\Omega)\cap C(\overline\Omega).}
$$

Here $L$ is uniformly elliptic with bounded drift, has no zeroth-order term, and the domain is bounded. Equivalently, $Lu\leq0$ gives $\inf_\Omega u\geq\min_{\partial\Omega}u$.

One can see why measurable coefficients suffice for the pointwise classical statement by adding $\varepsilon e^{\kappa x_1}$. Choose $\kappa$ large enough that $\lambda\kappa>\|b_1\|_\infty$; then $L(e^{\kappa x_1})=e^{\kappa x_1}(\kappa^2a_{11}+\kappa b_1)>0$. The perturbed subsolution cannot attain a maximum inside: its [gradient](../../../../../../gradient.md) would be zero and its Hessian [negative semidefinite](../../../../../../negative-semidefinite-matrix.md), forcing its elliptic second-order term to be nonpositive. Its maximum is therefore on the boundary. Letting $\varepsilon\downarrow0$ proves the stated estimate. Only the symmetric part of $a$ acts on the Hessian, and ellipticity gives its positive definiteness.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
