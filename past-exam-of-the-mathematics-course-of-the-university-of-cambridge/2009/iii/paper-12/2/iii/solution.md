<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Symmetry implies that all [eigenvalues](../../../../../../eigenvalue.md) of $A(x)$ lie between $\lambda$ and $\Lambda$, so $\|A(x)\|_{\mathrm{op}}\leq\Lambda$. In particular the [bilinear form](../../../../../../bilinear-form.md) $B$ from part (i) is bounded and symmetric under the printed assumptions. The [symmetric elliptic Dirichlet energy with a nonpositive potential](../../../../../../symmetric-elliptic-dirichlet-energy-with-a-nonpositive-potential.md) is

$$
\boxed{J(u)=\frac12\int_\Omega\left(a_{ij}D_juD_iu-qu^2\right)+\int_\Omega fu,\qquad u\in\psi+H_0^1(\Omega).}
$$

All its terms are finite. For an admissible variation $\varphi\in H_0^1$, its [first variation](../../../../../../first-variation.md) is $B(u,\varphi)+\int f\varphi$. Thus stationarity is exactly the [weak formulation](../../../../../../weak-formulation.md) of $Lu=f$.

Here is the [direct method in the calculus of variations](../../../../../../direct-method-in-the-calculus-of-variations.md). Put $u=\psi+w$. Expanding the symmetric [quadratic form](../../../../../../quadratic-form.md) gives

$$
J(\psi+w)=\frac12B(w,w)+B(\psi,w)+\int_\Omega fw+J(\psi)\geq\frac\lambda2\|Dw\|_2^2-C\|Dw\|_2-C.
$$

The [Poincaré inequality](../../../../../../poincare-inequality.md) controls $\|w\|_2$ by $\|Dw\|_2$. Therefore $J$ is bounded below on the admissible class, and a [minimizing sequence](../../../../../../minimizing-sequence.md) is bounded in $H^1$. By weak compactness in this [reflexive Banach space](../../../../../../reflexive-banach-space.md), a subsequence converges weakly to $u$. The affine closed subspace $\psi+H_0^1$ is weakly closed, so $u$ remains admissible.

The symmetric square root $A^{1/2}(x)$ is measurable and bounded. Since $-q\geq0$, the two bounded linear maps

$$
v\longmapsto A^{1/2}Dv,\qquad v\longmapsto\sqrt{-q}\,v
$$

take weak $H^1$ convergence to weak $L^2$ convergence. The [weak lower semicontinuity of the Hilbert norm](../../../../../../weak-lower-semicontinuity-of-the-hilbert-norm.md) shows that $B(u,u)$ is weakly lower semicontinuous. The term $\int fu$ is weakly continuous. Hence $J(u)\leq\liminf J(u_k)$ and $u$ attains the minimum. Varying in either sign yields the weak equation.

The sign $q\leq0$ was used both to make the potential energy nonnegative, hence weakly lower semicontinuous by this argument, and to obtain [coercivity](../../../../../../coercive-function.md). Finally $J(u+z)-J(u)=B(z,z)/2\geq\lambda\|Dz\|_2^2/2$ for $z\in H_0^1$, since the first variation at $u$ vanishes. Therefore

$$
\boxed{\text{the minimizer is unique and is the weak solution of }Lu=f.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
