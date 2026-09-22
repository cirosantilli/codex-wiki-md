<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $R_i(x)=\left.\partial x_{g(\theta)}/\partial\theta_i\right|_{\theta=0}$ be the infinitesimal orbit tangent vectors. Since $F_j(x_0)=0$, Taylor expansion gives

$$
F_j((x_0)_{g(\theta)})=\sum_iM_{ji}(x_0)\theta_i+O(|\theta|^2),\qquad M_{ji}(x_0)=\sum_a\frac{\partial F_j}{\partial x_a}(x_0)R_i^a(x_0).
$$

This explains the stated linearization. For a linear [group representation](../../../../../group-representation.md), $R_i(x)=t_ix$ in the corresponding action convention.

Two assumptions are implicit in the advertised integration formula. **The slice must be regular, and the determinant sign must be fixed if the absolute value is omitted.** Uniqueness alone does not imply regularity: translations on the line with $F(x)=x^3$ have a unique gauge-fixed representative but $M(0)=0$. For ordinary real integration the [Dirac delta distribution](../../../../../dirac-delta-function.md) change-of-variables formula uses $|\det M|$. The choice $F(x)=-x$ instead has a unique regular zero and negative determinant, illustrating why its sign cannot simply be dropped.

Assume a [regular gauge slice](../../../../../regular-gauge-slice.md) with one representative on each orbit, and choose the action convention $(x_{g_0})_{g(\theta)}=x_{g(\theta)g_0}$, matching the specified right-invariance of [Haar measure](../../../../../haar-measure.md). For the unique $x_0=x_{g_0}$ with $F(x_0)=0$, put $g=g(\theta)g_0$. The Haar density is one at the identity, so changing from $\theta$ to $F$ near the unique zero gives

$$
I(x):=\int_Gd\mu(g)\,\delta^{(p)}(F(x_g))=\frac1{|\det M(x_0)|}.
$$

The integral is orbit invariant by the right-invariance of [Haar measure](../../../../../haar-measure.md). Thus $\Delta(x)=I(x)^{-1}$ is also orbit invariant, and on the gauge slice it equals $|\det M(x)|$. Insert $1=\Delta(x)I(x)$ into the original integral and use its invariant volume measure and invariant $f$:

$$
\begin{aligned}
\int d^nx\,f(x)&=\int_Gd\mu(g)\int d^nx\,f(x)\Delta(x)\delta^{(p)}(F(x_g))\\
&=\int_Gd\mu(g)\int d^ny\,f(y)\Delta(y)\delta^{(p)}(F(y)).
\end{aligned}
$$

In the second line set $y=x_g$. This proves the [finite-dimensional Faddeev-Popov gauge reduction](../../../../../finite-dimensional-faddeev-popov-gauge-reduction.md)

$$
\boxed{\int d^nx\,f(x)=C\int d^nx\,\delta^{(p)}(F(x))|\det M(x)|f(x),\qquad C=\int_Gd\mu(g).}
$$

Choose a positive orientation of the regular slice to obtain the question's $\det M$ form. If the group volume is infinite, its cancellation in normalized quantities is formal or regulated. Multiple intersections and residual zero modes invalidate the simple identity; in a gauge theory these are the [Gribov ambiguity](../../../../../gribov-ambiguity.md) and residual [gauge transformations](../../../../../gauge-transformation.md).

The [Yang-Mills action](../../../../../yang-mills-action.md) counts every [gauge orbit](../../../../../gauge-orbit.md) redundantly in its [path integral](../../../../../path-integral.md), and its quadratic gauge-field operator has gauge zero modes. A [gauge fixing](../../../../../gauge-fixing.md) condition removes this redundancy, while the [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) supplies the orbit-to-slice Jacobian. This is a local perturbative construction with the same regularity qualifications as the finite-dimensional derivation.

Take the linear condition $G[A]=F^\mu A_\mu$. Under an infinitesimal [gauge transformation](../../../../../gauge-transformation.md) $\delta A_\mu=D_\mu\omega$, its change is $\delta G=F^\mu D_\mu\omega$. Hence the [Faddeev-Popov operator](../../../../../faddeev-popov-operator.md) is $\mathcal M[A]=F^\mu D_\mu$. For [Lorenz gauge](../../../../../lorenz-gauge-condition.md), $F^\mu=\partial^\mu$. The [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) acts in the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md).

Average the sharp constraint $G=h$ over $h$ with Gaussian weight $\exp[-i\int h^2/(2\xi)]$. This replaces it by $\exp[-i\int G[A]^2/(2\xi)]$. The [Gaussian gauge fixing with an auxiliary field](../../../../../gaussian-gauge-fixing-with-an-auxiliary-field.md) identity rewrites that factor as

$$
\int Db\,\exp\left[i\int\left(b\cdot G[A]+\frac\xi2b\cdot b\right)\right]\propto\exp\left[-\frac i{2\xi}\int G[A]\cdot G[A]\right],
$$

by completing the square. The bosonic [Nakanishi-Lautrup field](../../../../../nakanishi-lautrup-field.md) $b$ is nondynamical: its algebraic field equation is $b=-G[A]/\xi$. At $\xi=0$ it is a [Lagrange multiplier](../../../../../lagrange-multiplier.md) enforcing $G[A]=0$.

The [Grassmann Gaussian integral](../../../../../grassmann-gaussian-integral.md) exponentiates the determinant, up to a field-independent phase, as

$$
\det\mathcal M[A]\propto\int D\bar c\,Dc\,\exp\left[i\int\bar c\cdot\mathcal M[A]c\right].
$$

The independent anticommuting [Faddeev-Popov ghost field](../../../../../faddeev-popov-ghost.md) $c$ and [Faddeev-Popov antighost field](../../../../../faddeev-popov-antighost-field.md) $\bar c$ are spacetime scalars in the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md). They represent the Jacobian and do not describe physical external fermions. Combining these factors gives

$$
\boxed{\mathcal L_q=-\frac14F^{\mu\nu}\cdot F_{\mu\nu}+b\cdot F^\mu A_\mu+\frac\xi2b\cdot b+\bar c\cdot F^\mu(D_\mu c).}
$$

The parameter $\xi$ selects the Gaussian averaging of the gauge condition. In an anomaly-free regulated treatment, physical [gauge-invariant](../../../../../gauge-invariance.md) observables are independent of this choice. One way to express this is [BRST symmetry](../../../../../brst-symmetry.md): with $sA=Dc$, $s\bar c=-b$ and $sb=0$, the gauge and ghost terms are $s[-\bar c\cdot(G+\xi b/2)]$. The ghost transformation supplies the [off-shell nilpotence of the Yang-Mills BRST quartet](../../../../../off-shell-nilpotence-of-the-yang-mills-brst-quartet.md), and [gauge-fixing parameter independence from BRST symmetry](../../../../../gauge-fixing-parameter-independence-from-brst-symmetry.md) explains why these auxiliary fields do not change the physical content.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
