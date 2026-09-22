<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For one channel with momentum $p$, introduce a [Feynman parameter](../../../../../../feynman-parameter.md) and shift the loop momentum:

$$
\frac1{\ell^2(\ell+p)^2}
=\int_0^1dx\,
\frac1{\{(\ell+xp)^2+x(1-x)(-p^2)\}^2}.
$$

In $d=4-\epsilon$, with dimensional-regularization scale $\bar\mu$ before the usual modified-minimal-subtraction redefinition, the bubble at $p^2=-M^2$ is

$$
B(M)=\frac{i}{16\pi^2}
\left[
\frac2\epsilon-\gamma+\log4\pi
-\log\frac{M^2}{\bar\mu^2}
-\int_0^1dx\,\log\{x(1-x)\}
+O(\epsilon)
\right].
$$

Since $\int_0^1\log\{x(1-x)\}\,dx=-2$, summing the three equal channels gives the form displayed in the question, beginning with $6/\epsilon-3\gamma$.

Consequently

$$
-i\lambda_{\mathrm{eff}}
=-i\lambda
+\frac{i\,3\lambda^2}{32\pi^2}
\left[
\frac2\epsilon-\gamma+\log4\pi
-\log\frac{M^2}{\bar\mu^2}+2
\right]
-i\delta\lambda+O(\lambda^3).
$$

The [momentum-subtraction scheme](../../../../../../momentum-subtraction-scheme.md) condition $\lambda_{\mathrm{eff}}(M)=\lambda$ is enforced by

$$
\delta\lambda
=\frac{3\lambda^2}{32\pi^2}
\left[
\frac2\epsilon-\gamma+\log4\pi
-\log\frac{M^2}{\bar\mu^2}+2
\right].
$$

Choosing $\bar\mu=M$ removes the logarithm. A minimal-subtraction scheme keeps only the pole and therefore defines a different finite renormalized coupling.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
