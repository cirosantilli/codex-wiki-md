<h1 id="a/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The usual [Weyl character formula](../../../../../weyl-character-formula.md) requires **a [compact](../../../../../compact-space.md) [connected](../../../../../connected-space.md) [Lie group](../../../../../lie-group.md)**. Choose a [maximal torus](../../../../../maximal-torus.md) $T$, a positive [root system](../../../../../root-system.md) $\Phi^+$, [Weyl group](../../../../../weyl-group.md) $W$, and $\rho=\frac12\sum_{\alpha\in\Phi^+}\alpha$. Irreducible representations are indexed by dominant integral highest weights $\lambda$ belonging to the [character](../../../../../character-of-a-representation.md) [lattice](../../../../../lattice.md) of the actual [group](../../../../../group-split.md) $T$. For $X\in L(T)$ such that $\exp X$ is regular,

$$
\boxed{\chi_\lambda(\exp X)=
\frac{\sum_{w\in W}\det(w)e^{w(\lambda+\rho)(X)}}
{\sum_{w\in W}\det(w)e^{w\rho(X)}}}.
$$

Weights are written as linear functionals on the complexified [torus](../../../../../torus.md) algebra; their values on the [compact](../../../../../compact-space.md) real [torus](../../../../../torus.md) algebra are imaginary. The denominator is $e^{\rho(X)}\prod_{\alpha>0}(1-e^{-\alpha(X)})$. If $\rho$ is not itself a [character](../../../../../character-of-a-representation.md) of $T$, the individual expressions are interpreted on its covering algebra; their quotient is single-valued and descends to $T$. The apparent singularities at nonregular elements are removable, and conjugacy into a [maximal torus](../../../../../maximal-torus.md) determines the [character](../../../../../character-of-a-representation.md) on the whole [connected](../../../../../connected-space.md) [group](../../../../../group-split.md).

The formula explicitly determines all irreducible characters from their highest weights, and its limit at the identity gives the dimension formula

$$
\dim V_\lambda=\prod_{\alpha>0}\frac{\langle\lambda+\rho,\alpha^\vee\rangle}{\langle\rho,\alpha^\vee\rangle}.
$$

[Character](../../../../../character-of-a-representation.md) multiplication and [orthogonality](../../../../../orthogonal-vectors.md) then compute tensor-product multiplicities. For $SU_2$, highest weights are integers $m\ge0$, and at $\operatorname{diag}(z,z^{-1})$,

$$
\chi_m=\frac{z^{m+1}-z^{-m-1}}{z-z^{-1}}=z^m+z^{m-2}+\cdots+z^{-m},\qquad\dim V_m=m+1.
$$

[Connectedness](../../../../../connected-space.md) cannot simply be omitted from this version. For a nontrivial finite [group](../../../../../group-split.md) the [maximal torus](../../../../../maximal-torus.md) is trivial, yet characters can differ away from the identity. The root data on that [torus](../../../../../torus.md) alone cannot supply the characters of all disconnected [compact](../../../../../compact-space.md) groups.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the lie Groups and Differentiable Manifolds course of the University of Oxford](../../../../split.md)
6. [Lie Groups and Differentiable Manifolds course of the University of Oxford](../../../../../lie-groups-and-differentiable-manifolds-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
