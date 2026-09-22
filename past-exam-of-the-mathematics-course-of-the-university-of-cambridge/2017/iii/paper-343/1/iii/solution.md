<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

An impenetrable hard wall imposes the [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) $\psi(0)=0$. Choose the bulk [complex argument](../../../../../../argument-complex-analysis.md) to be zero and write a stationary solution as $\psi(y)=\sqrt{n_0}f(y)$ with $f\to1$ as $y\to\infty$. The dimensional [Gross–Pitaevskii equation](../../../../../../gross-pitaevskii-equation.md) becomes

$$
\ell_h^2 f''+(1-f^2)f=0,\qquad f(0)=0,\quad f(\infty)=1.
$$

Multiplication by $f'$ and use of the bulk limit yield the first [integral](../../../../../../integral.md)

$$
\frac{\ell_h^2}{2}(f')^2+\frac{f^2}{2}-\frac{f^4}{4}=\frac14,
\qquad f'=\frac{1-f^2}{\sqrt2\ell_h}
$$

for the increasing wall profile. Integrating gives the [hard-wall condensate healing profile](../../../../../../hard-wall-condensate-healing-profile.md)

$$
\boxed{f(y)=\tanh\frac y\xi,\qquad \xi=\sqrt2\ell_h=\frac\hbar{\sqrt{m\mu}},\qquad
n(y)=\frac\mu g\tanh^2\frac y\xi.}
$$

The PDF's expression without the factor $\mu/g$ is correct for the normalized [number density](../../../../../../number-density.md) $n/n_0$, not for the dimensional [number density](../../../../../../number-density.md) defined at the start of the paper. For example, a bulk [number density](../../../../../../number-density.md) $n_0=2$ must approach $2$, whereas the literal printed expression approaches $1$. If both [number density](../../../../../../number-density.md) and coordinates in this part are understood to have already been normalized, the same result reads $\widetilde n=\tanh^2(\widetilde y/\sqrt2)$ and the dimensionless width is $\sqrt2$. These are two descriptions of the same profile, not different physical [healing lengths](../../../../../../healing-length.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
