<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use primes for conformal-time [derivatives](../../../../../../derivative.md) in this question, reserving $V_{,\phi\phi}$ for a potential [derivative](../../../../../../derivative.md). The [inflaton](../../../../../../inflaton.md) background obeys $(a^2\bar\phi')'+a^4V_{,\phi}=0$, so the linear variation of its action vanishes up to boundary terms. With $\delta\phi=f/a$, the [conformal-time quadratic action for an inflaton perturbation](../../../../../../conformal-time-quadratic-action-for-an-inflaton-perturbation.md) is initially

$$
S^{(2)}=\frac12\int d\tau\,d^3x\left[(f'-\mathcal Hf)^2-(\nabla f)^2-a^2V_{,\phi\phi}f^2\right],\qquad\mathcal H=a'/a.
$$

The cross term $-\mathcal H(f^2)'$ integrates to $\mathcal H'f^2$. Since $\mathcal H'+\mathcal H^2=a''/a$, this becomes

$$
\boxed{S^{(2)}=\frac12\int d\tau\,d^3x\left[f'^2-(\nabla f)^2+\left(\frac{a''}a-a^2V_{,\phi\phi}\right)f^2\right]}.
$$

Varying $f$ gives $f''-\nabla^2f+(a^2V_{,\phi\phi}-a''/a)f=0$. The symmetric [Fourier transform](../../../../../../fourier-transform.md) convention used in the question turns $-\nabla^2$ into $k^2$. Dropping the small mass term under the stated [slow-roll inflation](../../../../../../slow-roll-approximation.md) assumption yields

$$
\boxed{f_{\mathbf k}''+\left(k^2-\frac{a''}a\right)f_{\mathbf k}=0}.
$$

For [de Sitter spacetime](../../../../../../de-sitter-spacetime.md), $a=-1/(H\tau)$ with $\tau<0$, so $a''/a=2/\tau^2$. The rescaled field has a canonical kinetic term; $f$ rather than $\delta\phi$ is therefore the convenient oscillator variable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
