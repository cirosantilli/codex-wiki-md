# Direct spherical-shell H2 estimate

↑ **Parent:** [Elliptic boundary value problem](elliptic-boundary-value-problem-split.md)

On a fixed shell $a<r<b$ with $a>0$, put $T=\partial_r^2+2r^{-1}\partial_r$ and $A=\Delta_{S^2}$. If $u$ is smooth and zero on both boundary spheres, direct radial and spherical [integration by parts](integration-by-parts.md) gives

$$
\|\Delta u\|_2^2=\|Tu\|_2^2+\|r^{-2}Au\|_2^2+2\int_a^b\!\int_{S^2}|\nabla_Su_r|^2-2\int_a^b\!\int_{S^2}r^{-2}|\nabla_Su|^2.
$$

The last term is controlled by the first-order energy estimate. The [spherical Hessian identity](spherical-hessian-identity.md) controls angular second [derivatives](derivative.md), and the radial/mixed [derivatives](derivative.md) follow from $T$ and $\nabla_Su_r$. The polar orthonormal-frame formulas for the Cartesian [Hessian matrix](hessian-matrix.md) then prove the estimate. Zero boundary values eliminate the radial boundary remainders because every angular [derivative](derivative.md) of their traces is zero.

## ↑ Ancestors (6)

1. [Elliptic boundary value problem](elliptic-boundary-value-problem-split.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-105/2/f/solution.md)
