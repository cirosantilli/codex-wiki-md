<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $t=\sqrt\lambda x$ and $w(t)=y(t/\sqrt\lambda)$. The [chain rule](../../../../chain-rule.md) turns the equation into the parameter-one [Bessel differential equation](../../../../bessel-differential-equation.md). By the regular-at-zero solution property supplied in the paper,

$$
y(x)=cJ_k(\sqrt\lambda x).
$$

For a nonzero solution, $c\ne0$, so $y(1)=0$ forces $J_k(\sqrt\lambda)=0$. Conversely, every positive zero $z$ supplies the admissible eigenfunction $J_k(zx)$ with eigenvalue $z^2$.

Here is a direct justification of the infimum characterization that does not assume a minimizer exists. Let $u(x)=J_k(z_{k,1}x)$ and choose its sign so that $u>0$ on $(0,1)$. The first positive zero exists by the oscillatory large-argument behavior of the [Bessel function of the first kind](../../../../bessel-function-of-the-first-kind.md). At zero, its [Frobenius series for Bessel functions](../../../../frobenius-series-for-bessel-functions.md) gives $u(x)=Cx^k(1+O(x^2))$. At one, its zero is simple by uniqueness for a regular second-order [ordinary differential equation](../../../../ordinary-differential-equation.md). Expanding $y=u(y/u)$ and using the equation for $u$ gives the [Ground-state representation of a Sturm-Liouville energy](../../../../ground-state-representation-of-a-sturm-liouville-energy.md):

$$
I[y]-z_{k,1}^2J[y]=\int_0^1xu(x)^2\left(\frac d{dx}\frac{y(x)}{u(x)}\right)^2dx\geq0.
$$

For completeness, apply the identity first on $[\varepsilon,1-\varepsilon]$. The discarded boundary term is $[xu'y^2/u]$. It tends to zero at both ends: $xu'/u\to k$ and $y=O(x)$ at zero, while $u'/u=O((1-x)^{-1})$ and $y=O(1-x)$ at one. Taking $y=u$ achieves equality, so

$$
\boxed{z_{k,1}^2=\inf_{y\ne0,\ y(0)=y(1)=0}\frac{I[y]}{J[y]}}.
$$

The infimum is over the stated smooth admissible functions with finite energy; the equality also proves attainment by a multiple of $u$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
