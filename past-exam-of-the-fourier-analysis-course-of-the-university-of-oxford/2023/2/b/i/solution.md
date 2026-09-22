<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For real $s$, the [Sobolev space](../../../../../sobolev-space-split.md) $H^s(\mathbb R)$ consists of those [tempered distributions](../../../../../tempered-distribution.md) $u$ whose [Fourier transform](../../../../../fourier-transform-split.md) is represented by a [locally square-integrable function](../../../../../locally-square-integrable-function.md) and for which

$$
\boxed{\|u\|_{H^s}^2:=\int_{\mathbb R}(1+\xi^2)^s|\widehat u(\xi)|^2\,d\xi<\infty.}
$$

This is the [Sobolev norm](../../../../../sobolev-norm.md) used here; inserting the fixed factor $(2\pi)^{-1}$ gives an equivalent convention.

For the [constant function](../../../../../constant-function.md) $c$, [Fourier inversion](../../../../../fourier-inversion-theorem.md) at zero gives

$$
\langle\widehat c,\phi\rangle=c\int\widehat\phi(x)\,dx=2\pi c\phi(0),
\qquad \widehat c=2\pi c\delta_0.
$$

A nonzero [Dirac delta distribution](../../../../../dirac-delta-function.md) cannot be represented by a [locally square-integrable function](../../../../../locally-square-integrable-function.md). Indeed, if $G$ represented $2\pi c\delta_0$, choose a [test function](../../../../../test-function.md) $\rho$ with $\rho(0)=1$, and put $\rho_\varepsilon(\xi)=\rho(\xi/\varepsilon)$. On a fixed [compact interval](../../../../../compact-interval.md) containing their supports, [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
|2\pi c|=\left|\int G\rho_\varepsilon\right|
\leq\|G\|_{L^2(K)}\sqrt\varepsilon\,\|\rho\|_2\longrightarrow0.
$$

Thus $c=0$. Every [Sobolev space](../../../../../sobolev-space-split.md) requires local square integrability of the [Fourier transform](../../../../../fourier-transform-split.md), regardless of how negative $s$ is. Therefore

$$
\boxed{c\in H^s(\mathbb R)\text{ for some }s\in\mathbb R\iff c=0.}
$$

The zero [constant function](../../../../../constant-function.md) belongs to every [Sobolev space](../../../../../sobolev-space-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fourier analysis course of the University of Oxford](../../../../split.md)
6. [Fourier analysis course of the University of Oxford](../../../../../fourier-analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
